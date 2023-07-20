# Network-Traffic-Classification-Techniques-and-Comparative-Analysis-Using-ML-Algorithms
Network Traffic classification has received growing attention over the last years. In the area of networking, it is very essential to know what type of applications flow through the network for the performance of certain tasks. Within the community of the internet, it may be essential to recognize what type of programs are flowing via the networks to execute particular activities. 

Network traffic classification sees its main usage among ISPs (Internet Service Providers) to analyze the characteristics required to design the network, and to determine the qualities needed to construct a connection, which in turn influences the cable network's current effectiveness and hence affects the overall performance of a network. 

There are various techniques adopted to classify internet traffic like Port-based, PayLoad based, Stream, Bandwidth, and Machine Learning based, all of which have their pros and cons. The most common technique used these days by many researchers is Machine Learning (ML) technique which results in giving higher accuracy when compared to others.

In this project,the network traffic classification techniques are discussed step by step, and a real-time internet dataset is developed using the network traffic capture tool Wireshark.The traffic is collected grom an Android and an IOS device.The machine learning classifiers CART DECISION TREE, NAIVE BAYES and SUPPORT VECTOR MACHINE  are then employed on the networking data set and the results are observed and compared. For the implementation of the Machine learning algorithms, the python sklearn library is used along with pandas and NumPy modules.For the purpose of analysis of the results obtained,Excel tool is used.

**A. Network Traffic Capture:**

To start working with the algorithms, we first need to get the data on which we need to employ it. This is the base of every algorithm employment and is known as the data collection step. Numerous tools are employed for capturing network data, popular ones being Wireshark and tcpdump tools. In this paper, the Wireshark tool is used for capturing the network packet which is further analyzed. The real time data of Internet surfing is captured for a duration of 15 minutes and around 50000 entries are produced.
Wireshark is a free and open source packet analyser. It is used for network troubleshooting, analysis, software and communications protocol development, and education.Basically, Wireshark is an open source tool to analyze network traffic or simply speaking, Wireshark captures data from a LAN wire, or from a live network connection or read from a file of already-captured packets. Live data can be read from different types of networks, including Ethernet, IEEE 802.11, PPP, loopback and wifi.
We can create a tcpdump file for the captured traffic. Wireshark allows you to save files in multiple extensions but for our purpose we will use the .pcap extension. It is the most widely used format.In this project we capture data for 15 minutes each from an android and an iphone using wireshark.The data is then converted into a csv file using .csv extension for the analysis purpose.

**B. Network Data Featuring:**

Wireshark provides an easy method to convert data to csv format for further analysis. Anyhow, identifying the correct attribute required to classify the protocol is a challenging task that can be achieved only through extensive study of the topic. Four features are identified that can help in accurate prediction of the protocol and classify network traffic as well. These features are Source IP address, Destination IP address, interval between packets, and length of packet. Target Variable is Protocol.

**C.Network Data Sampling:**

This process is carried out to sample the data. Sampling the data in the supervised technique refers to labeling the data to achieve the purpose of classifying the unknown network classification.

**D.Machine Learning Algorithms used for Analysis:**

This is the implementation step which includes applying machine learning algorithms or classifiers on the instances. For example, applying supervised, unsupervised and semi supervised machine learning algorithms. For the implementation of machine learning algorithms, there are many tools available on the internet such as  MatLab, Weka classification simulation tools etc. In this paper, we use python libraries to achieve these particular tasks such as numpy and pandas. We have made predictions against algorithms such as Naive Bayes, SVM and Cart Decision Tree to get the best results and to do a comparative analysis of the same.The analysis is also done for both IOS and android devices.

**RESULTS**
On using Wireshark for capturing data for two different devices, we can come to a conclusion on the type of traffic that is differing from the two devices.

We find that Cart Decision Tree Classifier outperforms Naive Bayes algorithm and SVM in terms of accuracy for both the datasets which is due to the fact that Decision Trees are discriminative models and uses better classification criterion than Naive Bayes and SVM Algorithms. We find that Cart Decision Tree is the most robust among the algorithms for training data set. It is also able to maintain the highest precision and recall.

On comparing the precision values for both the datasets,since the IOS dataset has more types of traffic compared to the android the Naive Bayes has higher value than that of SVM but lower value than Cart Decision Tree.Recall values for both the datasets follow the trend of the accuracies.
