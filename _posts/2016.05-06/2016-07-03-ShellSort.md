---
layout: post
title: 希尔排序（Shell）
date: 2016-07-03  20:03:23 
categories: [algorithm]
tags: [algorithm]
---

把数据列按照一定间隔分组，组内通过比较大小进行排序而进行排序
<!--more-->

##  希尔排序（Shell）

  希尔排序不是对紧挨着的数据顺序进行排序，而是把有相隔固定距离的数据分为一组，组内进行大小比较并排序，希尔排序与交换排序和插入排序相比稍微复杂一点，但是值得交换处理次数与其它排序比起来能得到很好的控制，所以执行速度很快。<br/>
 对一列有N个元素的数列进行排序时，分割的距离可以取任意数，在这里取数据间隔为N/2。这一组的间隔在对组内数据排序结束后，可以缩短为之前的1/2，即N/2,N/4,N/6,N/8,...
<br/>
<br/>

##  希尔排序（Shell）(JAVA)代码 
    `/**
 	* 希尔排序
 	* @author Poarry
 	*
 	*/
	public class ShellSort {

	public int[] ShellSort(int[] arrays) {
		if(arrays==null){
			return null ;
		}
		int length = arrays.length;
		int h = 1;
		while (h<length/3) {
			h=3*h+1;
			
		}
		while (h>=1) {
			for (int i = h; i < length; i++) {
				for (int j = 0; j >=h&&arrays[j]<arrays[j-h]; j-=h) {
					int temps = arrays[j];
					arrays[j]=arrays[j-h];
					arrays[j-h]=temps;
				}
				h=h/3;
			}
			
		}
		return arrays;				
	}

	}`

