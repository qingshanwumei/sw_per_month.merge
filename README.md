# -*- coding: utf-8 -*-
"""
Created on Mon Jul 22 09:47:57 2019

@author: Administrator
"""

import os,re
import pandas as pd

#df=pd.read_excel('./附件一/附件一：SW退网进展（6月）_gd_dengxiaoyun6_00(1)_mz_wukaifa_09.xlsx', sheet_name='1 交换机汇总统计')
#
#df1=df[pd.notna(df['6月份退网数量'])]

#def city_nogd(filename):
#    try:
#       suitablename = filename.replace('_gd_','') 
#       return suitablename
#    except:
#        return filename
#             
#def recity(filename):
#    
#    mod=re.compile(r'_\w\w_')
#    aaa = mod.search(filename)
#    return aaa.group()
print(os.getcwd())

#df = pd.DataFrame(columns=range(17))

for filename in os.listdir('附件一'):
#    filename = '附件一：SW退网进展（6月）_gd__fs_dengxiaoyun6_00.xlsx'
#    try:
        
    df_1 = pd.read_excel('./附件一/'+filename,sheet_name='1 交换机汇总统计') 
#    except:
#        print(filename)


#print(df_1)
#    filename1=city_nogd(filename)
#    titlename=recity(filename1)  
#    
#    df_1['title']=titlename
#    
#    df.colums = df_1.colums
#    df_1=df_1[pd.notna(df_1['6月份退网数量'])]
#    
#    df.append(df_1)
#    
#df.to_excel('Cool.xlsx', sheet_name='Sheet1')
