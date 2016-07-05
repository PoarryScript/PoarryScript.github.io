---
layout: post
title: 归并排序（Merger）
date: 2016-07-04  21:11:51 
categories: [algorithm]
tags: [algorithm]
---

归并排序
<!--more-->

##  归并排序(Merger Sort)

利用归并算法排序一个数组，可以先递归的将它分成两半分别排序，然后将结果归并起来。归并排序最吸引人的性质是他能够保证任意长度为N的数组排序所需时间和NLogN成正比；它的主要缺点是需要额外空间和N成正比。<br />
**把多个已排好序的数列变成一个排好序的数列的算法

归并排序有二分和归并两个步骤**


##  归并排序(JAVA)代码(Merger Sort) 
     `/**
 	   * 原地归并
	   * @author Poarry
	   *
 	   */
	public class MergerSort {

	public  int[] MergerSort(int[] arrays,int low,int mid,int high) {
		int i = low,j =mid+1;
		int[] temps = new int[arrays.length];
		for (int k = low; k <= high; k++) {
			temps[k] = arrays[k];
		}
		for (int k = low; k <=high; k++) {
			if(i>mid){
				arrays[k] = temps[j++];
				
			}else if (j>high) {
				
				arrays[k] = temps[i++];
			}else if (temps[j]<temps[i]) {
				arrays[k]=temps[j++];
				
			}else {
				arrays[k] = temps[i++];
			}
		}
		return arrays;
	}

	}`


