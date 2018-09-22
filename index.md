<h1> Cluster1 Info </h1>
<table>
  <th>
    <tr>
      <td> Node </td>
      <td> CPU Requests </td>
      <td> CPU Limits </td>
    </tr>
  </th>
     
{% for x in site.data.cluster1 %}
<tr>
  <td> {{ x.node }} </td>
  <td> {{ x.cpu_requests	}} </td>
  <td> {{ x.cpu_limits	}} </td>
</tr>

{% endfor %}
  
</table> 



{{ site.data }}
