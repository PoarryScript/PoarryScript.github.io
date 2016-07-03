---
layout: post
title: 归并排序（Merger）
date: 2016-07-1  21:01:01 
categories: [algorithm]
tags: [algorithm]
---

归并排序
<!--more-->

##  归并排序(Merger Sort)

简单插入法是向已排序部分的数列中的大小关系正确的位置插入数据的排序算法


##  归并排序(JAVA)代码(Merger Sort) 
     `/**
	 * 插入排序
	 * 
	 * @author Poarry
	 * 
	 */
	public class InsertSort {
	  public int[] InsertSort(int[] arrays) {
		if(arrays==null||arrays.length<2){
			return arrays;
		}
		int arrayLength = arrays.length;
		
		for (int i = 1; i < arrayLength; i++) {
			for (int j = i; j>0&&j < arrayLength; j--) {
				if(arrays[j-1]>arrays[j]){
					int temp = arrays[j-1];
					 arrays[j-1] = arrays[j];
					 arrays[j]=temp;
				}
				
			}
		}
		return arrays;
	  }

	}`


