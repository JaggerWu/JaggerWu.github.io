---
layout: post
title:  "Time series forecast"
date:   2019-03-23 21:03:36 +0530
categories: C++ Python
---
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse

```cpp
class Solution {
public:
	// #11. Container With Most Water
	int maxArea(vector<int>& height) {
		long maxVol = 0;

		int left = 0, right = height.size() - 1;

		while (left < right)
		{
			int vol = 
				(right - left) * (height[left] < height[right] ? height[left] : height[right]);
			maxVol = vol > maxVol ? vol : maxVol;

			if (height[left] < height[right]) left++;
			else right--;
		}

		return maxVol;
	}

	// #42. Trapping Rain Water
	int trap(vector<int>& height) {
		int maxHeigh, idx = 0;
		for (int i = 0; i < height.size() - 1; i++)
		{

		}
	}
};
```

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
