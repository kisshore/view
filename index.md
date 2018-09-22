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




Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
