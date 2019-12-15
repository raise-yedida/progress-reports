# December 9 - December 16 Summary

* Improved results a bit by using wider neural nets, but more neurons.

    ![table](./table.png)

* We should instead compare (deep learning literature + our method) vs. (MSR + Lin Tan), i.e., standard deep learning stuff vs. SE literature

    <img src="./compare.png" alt="compare" style="zoom:50%;" />

    * Overall Cohen d (with bias correction): 0.35 (medium effect)

    * Overall Cohen d (without bias correction): 0.40 (medium effect)

    * Individual *diff / pooled SD* values:

        <table>
          <tr>
          	<th>Data</th>
            <th>Cohen d</th>
          </tr>
          <tr>
          	<td>ant 1.5-1.6</td>
            <td>2.63</td>
          </tr>
          <tr>
            <td>ant 1.6-1.7</td>
            <td>4.22</td>
          </tr>
          <tr>
          	<td>camel 1.2-1.4</td>
            <td>-0.55</td>
          </tr>
          <tr>
          	<td>camel 1.4-1.6</td>
            <td>0.14</td>
          </tr>
          <tr>
          	<td>ivy 1.4-2.0</td>
            <td>-0.12</td>
          </tr>
          <tr>
          	<td>jedit 3.2-4.0</td>
            <td>-0.85</td>
          </tr>
          <tr>
          	<td>jedit 4.0-4.1</td>
            <td>1.7</td>
          </tr>
          <tr>
          	<td>log4j 1.0-1.1</td>
            <td>3.3</td>
          </tr>
          <tr>
          	<td>lucene 2.0-2.2</td>
            <td>-3.2</td>
          </tr>
          <tr>
          	<td>lucene 2.2-2.4</td>
            <td>-0.18</td>
          </tr>
          <tr>
          	<td>poi 1.5-2.5</td>
            <td>0.28</td>
          </tr>
          <tr>
          	<td>poi 2.5-3.0</td>
            <td>0.1</td>
          </tr>
          <tr>
          	<td>synapse 1.0-1.1</td>
            <td>-1.0</td>
          </tr>
          <tr>
          	<td>synapse 1.1-1.2</td>
            <td>1.24</td>
          </tr>
          <tr>
          	<td>xalan 2.4-2.5</td>
            <td>-2.3</td>
          </tr>
          <tr>
          	<td>xerces 1.2-1.3</td>
            <td>1.1</td>
          </tr>
        </table>

* Started running Cross-Project Defect Prediction (CPDP)

    <table>
      <tr>
        <th>Data</th>
      	<th>Our method</th>
        <th>MSR</th>
        <th>Lin Tan</th>
        <th>TCA+</th>
      </tr>
      <tr>
      	<td>ant 1.6 - camel 1.4</td>
        <td>33.2 (2.4)</td>
        <td>32</td>
        <td>31.6</td>
        <td>29.2</td>
      </tr>
      <tr>
      	<td>jEdit 4.1 - camel 1.4</td>
        <td>32.4 (1.9)</td>
        <td>31</td>
        <td>69.3</td>
        <td>33</td>
      </tr>
      <tr>
      	<td>camel 1.4 - ant 1.6</td>
        <td>57.0 (2.3)</td>
        <td>45</td>
        <td>97.9</td>
        <td>61.1</td>
      </tr>
      <tr>
      	<td>poi 3.0 - ant 1.6</td>
        <td>57.4 (1.9)</td>
        <td>39</td>
        <td>47.8</td>
        <td>59.8</td>
      </tr>
    </table>

    