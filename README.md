
<a name="readme-top"></a>
<div align="center">

  

  <h1>Artificial-Intelligence </h1>
  
 

<!-- Badges -->
<p>
  <a href="https://github.com/EmmanuelloDaniele/3D-Porfolio/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/EmmanuelloDaniele/Artificial-Intelligence" alt="contributors" />
  </a>
  <a href="">
    <img src="https://img.shields.io/github/last-commit/EmmanuelloDaniele/Artificial-Intelligence" alt="last update" />
  </a>
  <a href="https://github.com/EmmanuelloDaniele/3D-Porfolio/network/members">
    <img src="https://img.shields.io/github/forks/EmmanuelloDaniele/3Artificial-Intelligence" alt="forks" />
  </a>
  <a href="https://github.com/EmmanuelloDaniele/3D-Porfolio/stargazers">
    <img src="https://img.shields.io/github/stars/EmmanuelloDaniele/Artificial-Intelligence" alt="stars" />
  </a>
  <a href="https://github.com/EmmanuelloDaniele/3D-Porfolio/issues/">
    <img src="https://img.shields.io/github/issues/EmmanuelloDaniele/Artificial-Intelligence" alt="open issues" />
  </a>
  <a href="https://github.com/EmmanuelloDaniele/3D-Porfolio/blob/master/LICENSE">
    <img src="https://img.shields.io/github/license/EmmanuelloDaniele/Threejs_3D_Portfolio.svg" alt="license" />
  </a>
</p>
   
 <h4>
  <span> · </span>
    <a href="https://github.com/EmmanuelloDaniele/Artificial-Intelligence/issues/">Report Bug</a>
  <span> · </span>
    <a href="https://github.com/EmmanuelloDaniele/Artificial-Intelligence/issues/">Request Feature</a>
  </h4>
</div>

<br />

<!-- Agenti -->
<details>

<summary>

# :notebook_with_decorative_cover: Agent


</summary>
<!-- Robot -->
<div align="center"><h1>Robot</h1></div>
<p>In the context of artificial intelligence and robotics, an <strong>agent</strong> is an entity capable of perceiving its environment, making decisions, and taking actions to achieve certain goals. Agents can range from simple programs to complex robotic systems.</p>

<!-- Environment Class -->
<h2>Environment Class:</h2>
<p>The <code>Environment</code> class in this code represents a grid-based environment. It consists of an 11x14 grid with a 1-cell thick border. The grid contains obstacles, represented by cells with a value of 1, and open passages with a value of 0. Additionally, a robot is placed in the environment.</p>

<p>The key functionalities of the <code>Environment</code> class include:</p>
<ul>
  <li><strong>Initialization:</strong> Setting up the grid with borders, obstacles, passages, and placing the robot.</li>
  <li><strong>Perception:</strong> The <code>perceive</code> method returns the values in the 3x3 grid around the robot, excluding the center cell. This mimics the robot's ability to sense its immediate surroundings.</li>
  <li><strong>Movement:</strong> The <code>move</code> method allows the robot to move in different directions (Up, Down, Left, Right) based on the given action, provided the destination cell is not obstructed.</li>
</ul>

<!-- Robot Class -->
<h2>Robot Class:</h2>
<p>The <code>Robot</code> class represents an agent that operates within the defined environment. It interacts with the environment through perception and action.</p>

<p>The main components of the <code>Robot</code> class include:</p>
<ul>
  <li><strong>Initialization:</strong> Associating the robot with a specific environment.</li>
  <li><strong>Action Function:</strong> The <code>action</code> method defines the robot's behavior. It first checks its perception of the environment. If there are no obstacles nearby (sum of perception is 0), it moves upward. The perception is then rearranged to focus on specific directions, and the robot decides its next move based on the presence of obstacles in those directions.</li>
</ul>

<!-- Overall Scenario -->
<h2>Overall Scenario:</h2>
<p>This code simulates a simple scenario where a robot agent navigates through a gridded environment. The environment includes obstacles, and the robot's task is to move toward unobstructed paths while avoiding obstacles. The state of the environment is visually represented to show the current position of the robot and the layout of obstacles.</p>

<p>In summary, this code represents a basic example of an agent (robot) operating in an environment, perceiving its surroundings, and taking actions accordingly. The scenario demonstrates a simple navigation task within a grid-based world.</p>


<!-- Vacum -->
<h2>Vacuum</h2>
<p>The provided Python code represents different agents operating in a vacuum world environment. Each agent has a specific function and behavior for cleaning dirty locations within the environment.</p>


<div align="center"><h1>Vacuum Class:</h1></div>
<p>The <code>Vacuum</code> class serves as the base class for different types of vacuum agents. It contains methods for perceiving the environment, getting the current location, moving, and cleaning. The specific vacuum agents extend this class and implement their unique functionalities.</p>


<h2>Environment Class:</h2>
<p>The <code>Environment</code> class defines the vacuum world environment. It keeps track of the cleanliness status of locations ('A' and 'B'). The <code>perceive</code> method allows agents to gather information about the cleanliness of their current location, and the <code>clean</code> method updates the cleanliness status.</p>


<h2>TableVacuum Class:</h2>
<p>The <code>TableVacuum</code> class is a type of vacuum agent that follows a specific set of rules for moving and cleaning. It checks the cleanliness status of its current location and acts accordingly, moving between locations 'A' and 'B'.</p>

<!-- ReflexVacuum Class -->
<h2>ReflexVacuum Class:</h2>
<p>The <code>ReflexVacuum</code> class is another type of vacuum agent with a reflexive behavior. It cleans if the current location is dirty and moves to the right or left based on the current location.</p>

<!-- BlindVacuum Class -->
<h2>BlindVacuum Class:</h2>
<p>The <code>BlindVacuum</code> class is a vacuum agent with limited perception. It does not know its current location but still cleans if the location is dirty. It moves randomly between right and left.</p>

<!-- ModelVacuum Class -->
<h2>ModelVacuum Class:</h2>
<p>The <code>ModelVacuum</code> class maintains a model of the cleanliness status of both locations. It cleans if the current location is dirty and updates its model. The process continues until both locations are clean.</p>

<!-- Overall Scenario -->
<h2>Overall Scenario:</h2>
<p>This code simulates a vacuum world environment with various types of vacuum agents. Each agent has a unique approach to cleaning dirty locations. The scenario demonstrates different agent architectures, including rule-based reflex agents, random agents, and agents with internal models.</p>

<p>In summary, this code provides a basic implementation of vacuum agents operating in a simple environment, showcasing different agent designs and behaviors for cleaning tasks.</p>


</details>

<!-- Neural Net -->
<details>

<summary>

# :notebook_with_decorative_cover: Neural Net


</summary>

<p>
<p>▶Traning a neural network means fidingi the weights' values that minimize an error function on the traning set.</p>
<p>▶To the optima weights, it is necesssary to use an optimization algorithm</p>
<p>▶The simplest optimization alghorithm is GRADIENT DESCENT</p>
<p>▶Gradient descent is an interative algorithm that can be applied to any diffentiable function</p>

<p>Neural networks are mathematical models inspired by the nervous system</p>
<p>A neural network is composed of a set of artificial neurons.
A neuron is a mathematical model inspirated by the biological neuron A neuron consists of: a set of input connections an aggregation function and an activaction function</p>

<p>▶ The neuron receives a set of inputs x = (x1, x2, . . . , xn, 1).</p>
<p>▶ Each input xi is multiplied by a weight Wi.</p>
<p>▶ The weights W are the parameters of the neural network.</p>
<p>▶ The weights W are initialized randomly.</p>
<p>▶ The weights W are updated during training.</p>

<p>
PyTorch is a very effective deep learning framework for the construction and traning of neural nerworks. It is based on Tensor, which is a multidimensional array(often involves operation on multidimensional data, and the use of tensor simplifies data management). It is efficient for tensor operations and provides numerous optimization algorithms.
</p>

<p> We weill primarilyy use the following components:
</p>
<p>torch.tensor: multidimensional arrays </br>
torch.nn: modules for defining neural networks. </br>
activation functions</br>
layars</br>
loss</br>
torch.optim: modules for optimatization</br></p>

<h2>Try to implement a Neural Net Toy with PyTorch</h2>

```python
import torch
import torch.nn as nn

class ToyNet(nn.Module):
  def __init__(self):
    super(ToyNet, self) .__init__()
    self.fc1 = nn.Linear(2, 1)

  def forward(self, x):
    x = self.fc1(x)
    return x
```

<p> nn.Moduls is base class for all modules in PyTorch NeuralNet</p>

<h2>To Access The Parameters</h2>

```python
>>> net = ToyNet()
>>> print(net)
ToyNet (
  (fc1): Linear(in_features=2, out_features=1, bias=True)
)
>>> for name , param in net.named_parameters():
...   print(name, param)
fc1.weight Paramet contaning:
tensor([[-0.6990, 0.4320]], requires_grad=True)
fc1.bias Parameter contaning:
tensor([-0.0255], requires_grad=True)
```

<p>It is pobbible to modify the parameters of the neural network by directly accessing the tensor</p>
<p>In practice, this is often inconvenient, and prameters are not typically modified manually.</p>

```python
>>> print ( net . fc1 . weight )
tensor ([[ -0.6990 , 0.4320]] , requires_grad = True )
>>> net . fc1 . weight . data = torch . nn . Parameter ( torch . tensor ([[1.0 ,
0.0]]) )
>>> print ( net . fc1 . weight )
tensor ([[1.0 , 0.0]] , requires_grad = True )
```


<h2>Load dates and View</h2>

```python
  def load_data(fie):
    data = np.loadtxt(file)
    x = data [:, : -1]
    y = data [:, -1]
    return torch.tensor(x, dtype=torch.float32),\
            torch.tensor(y, dtype=torch.floar32)
```

```python
import matplotlib.pyplot as plt
def plot(x,y, net):
    plt.scatter(x[:, 0], x[: , 1], c=y)
    w = net.fc1.weight.data
    b = net.fc1.bias.data</code>

    x1 = np.linspace(min(x[:, 0]), max(x[:, 0]), 100)
    # w_0*x + w_1*y +b = 0
    x2 = -(w[0, 0]*x1 +b[0]/w[0, 1])
    plt.plot(x1, x2)
    plt.ylim(min(x[:,1])-1,max(x[:,1])+1)
    plt.show()
  ```

<p>
Correct current error</br>
<detalis>
POSITIVE W^T(x) < 0
WT
t+1x = (Wt + xt)T xt
= WT
t xt + xT
t xt
= WT
t xt + ||xt||2</br>
NEGATIVE 
WT x > 0
WT
t+1x = (Wt − xt)T xt
= WT
t xt − xT
t xt
= WT
t xt − ||xt||2
</detalis>
</p>

```python 
W1 ← 0
t ← 1
while non convergente do
δ ← y−sign(WTt xt)/2
 Wt+1 ← Wt + δxt
 t ← t + 1
 end while
```
<p>
Interpretazione geometrica: rotate the decision hyperplane until the points are correctly classified. IF the data is linearly separable THEN the algorithm converges in a finite number of steps. Otherwise, the algorithm will not converge.
</p>

<h2>Traning: Evaluate the erroe on a sample and update the weights.
</h2>

```python
class ToyNet(nn.Module):
  def __init__(self):
    super(ToyNet, self) .__init__()
    self.fc1 = nn.Linear(2, 1)

  def forward(self, x):
    x = self.fc1(x)
    return x
  
  def train_sample_percepition(self, x,y):
    y_hat = torch.sign(self.forward(x))
    delta = (y - y_hat)/2
    self.fc1.weight.data + = delta*x
    self.fc1.bias.data += delta
```

<h2>Traning Loop
</h2>

```python
net = ToyNet.ToyNer()
x , y = load_data(DATA)

while True:
  #shuffle x and y
  indices = torch.rendperm(len(x))
  x = x[indices]
  y = y[indices]

  for i in range(len(x)):
    net.train_sample_perceptron(x[i], y[i])

  plot(x, y, net)

  y_hat = torch.sign(net.forward(x))
  if torch.all(y_hat.flatten() == y):
      break
print("w:", net.fc1.weight.data)
print("b:", net.fc1.bias.data)
```
<h1>Gradient Descent</h1>
<p>When we examine the learning process of a neural network, we enter the realm of optimization. Efforts are directed towards minimizing a specific error function calculated on the training set. This is the core of neural network training.</br>

Error functions are crucial in this context, and there are several, each suitable for specific types of problems. For classification problems, as in the case of cross-entropy, the goal is to reduce the discrepancy between the network's predictions and the actual labels. The formula, with the summation over all classes, reflects this process of penalizing incorrect predictions.</br>

In regression situations, where numerical values are predicted instead of classes, we often turn to mean squared error. Here, the focus is on minimizing the difference between the network's prediction and the actual value, squared.</br>

It is essential to note that during training, we usually use only a subset of the available data, the training set. This approach allows us to train the network on a representative sample without considering the entire dataset, making the process more efficient.</p>

<h2>SGD Alghorith</h2>
<p>
1Weights W are initialized randomly.</br>
2For each element x in the training set:</br>
2.2 Calculate the network output ˆy = g(WT x).</br>
2.3 Calculate the error through the chosen loss function.</br>
2.4 Calculate the gradient of the loss with respect to the weights ∂L ∂Wi .</br>
2.5 Update the weights in the direction opposite to the gradient.</br>

Repeat the process until the error is sufficiently low or the number of epochs is sufficiently high.</br>
</p>

<h2>Gradient Calculation</h2>
<p>We use Mean Squared Error (MSE) ad the loss fuction.</p>
<p>
Optimization occurs through gradiet descent.
</p>
<p>We differentiate the loss with respect to the output ∂L</p>
<p>Weight Update reule:Wi = Wi − α × (ˆy − y) × xi </p>

```python
class ToyNet(nn.module):
  ...
  def manual_sgd_train(self, x, y, epochs=40, lr=0.05):
    #train using SGD optimizer and MSE loss
    for _ in range (epocs):
      for i in tange(len(x)):
        y_hat = self.forward(x[i])
        error = y_hat - y [i]
        self.fc1.weight.data -= lr * error * x[i]
        self.fc1.bias.data -= lr * error * 1
```
<h2>Not Artigianal Solution</h2>

```python
class ToyNet(nn.Module):
  ...
  def train (self, x, y, epochs=40, lr= 0.05):
    #train using SGD optimizer
    optimizer = torch.optim.SGD(self.parameters(), lr=lr)
    criterion = nn.MSELoss()
    for _ in range(epochs):
      optimizer.zero_grad()
      y_hat = self.forward(x).flatten()
      loss = criterion(y_hat, y)
      loss.backwar()
      optimizer.step()
```
<h2>Funciton for Plotting Classifier not linear with more layer</h2>

```python
def plot2 (X ,y , model , title = " " ) :
    # define bounds of the domain
    min1 , max1 = X [: , 0]. min () -1 , X [: , 0]. max () +1
    min2 , max2 = X [: , 1]. min () -1 , X [: , 1]. max () +1
    # define the x and y scale
    x1grid , x2grid = np . arange ( min1 , max1 , 0.025) , np . arange ( min2 , max2 , 0.025)
    # create all of the lines and rows of the grid
    xx , yy = np . meshgrid ( x1grid , x2grid )
    # flatten each grid to a vector
    r1 , r2 = xx . flatten () , yy . flatten ()
    # horizontal stack vectors to create x1 , x2 input for the model
    grid = [[ x1 , x2 ] for x1 , x2 in zip ( r1 , r2 ) ]
    # make predictions for the grid
    yhat = model . forward ( torch . tensor ( grid , dtype = torch . float32 ) ) . detach () . numpy ()
    # reshape the predictions back into a grid
    zz = yhat . reshape ( xx . shape )
    # plot the grid of x , y and z values as a surface
    plt . contourf ( xx , yy , zz , cmap = ’ viridis ’)
    # create scatter plot for samples from each class
    plt . scatter ( X [: , 0] , X [: , 1] , c =y , cmap = ’ viridis ’ , edgecolors = ’ black ’)
    plt . title ( title )
    # show the plot
    plt . pause (2)
    plt . clf ()
```

</details>

<!-- Search and Problem Solving -->
<details>

<summary>

# :notebook_with_decorative_cover: Search and Problem Solving


</summary>
<h2>Graph Search</h2>
<p>
Many problems can be modeled as graph search problems.</br>
▶ Initial state: the state from which the search begins.</br>
▶ Goal state: the state one wants to reach.</br>
▶ Current state: the state in which the algorithm currently resides.</br>
▶ Operator: an action that modifies the current state.</br>
▶ Path: a sequence of states that leads from the initial state to the current one.</br>
▶ Path cost: the total cost to reach the current state.</br>
Not all of this information is necessary and/or available for every problem.

</p>
  <details>
      <summary>Example</summary>
      <p>▶ The graph is represented by a dictionary of lists (adjacency lists).</br>
      ▶ The keys of the outer dictionary are the nodes of the graph.</br>
      ▶ The graph is non-directed, so each edge is represented twice."</p>
      <p>In this first example, the problem is to find a path from node A to node D (if it exists) by traversing the fewest number of edges.</br>
      ▶ Initial state: A</br>
      ▶ Goal state: D</br>
      ▶ Current state: The node where the algorithm is at each step</br>
      ▶ Operator: Move to an adjacent node</br>
      ▶ Path cost: Number of edges traversed</br>
      To minimize the number of edges traversed, we can use a breadth-first search</p>
  <h4>Implement an agent that performs a breadth-first search.
  </h4>

      
      ```python
      class Agent():
        def __init__(self, graph, start, goal):
          self.graph = graph
          self.goal = goal
          self.frontier = [[start]]

        def next_states(self, path):
            pass
        
        def is_goal(self, state):
            pass

        def bfs(self):
          return self.bfs()  
      ```
 
  <p>
        If the frontier is empty, return None.</br>
        Take the first path from the frontier.</br>
        If the last state of the path is a goal state, return the path.</br>
        Otherwise, generate all obtainable paths by adding a new state to the end of the path (avoiding cycles).</br>
        Add the new paths to the frontier.</br>
        Repeat from step 1.</br>

  It's not always possible to model a graph explicitly.</br>
        ▶ The number of states can be infinite.</br>
        ▶ The graph may be too large to be stored.</br>
        ▶ The graph may be dynamic.</br>
        ▶ Adjacency may be determined by a function.</br>
        The next_states function may need to make less trivial evaluations.</br>
        ▶ We therefore make use of state transformation operators.</br>
        ▶ Given a state and an action, a state transformation operator returns a new state.</br>
  </p>
  </details>

  <details>
  <summary>
      Cannibals and Missionaries.
  </summary>
  <p>Three missionaries and three cannibals need to cross a river.</br>
    ▶ Missionaries and cannibals are initially on the left bank of the river and
    must reach the right bank.</br>
    ▶ To do this, they have a boat that can carry a maximum of two
    people.</br>
    ▶ The boat cannot cross the river without anyone on board.</br>
    ▶ The number of cannibals must never exceed the number of missionaries
    on either bank.</br>
    The goal is to find a minimal sequence of actions that allows
    everyone to cross the river.</br>
  </p>
  <h2>Let's look at the skeleton of an agent that solves the problem.
  </h2>

  ```python
  class Agent():
    def __init__(self):
      pass

    def is_valid(self,state):
      pass # Check state 

    def apply_move(self, state, move):
      pass # Apply a move to a state

    def next_states(self, state):
      pass # Generate all states rechable from a state

    def is_goal(self, state):
      pass # Check if a state is the goal state 

    def bfs(self):
      pass # Implement BFS  
  ```

  <p>
  We represent the state as a dictionary
  </p>

  ```python
  start = {'L': {'missionaries': 3, 'cannibals':3},
           'R': {'missionaries': 0, 'cannibals':0},
           'boat': 'L'}

  goal = {'L': {'missionaries': 0, 'cannibals':0},
          'R': {'missionaries': 3, 'cannibals':3},
          'boat': 'R'}
  ```

  <p>
  Explicitly representing all possible states and their transitions would be too costly. Therefore, we define a list of possible actions that, when applied to a state, generate a new state. Given the position of the boat, the possible actions are:</br>

▶ {’missionaries’: 1, ’cannibals’: 0}: move one missionary</br>
▶ {’missionaries’: 0, ’cannibals’: 1}: move one cannibal</br>
▶ {’missionaries’: 1, ’cannibals’: 1}: move one missionary and one cannibal</br>
▶ {’missionaries’: 2, ’cannibals’: 0}: move two missionaries</br>
▶ {’missionaries’: 0, ’cannibals’: 2}: move two cannibals</br>

However, not all actions are always possible or result in a valid state.
  </p>

  <p>
  We need a function that allows us to check if a state is valid according to the rules of the problem to remove invalid states from the frontier.</br> A state is valid if, on each bank, the number of missionaries is greater than or equal to the number of cannibals, or if there are no missionaries on that bank.
  </p>

<h2>Check Valid State</h2>

  ```python
  def is_valid(self,state):
    left_ok = state['L']['missionaries'] >=
      state['L']['cannibals'] or state ['L']['missionaries'] == 0
    right_ok = state['R']['missionaries'] >=
      state['R']['cannibals'] or state ['R']['missionaries'] == 0
    return left_ok and right_ok
  
  ```
<h2>Apply Move</h2>

  ```python
  def apply_move ( self , state , move ) :
      boat = state [’boat ’]
      new_state = copy . deepcopy ( state )
      new_state [ boat ][ ’ missionaries ’] -= move [’ missionaries ’]
      new_state [ boat ][ ’cannibals ’] -= move [’cannibals ’]

      new_state [’boat ’] = ’L’ if boat == ’R’ else ’R’
      new_state [ new_state [’boat ’]][ ’ missionaries ’] +=
        move [’ missionaries ’]
      new_state [ new_state [’boat ’]][ ’cannibals ’] += move [’cannibals ’]

        return new_state
  ```
<h2>Generate Next States</h2>

  ```python
  def next_states ( self , state ) :
      boat = state [’boat ’]
      next_states = []
      for move in self . moves :
          enough_miss = state [ boat ][ ’ missionaries ’] >= move [’ missionaries ’]
          enough_cann = state [ boat ][ ’cannibals ’] >= move [’cannibals ’]
          if enough_miss and enough_cann :
              new_state = self . apply_move ( state , move )
              if self . is_valid ( new_state ):
              next_states . append ( new_state )
      return next_states

  ```

  <h2>Generate Next States</h2>

  ```python
  def states_to_moves ( self , path ) :
      moves = []
      for i in range (len ( path ) - 1) :
          for move in self . moves :
              if self . apply_move ( path [ i ] , move ) == path [ i + 1]:
                  moves . append ( move )
                  break
      for i in range (len ( moves ) ) :
          moves [ i ] = str( moves [ i ][ ’ missionaries ’]) + ’ missionaries and
          ’ + str( moves [ i ][ ’cannibals ’]) + ’ cannibals from ’ +
          path [ i ][ ’boat ’] + ’ to ’ + path [ i + 1][ ’boat ’]
      return moves
def solve ( self ) :
    path = self . bfs ()
    return self . states_to_moves ( path ) if path else None


  ```

  </details>
</details>

<!-- Search2 -->
<details>

<summary>

# :notebook_with_decorative_cover: Depth First Search

</summary>
<h2>Colors Problem</h2>
<p>The theorem states that, given a flat surface divided into connected regions, such as a political map, four colors are sufficient to color each region in such a way that adjacent regions do not have the same color. This theorem was one of the first to be proven using a computer.</p>

<p>"We store with a dictionary of adjacency lists the graph representing the regions and their adjacencies.</br> Additionally, we store the available colors in a list."</p>

                      ```python
                      adjacency = {
                        'A' : ['B' , 'G', 'F'],
                        'B' : ['A', 'C'],
                        'C' : ['B', 'D', 'F','E'],
                        'D' : ['C'],
                        'E' : ['C'],
                        'F' : ['A','C','G'],
                        'G' : ['A','F']
                      }
                      
                      colors = ['red', 'green', 'blue', 'yellow']
                      ```
<h2>
Constraint checking
</h2>

              ```python
              class DFSAgent:
                def __init__(self,colors, adjacency):
                  self.colors = colors
                  self.adjacency

                def valid_coloring(self, state):
                  for node in state:
                    for neighbors in self.ajacency[node]:
                      if neighbors in state and state[node] == state[neighbors]:
                        return False
                  return True
              ```
<h2>
Possible New Assignments
</h2>

                    ```python
                    def next_moves(self, state):
                      for node in self.adjacency:
                        if node not in state:
                          for color in self.colors:
                            yield(node,color)

                    ```
<h2>
DFS
</h2>
      
          ```python
            def dfs(self, state={}):
              if len(state) == len(self.adjacency):
                yield state
              for node, color in self.next_moves(state):
                new_state = state.copy()
                new_state[node] = color
                if self.valid_coloring(new_state):
                  yield from self.dfs(state=new_state)
              return None
            ```
</details>



</details>

<!-- SGD -->
<details>

<summary>

# :notebook_with_decorative_cover: SGD


</summary>
<p>Utilizzo grafo non orientato rappresentato come un dizionario di liste di adiacenza. Ogni nodo del grafo è una chiave del dizionario, e i suoi vicini sono elencati nelle liste associate.

 definita una classe Agent con un costruttore __init__. Questa classe rappresenta un agente che eseguirà la ricerca in ampiezza (BFS) nel grafo. 
 Gli viene passato il grafo, il nodo di partenza (start), e il nodo obiettivo (goal). self.frontier è una lista di percorsi, inizializzata con il percorso iniziale contenente solo il nodo di partenza.
 Il metodo next_states restituisce i vicini dell'ultimo nodo nel percorso attuale.
is_goal verifica se lo stato corrente è l'obiettivo.
bfs è un generatore che esegue la ricerca in ampiezza.
Estrae il primo percorso dalla frontiera.
Se è l'obiettivo, lo restituisce.
Altrimenti, genera nuovi percorsi aggiungendo i vicini dello stato finale del percorso corrente alla frontiera.
Ricorsivamente continua la ricerca.
Il blocco finale crea un'istanza dell'agente, imposta una lunghezza minima iniziale a infinito, e successivamente itera attraverso i percorsi restituiti dalla BFS. Stampa ogni percorso e aggiorna la lunghezza minima quando trova un percorso più breve.
</p>
</details>

<!-- Deep Learning Image Classifier -->
<details>

<summary>

# :notebook_with_decorative_cover: Deep Learning Image Classification


</summary>
# SGD: Stochastic Gradient Descent
It is an optimization algorithm used to train neural networks and minimize the cost function, aiming to find the global minimum. The stochastic approach stems from the fact that the gradient is calculated on random subsets of the training data rather than the entire dataset.




<h2>1. Install Dependencies and Setup</h2>
In [ ]: <code>!pip install tensorflow tensorflow-gpu opencv-python matplotlib</code></br>
In [ ]: <code>!pip list</code></br>
In [1]: <code>import tensorflow as tf</code></br>
In [1]: <code>import os</code></br>
 # Avoid OOM errors by setting GPU Memory Consumption Growth</br>
In [2]: <code>gpus = tf.config.experimental.list_physical_devices('GPU')</code></br>
In [2]: <code>for gpu in gpus:</code></br>
In [2]: <code>tf.config.experimental.set_memory_growth(gpu, True)</code></br>
In [3]: <code>tf.config.list_physical_devices('GPU')</code></br>

Out [3]: <code>[PhysicalDevice(name='/physical_device:GPU:0', device_type='GPU')] </code></br>

<h2>2. Remove dodgy images</h2>
In [4]: <code>import cv2</code></br>
In [4]: <code>import imghdr</code></br>
In [6]: <code>data_dir = 'data' </code></br>
In [6]: <code>image_exts = ['jpeg','jpg', 'bmp', 'png']</code></br>
 </br>
In [7]: <code>for image_class in os.listdir(data_dir): 
    for image in os.listdir(os.path.join(data_dir, image_class)):
        image_path = os.path.join(data_dir, image_class, image)
        try: 
            img = cv2.imread(image_path)
            tip = imghdr.what(image_path)
            if tip not in image_exts: 
                print('Image not in ext list {}'.format(image_path))
                os.remove(image_path)
        except Exception as e: 
            print('Issue with image {}'.format(image_path))
            # os.remove(image_path)</code></br>

<h2>3. Load Data</h2>
In [8]: <code>import numpy as np
from matplotlib import pyplot as plt</code></br>
In [9]: <code>data = tf.keras.utils.image_dataset_from_directory('data')
</code></br>
Out [9]: Found 305 files belonging to 2 classes.</br>
In [10]: <code>data_iterator = data.as_numpy_iterator()
</code></br>
In [11]: <code>batch = data_iterator.next()</code></br>
In [12]: <code>for image_class in os.listdir(data_dir): 
    fig, ax = plt.subplots(ncols=4, figsize=(20,20))
for idx, img in enumerate(batch[0][:4]):
    ax[idx].imshow(img.astype(int))
    ax[idx].title.set_text(batch[1][idx])</code></br>

<h2>4. Scale Data</h2>
In [13]: <code>data = data.map(lambda x,y: (x/255, y))</code></br>
In [ ]: <code>data.as_numpy_iterator().next()</code></br>


<h2>5. Split Data</h2>
In [15]: <code>train_size = int(len(data)*.7)
val_size = int(len(data)*.2)
test_size = int(len(data)*.1)</code></br>
In [16]: <code>train_size</code></br>
Out [16]: 7</br>
In [17]: <code>train = data.take(train_size)
val = data.skip(train_size).take(val_size)
test = data.skip(train_size+val_size).take(test_size)
</code></br>

<h2>6. Build Deep Learning Model
</h2>
In [18]: <code>train</code></br>
Out [18]: <code><TakeDataset element_spec=(TensorSpec(shape=(None, 256, 256, 3), dtype=tf.float32, name=None), TensorSpec(shape=(None,), dtype=tf.int32, name=None))>
</code></br>
In [19]: <code>from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Conv2D, MaxPooling2D, Dense, Flatten, Dropout</code></br>
In [20]: <code>model = Sequential()
</code></br>
In [21]: model.add(Conv2D(16, (3,3), 1, activation='relu', input_shape=(256,256,3)))
model.add(MaxPooling2D())
model.add(Conv2D(32, (3,3), 1, activation='relu'))
model.add(MaxPooling2D())
model.add(Conv2D(16, (3,3), 1, activation='relu'))
model.add(MaxPooling2D())
model.add(Flatten())
model.add(Dense(256, activation='relu'))
model.add(Dense(1, activation='sigmoid'))</br>
</code></br>
In [22]: <code>model.compile('adam', loss=tf.losses.BinaryCrossentropy(), metrics=['accuracy'])
</code></br>
In [23]: <code>model.summary()
</code></br>
Out [23]: <code>Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 conv2d (Conv2D)             (None, 254, 254, 16)      448       
                                                                 
 max_pooling2d (MaxPooling2D  (None, 127, 127, 16)     0         
 )                                                               
                                                                 
 conv2d_1 (Conv2D)           (None, 125, 125, 32)      4640      
                                                                 
 max_pooling2d_1 (MaxPooling  (None, 62, 62, 32)       0         
 2D)                                                             
                                                                 
 conv2d_2 (Conv2D)           (None, 60, 60, 16)        4624      
                                                                 
 max_pooling2d_2 (MaxPooling  (None, 30, 30, 16)       0         
 2D)                                                             
                                                                 
 flatten (Flatten)           (None, 14400)             0         
                                                                 
 dense (Dense)               (None, 256)               3686656   
                                                                 
 dense_1 (Dense)             (None, 1)                 257       
                                                                 
=================================================================
Total params: 3,696,625
Trainable params: 3,696,625
Non-trainable params: 0
</code></br>


<h2>7. Train
</h2>
In [24]: <code>logdir='logs'

</code></br>
In [25]: <code>tensorboard_callback = tf.keras.callbacks.TensorBoard(log_dir=logdir)

</code></br>
In []: <code>hist = model.fit(train, epochs=20, validation_data=val, callbacks=[tensorboard_callback])

</code></br>

<h2>8. Plot Performance Loss, Accuracy
</h2>
In [27]: <code>fig = plt.figure()
plt.plot(hist.history['loss'], color='teal', label='loss')
plt.plot(hist.history['val_loss'], color='orange', label='val_loss')
fig.suptitle('Loss', fontsize=20)
plt.legend(loc="upper left")
plt.show()
</code></br>
In [28]: <code>fig = plt.figure()
plt.plot(hist.history['accuracy'], color='teal', label='accuracy')
plt.plot(hist.history['val_accuracy'], color='orange', label='val_accuracy')
fig.suptitle('Accuracy', fontsize=20)
plt.legend(loc="upper left")
plt.show()</code></br>

<h2>9. Evaluate
</h2>
In [29]: <code>from tensorflow.keras.metrics import Precision, Recall, BinaryAccuracy
</code></br>
In [30]: <code>pre = Precision()
re = Recall()
acc = BinaryAccuracy()
</code></br>
In [31]: <code> for batch in test.as_numpy_iterator(): 
    X, y = batch
    yhat = model.predict(X)
    pre.update_state(y, yhat)
    re.update_state(y, yhat)
    acc.update_state(y, yhat)
    </code></br>
In [32]: <code>print(pre.result(), re.result(), acc.result())
</code></br>
Out [ ]: tf.Tensor(1.0, shape=(), dtype=float32) tf.Tensor(1.0, shape=(), dtype=float32) tf.Tensor(1.0, shape=(), dtype=float32)</br>

<h2>10. Test
</h2>
In [33]: <code>import cv2
</code></br>
In [39]: <code>img = cv2.imread('154006829.jpg')
plt.imshow(img)
plt.show()
</code></br>
In [40]: <code> resize = tf.image.resize(img, (256,256))
plt.imshow(resize.numpy().astype(int))
plt.show()
    </code></br>
In [41]: <code>yhat = model.predict(np.expand_dims(resize/255, 0))

</code></br>
In [42]: <code>yhat</code></br>
Out [42]: array([[0.01972741]], dtype=float32)</br>
In [42]: <code>if yhat > 0.5: 
    print(f'Predicted class is Sad')
else:
    print(f'Predicted class is Happy')</code></br>
  Predicted class is Happy</br>

<h2>11. Save the Model

</h2>
In [44]: <code>from tensorflow.keras.models import load_model

</code></br>
In [45]: <code>model.save(os.path.join('models','imageclassifier.h5'))

</code></br>
In [46]: <code>new_model = load_model('imageclassifier.h5')
</code></br>
In [47]: <code>new_model.predict(np.expand_dims(resize/255, 0))
</code></br>
Out [47]: array([[0.01972741]], dtype=float32)</br>



</details>

<!-- Rete Neurale SGD -->
<details>

<summary>

# :notebook_with_decorative_cover: Train a Neural Network(SGD)


</summary>
# SGD: Stochastic Gradient Descent
It is an optimization algorithm used to train neural networks and minimize the cost function, aiming to find the global minimum. The stochastic approach stems from the fact that the gradient is calculated on random subsets of the training data rather than the entire dataset.

<h2>To train a neural network means finding the weight values that minimize an error function on the training set.</h2>
▶ To find the optimal weights, it is necessary to use an optimization algorithm.</br>
▶ The simplest optimization algorithm is gradient descent.</br>
▶ Gradient descent is an iterative algorithm that can be applied to any differentiable function.</br>
<p>
x1\
   \
    w3
     \      W^t x
x2--w2->P------------->g(·)------------>
     /                        y
    w1
   /
  /
1/
</p>
The neuron receives a set of inputs x = (x1, x2, . . . , xn, 1), where each input xi is multiplied by a weight Wi.</br>
▶ The weights W are the parameters of the neural network.</br>
▶ The weights W are initialized randomly.</br>
▶ The weights W are updated during training.</br>
Consider a neural network with a single neuron.
The network must learn to separate two linearly separable classes on the plane,
and its activation function is the identity function.
g(x) = x</br>
g′(x) = 1</br>
Dataset:</br>
 x1 |  x2  | y</br>
2.0 |  1.0 | 1</br>
6.0 |  0.5 |-1</br>
2.5 | -1.0 | 1</br>
5.0 |  0.0 |-1</br>
0.0 |  0.0 | 1</br>
4.0 | -1.0 |-1</br>
1.0 |  0.5 | 1</br>
3.0 |  1.5 |-1</br>
</details>
<!-- 8 Regine -->
<details>

<summary>

# :notebook_with_decorative_cover: 8 Queens Problem

</summary>

 <p>
  The problem involves placing 8 queens on a standard 8x8 chessboard in such a way that none of them can threaten or be threatened by another. It is important to note that a queen can move any number of squares horizontally, vertically, or diagonally. The problem is approachable and solvable through different paths, each with varying efficiency and performance.
</p>
<h1>Exercise Text</h1>
Write a Python program to determine the solutions to the Eight Queens puzzle. The Eight Queens puzzle is a problem that involves finding a way to place eight queens (chess pieces) on an 8 × 8 chessboard in such a way that none of them can capture another, using the standard moves of a queen. Therefore, a solution must ensure that no queen shares a column, row, or diagonal with another queen.
Encode the problem state as a list, where each element of the list represents the column in which the queen of the corresponding row is positioned. The chessboard in the figure would be encoded as [6, 2, 7, 1, 4, 0, 5, 3]. The initial state will be an empty list, and each action consists of adding a queen in the next row.
Hint: Define a function `is_valid(state)` that, given a state, returns True if the state is valid and False if it contains two queens in the same column or diagonal (the state encoding prevents two queens from being in the same row).

<h2>Initial Intuitive Approach</h2>

Let's start with the "brute force" solution.

The solution involves generating all possible arrangements of 8 queens on an 8x8 chessboard, totaling 64 squares. Using the binomial coefficient, we calculate that these arrangements amount to 4,426,165,368. We write a program that generates all arrangements and discards those where at least one queen threatens another. The number of arrangements to analyze is significantly high. To speed up the solution, we need to simplify the problem, for example, by reducing the number of arrangements to be analyzed.

<h2>Simplify.</h2>

A first simplification could be, for example, to impose only one queen per row. Two queens in the same row threaten each other horizontally.

And in the eight rows, all the queens are definitely arranged in different positions (columns) in our solution. To avoid threats vertically. 

So, on the entire chessboard, in our solution, we will definitely have a row with a queen in the leftmost position, a row with the queen in the second position, and so on. 

This simplified algorithm, instead of generating all the arrangements described above, generates only the possible combinations of 8 rows, each with a queen in a different position. In the first row, I have 8 possible positions. In the second one, I have seven (actually, I have 5 or 6, considering the diagonally threatened squares). In the third one, I have six, and so on. These combinations are 8 factorial (8! == 40320), an order of magnitude lower than the arrangements calculated above. Here we have to generate the combinations and discard all those where at least one queen threatens another. 

The threat can only come diagonally, as threats horizontally and vertically have already been eliminated "by construction."
Can we optimize further?

For a problem of order 8, about forty thousand combinations to analyze are relatively few. But what if we want to solve the problem with 16 queens on a 16x16 chessboard? Or if we wanted to solve the problem with 24? 24 Factorial (24!) is a number of the order of 10^23. If we had a billion computers, each capable of examining a billion combinations per second, we could calculate all the solutions in about a week of computation. Definitely too many combinations to generate and analyze in "human" time with limited resources. We need to further simplify the problem to make it manageable.

<h2>But let's go back to the order 8 problem. </h2>

For example, we can think of starting to check diagonal threats even with incomplete combinations, while building them, without waiting to have placed all the queens to do so. For each row, therefore, before placing a queen in the candidate square, I check for diagonal threats on this square. If the square is threatened, I move on to the next one in the row. I place the queen in the non-threatened and not previously tried position. If I reach the end of the row without other available positions, I go back to the previous row, where I apply the same logic, looking for a new arrangement for that queen. When I have placed all 8 queens on the 8 rows, the solution is valid; I count it and print or store it. And I continue the search. When I have generated all possible combinations, I stop.

This approach lends itself very well to a recursive implementation. If in the current row there are no other usable positions because all have already been tried or are threatened by the queens placed in the previous rows, I interrupt the search on the current row and trigger backtracking, returning to the previous row. By not trying (and therefore not verifying) all possible complete combinations, it is clearly much more efficient than the previous ones. Because when I trigger backtracking due to a lack of positions in the current row, I am actually discarding a large portion of combinations to be analyzed. I am discarding all at once the entire subtree of possible combinations, but certainly not valid. A tree that can be decidedly large. 
<h2>How do we know if a square is threatened?</h2>

As mentioned above, if we want to extend the problem from 8 to 12, 16, or even 24 queens, respectively on 12x12, 16x16, or 24x24 chessboards, the first solutions proposed above run into the exponential and factorial complexity of the problem. And become therefore inapplicable. The recursive method remains still applicable, even for problem sizes larger than 8. Now we need a fast method to understand if the square analyzed is threatened by the queens already placed above. Coupled with an efficient method for representing this data in memory, so that we can both arrange the queens and check threats very quickly. Intuitively, we could use an 8x8 matrix to represent the chessboard. As we will see later, there are more compact and efficient structures, given the nature of the data and calculations to be done. For now, let's use a matrix to graphically represent what we want to do. We use an 'R' symbol to place a queen in a row of the matrix and an 'M' symbol to indicate that a square is threatened.

We number rows and columns starting from the top left corner, with row and column numbers ranging from 0 to 7. At the beginning, we place the first queen at (0,0) (row, column) and mark the threatened squares. 

To place the second queen in the second row, we use the square in the third column, at (1,2). Because (1,1) is threatened diagonally. And here we mark the threatened squares as well. 

To place the third queen in the third row (row 2), we can only place it starting from the fifth column (2,4), as the previous ones from (2,0) to (2,3) are all threatened. 

And so on. As you can see, every time we place a queen, several combinations are avoided in the future, due to the threatened squares. In the 3rd row, for example, we start exploring the tree with the queen at (3,1) to see if it contains solutions. Once done exploring this, we will try with the queen at (3,6), discarding the previous ones from (3,2) to (3,5), as they are threatened. In the 5th row, we only have the possibility to place our queen at (5,3).

<h2>What if the threat comes diagonally?</h2>

As mentioned above, by construction, if we place a queen per row, in a position different from the queens in the previous rows, we immediately exclude threats horizontally and vertically. We only need to verify if the "candidate" position is threatened diagonally by the queens placed previously. For example, we can say that a queen in position (4,5) is threatened by the queen in the previous row (row 3) only if this queen is in position (3,4) or in position (3,6). The squares diagonally at the top right and top left of (4,5).

If it is, we stop and find the next candidate square. If it is not, we go and check if it is threatened by the queen in row 2. The square (4,5) is threatened by the queen in row 2 if it is in position (2,3) or in position (2,7). 

And so on, until checking if our candidate square (4,5) is threatened by the queen in the first row (row 0). We must then generate the coordinates of the squares in the two diagonally right and left directions above the position we are checking and check if a queen is present at these coordinates.

For (4,5), which is our candidate square, these "threatening" squares are:

(3,4), (2,3), (1,2), (0,1) for the left diagonal 

(3,6), (2,7) for the right diagonal 

In general, to check if the square (j,k) is threatened diagonally by the queens arranged above, we must check, row by row starting from row j, the presence of a queen in the squares that have column k-1 or k+1 in row j-1, k-2 or k+2 in row j-2, k-3 or k+3 in row j-3, etc., backward to row 0. If we get a negative column (less than zero) or greater than 7, of course, we can ignore the check. 


</details>





<!-- Contact -->


##  More info  :handshake: Contact

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/emmanuello) 
<p dir="auto">Daniele Emmanuello - <a href="https://www.linkedin.com/in/emmanuellodaniele/" rel="nofollow">@Linkedin</a> -<a href="https://t.me/emmanuellodaniele"rel="nofollow">@Telegram</a></p> 

<p align="right">(<a href="#readme-top">back to top</a>)</p>
