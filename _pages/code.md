---
title: Codes
permalink: /codes/
layout: section
active4: active
css_dir: ../css/
---

Testing of higlighter:

```python
class Shape(object):
  def __init__(self):
    self.id = 'base'
```

{% highlight csharp %}
/// <summary>
/// Build data table.
/// </summary>
/// <returns></returns>
static private DataTable Build() {
    DataTable dt = new DataTable( "Data" );
    return dt;
}
{% endhighlight %}

```cpp
/**
 * Week of Code 32
 * Day 3:
 * https://www.hackerrank.com/contest/w32/challenges/circular-walk
 *
 * Author: Joel Enriquez
 * Date: 2017/05/18
 *
 **/
#define sws(v) std::ios_base::sync_with_stdio(v)

#include <algorithm>
#include <cmath>
#include <iostream>
#include <vector>

using namespace std;

void solve()
{
    int n, s, t, g, seed, p;
    cin >> n >> s >> t;
    vector<int> r(n * 2);
    cin >> r[0] >> g >> seed >> p;
    for (int i = 1; i < n * 2; i++)
    {
        if (i % n == 0) r[i] = r[0];
        else r[i] = ((r[i - 1]) * g + seed) % p;
        // cout << r[i] << endl;
    }
    int time = 0, a = 0, b = 0;
    for (int i = s; i < n && s != t; i++)
    {
        bool reached = false;
        int w = 0; // initial weight
        time++;
        a = n + i - r[s];
        b = n + i + r[s];
        cout << "a: " << a % n << endl;
        cout << "b: " << b % n << endl;
        if (a % n <= t || b % n >= t ) break;
        for (int j = a; j <= b; j++)
        {
            cout << "->" << (j + r[j]) % n << endl;
            reached = (j + r[j]) % n >= t;
            if (reached)
            {
                time++;
                break;
            }
            if (r[j] > r[s])
            {
                s = j;
                cout << "s: " << s << endl;
            }
        }
        if (reached) break;
    }
    cout << time << '\n';
}

int main()
{
    #ifdef LOCAL
        freopen("input.txt", "rt", stdin);
        freopen("output.txt", "wt", stdout);
    #endif
    sws(false);
    solve();
    return 0;
}
```
