# Hashtable
package com.homework.java;

import java.util.*;

public class HashTableEx {

	public static void main(String[] args) {
		Hashtable<String,String> ht= new Hashtable<String,String>();
		ht.put("one","praksh");
		ht.put("two","thiru");
		ht.put("three","hari");
		ht.put("four","karthic");
		ht.put("five","sathish");
		Hashtable t=new Hashtable();
		t.put("one","hari");
		t.put("seven","prakash");
		ht.putAll(t);
		System.out.println(ht);
		System.out.println(ht.get("four"));
		System.out.println(ht.size());
		System.out.println(ht.remove("five"));
		System.out.println(ht.isEmpty());
		System.out.println(ht.put("six","uma shankar"));
		System.out.println(ht.contains("thiru"));
		System.out.println(ht.containsKey("nine"));

		Set i = ht.keySet();
		for(Object k:i)
		{
			System.out.println(k+"\t"+ht.get(k));
		}
//		
	}
}
o/p====
{five=sathish, two=thiru, one=hari, seven=prakash, three=hari, four=karthic}
karthic
6
sathish
false
null
true
false
six	uma shankar
two	thiru
one	hari
seven	prakash
three	hari
four	karthic

