---
layout: post
title: 交换排序法（冒泡排序）
date: 2016-07-01  0:26:18 
categories: [algorithm]
tags: [algorithm]
---

交换排序法
<!--more-->

##  交换排序法介绍(冒泡排序)


 
 通过比较相邻数据大小来排序。<br />


##交换排序法(冒泡排序)具体步骤 <br />
>  升序排序步骤如下：<br/>
>  条件： 当前有未排序数据arrays[];<br/>
>    1、确定数组索引第一个最为当前需要比较的数，其索引为mCurrentIndex =0； <br />
>  2、 比较arrays[mCurrentIndex]和arrays[mCurrentIndex+1] 位置上的数值大小<br />
>  3、如果arrays[mCurrentIndex]大于arrays[mCurrentIndex+1]，则交换。<br />
>  4、要比较的数值移动一位，即 mCurrentIndex++；直到mCurrentIndex==arrays.length。<br />

##  交换排序法(冒泡排序)(JAVA)代码 
    `/**
 * 交换排序(冒泡排序)
 * @author Poarry
 *
 */
public class SimpleExchangeSort {

	public int[] SimpleExchangeSort(int[] array) {
		if(array.length<=1){
			return array;
		}
		for (int i = 0; i < array.length-1; i++) {
			for (int j = i+1; j < array.length; j++) {
				if(array[i]>array[j]){
					int temp = 0;
					temp =array[j];
					array[j]= array[i];
					array[i] = temp;
				}
			}
		}
		return array;
	}



}
`

<img src="/assets/ico/wechat_qrcode.jpg"  alt="pic" />
