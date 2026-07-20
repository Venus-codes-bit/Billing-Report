Create some new cols after the wide billing report is made, before the report is written to csv:

1) Col name 'Mutiple_Terminus_Queues'. This will be a flag -it will take the value 1 if there are multiple batch set queues present from BS1 to BS7. It will be zero if there is only one terminus queue in BS1 to BS7 and null if Delivered_to_VA=0

2) Col name 'Count_Terminus_Queue': Count of how many terminus queues are present from BS1 to BS7. It will take the value 0 when Delivered_to_VA=0, else it will count the number of terminus queues present in BS1 to BS7.

3) Col name 'Terminus_Queue_Pairs': It will list the terminus queue BS names of a particular case separated by comma in alphabetical order. For e.g. if a case has BS2='Case Closeout' and BS3='OMS Closeout', this col will be Case Closeout, OMS Closeout

4) Col name 'Earliest_Terminus_Queue': It will list the terminus queue BS name of the terminus queue BS with the earliest created on date. If Delivered_to_VA=0 it will be N/A

5) Col name 'Latest_Terminus_Queue': It will list the terminus queue BS name of the terminus queue BS with the latest created on date. If Delivered_to_VA=0 it will be N/A
