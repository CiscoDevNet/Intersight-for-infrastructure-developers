## Bringing it all together
Great! Now we see the number of physical compute devices and now we can pull more information from the returned JSON and organize it by Device, Chassis ID, Management Mode, Model, Memory, and CPU. The information in the `Management Mode` column shows if the phsyical compute device is managed in Intersight Management Mode.

> Intersight Managed Mode (IMM) is a new architecture that manages the UCS Fabric Interconnected systems through a Redfish-based standard model. If you are familiar with the UCS blades, it means the Fabric Interconnect is fully managed by Intersight. Instead of having the familiar UCSM (UCS Manager) interface available directly from the Fabric Interconnect, the interface and all of the Fabric Interconnect operations are managed by Intersight.

We do some CLI formatting to organize our data and see the type of compute hardware managed by Intersight along with its resources (memory and CPU). Then, we iterate over the JSON data and pull the data we're interested in. In this instance, the Model shows the UCS-X series hardware.

> Experiment! See if you can add more information to the list below by choosing other items from the returned JSON data above. For example, you could add a column with `num_cpu_cores` and or `ipv4_address` to the code below. There's no right or wrong answer as to which columns you would like displayed.

```python
print ("{:<8} {:12} {:<21} {:<15} {:<10} {:<10}".format(
       'Device',
       'Chassis ID',
       'Management Mode',
       'Model',
        'Memory',
        'CPU'))
for num, items in enumerate(response.json()['Results'], start=1):
    print (
        "{:<8} {:<12} {:<21} {:<15} {:<10} {:<10}".format(
            num, 
            items['ChassisId'], 
            items['ManagementMode'], 
            items['Model'], 
            items['AvailableMemory'], 
            items['CpuCapacity']))
```
<details><summary>Click here to see output</summary>
<pre><code>
Device   Chassis ID   Management Mode       Model           Memory     CPU       
1        1            Intersight            UCSX-210C-M6    512        140.8     
2        1            Intersight            UCSX-210C-M6    1152       145.59999 
3        1            Intersight            UCSX-210C-M6    512        145.59999 
4        1            Intersight            UCSX-210C-M6    512        108.0     
5        1            Intersight            UCSX-210C-M6    512        145.59999 
6        1            Intersight            UCSX-210C-M6    320        145.59999 
</code></pre>
</details> 
**Congratulations! You completed Getting Physical Compute Inventory from Intersight using the Cisco Intersight REST API with Python**
