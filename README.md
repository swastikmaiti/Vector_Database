# Vector Database
Implementing Vector Database on CoNaLa: The Code/Natural Language Challenge dataset to retrieve program snippets relevant to user queries. 

<br>
Vector Database is implemented with in-memory vector database using Qdrant library. Embeddings are created using Sentence Transformer.
<br>
<br>


### Some Results
1. input: Farm.objects.filter(tree__in=TreeQuerySet)<br>
score: 0.7407113992591807<br>
{'intent': 'Getting Unique Foreign Keys in Django?', 'snippet': 'Farm.objects.filter(tree__in=TreeQuerySet)'}<br>
score: 0.604259202467448<br>
{'intent': 'How to get all children of queryset in django?', 'snippet': "Category.objects.filter(animal__name__startswith='A')"}<br>
score: 0.5979930194641302<br>
{'intent': 'How to get all children of queryset in django?', 'snippet': "Animals.objects.filter(name__startswith='A')"}<br>

2. input: python -> time a while loop has been running<br>
score: 0.8861537367742911<br>
{'intent': 'python -> time a while loop has been running', 'snippet': 'time.sleep(1)'}<br>
score: 0.6401777126086143<br>
{'intent': 'Exit while loop in Python', 'snippet': 'sys.exit()'}<br>
score: 0.6401777126086143<br>
{'intent': 'exit while loop in python', 'snippet': 'sys.exit()'}<br>

3. input: ax.legend(handles[::-1], labels[::-1], title='Line', loc='upper left')<br>
score: 0.9006352410454543<br>
{'intent': 'Reverse the order of legend', 'snippet': "ax.legend(handles[::-1], labels[::-1], title='Line', loc='upper left')"}<br>
score: 0.7188311901852373<br>
{'intent': 'Duplicate items in legend in matplotlib?', 'snippet': 'handles, labels = ax.get_legend_handles_labels()'}<br>
score: 0.7188311901852373<br>
{'intent': 'duplicate items in legend in matplotlib?', 'snippet': 'handles, labels = ax.get_legend_handles_labels()'}<br>
