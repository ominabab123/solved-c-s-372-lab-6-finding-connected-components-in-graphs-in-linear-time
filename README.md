Download Link: https://assignmentchef.com/product/solved-c-s-372-lab-6-finding-connected-components-in-graphs-in-linear-time
<br>









You will implement algorithms to find connected components in undirected graphs and strongly connected components in directed graphs. In this lab, you can re­use the DFS code you did in Lab 5.

<h1>1        Requirement for the algorithms</h1>

<h2>1.1       Connected components in undirected graphs</h2>

Implement the first algorithm to find connected components in an undirected graph with the following function prototype:

vector &lt;size_t &gt;             find_connected_components ( Graph &amp; G)

{

}

The input must be treated as an undirected graph <em>G</em>. The output is a vector containing connected component ids for each node in the graph. The id of node <em>i </em>must be contained in the <em>i</em>­th entry of the vector. If the graph has <em>K </em>connected components, the ids must range from 0 to <em>K </em>− 1.

The algorithm must run in <em>O</em>(|<em>V </em>| + |<em>E</em>|) time.

<h2>1.2       Strongly connected components in directed graphs</h2>

Implement the second algorithm to find <em>strongly </em>connected components in a directed graph with the following function prototype:

vector &lt;size_t &gt;                          find_strongly_connected_components ( Graph &amp; G)

{

}

The input must be treated as an directed graph <em>G</em>. The output is a vector containing connected component ids for each node in the graph. The id of node <em>i </em>must be contained in the <em>i</em>­th entry of the vector. If the graph has <em>K </em>connected components, the ids must range from 0 to <em>K </em>− 1.

As the standard solution to strongly connected components relies on previsit and postvisit time stamps for each node using DFS on the reverse graph of <em>G</em>, will the recursive and iterative DFS algorithms (from Lab 5) generate different time stamps? If so, which one you will use for strongly connected components? Please discuss this in your lab report.

<h1>2        Test the classes</h1>

Generate five example undirected graphs and five example directed graphs to test your code. The graphs do not have to be very large but must represent a variety: cyclic/acyclic, directed/undirected, having one or more connected components.

Your C++ program must include a main() function that calls the testall() function. When the program is compiled by a C++ compiler it generates a binary executable file that will run when invoked from the command line.

<h1>3        Graphtheruntimeasafunctionofnumberofnodes and edges</h1>

After testing the correctness of the the program, you will study how the runtime scale with the size of graph for the two methods. Use the random graph function you developed in Lab 4 to generate random graphs of increasing sizes.

You will produce four curves in R:

<ol>

 <li>find_connected_components runtime as a function of number of nodes in the graph, given the number of edges</li>

 <li>find_strongly_connected_components runtime as a function of number of nodes in the graph, given the number of edges</li>

 <li>find_connected_components runtime as a function of number of edges in the graph, given the number of nodes</li>

 <li>find_strongly_connected_components runtime as a function of number of edges in the graph, given the number of nodes</li>

</ol>

You will design sizes of the graphs so that your runtime will change substantially among the sizes.


