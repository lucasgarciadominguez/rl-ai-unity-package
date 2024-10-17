# Generator Reinforcement Learning Cases Package

> Uses the game Iver's Tales https://iguanago.itch.io/ivers-tales as a base for all the models, environment and player controller. 

## Description
 Tool for generating environments that can train an agent model for achieving whatever task is needed. Uses the Reinforcement Learning (RL) algorithm of the ML-Agents library for developing a trained neural network.

## Requirements

Below is a non-exhaustive list of technologies used throughout the project.
### Unity Libraries
<table>
      <thead>
        <tr>
          <th>Libraries</th>
          <th>Version</th>
        </tr>
      </thead>
      <tbody>
            <tr>
              <td>ML Agents</td>
              <td>2.0.1</td>
            </tr>
            <tr>
              <td>New Input System</td>
              <td>1.7.0</td>
            </tr>
      </tbody>
  </table>

### Python Libraries
<table>
      <thead>
        <tr>
          <th>Libraries</th>
          <th>Version</th>
        </tr>
      </thead>
      <tbody>
            <tr>
              <td>Python</td>
              <td>3.9.0</td>
            </tr>
            <tr>
              <td>Numpy</td>
              <td>2.1.0</td>
            </tr>
             <tr>
              <td>Onnx</td>
              <td>1.16.2</td>
            </tr>
            <tr>
              <td>Pytorch</td>
              <td>2.4.0+cpu</td>
            </tr>
             <tr>
              <td>ML-Agents for Python</td>
              <td>0.30.0</td>
            </tr>
      </tbody>
  </table>

## Setup

Steps to follow:

```
py //for checking the version of python, you can use the command $python instead
cd DirectoryUsed
py -m venv venv
venv\Scripts\activate
python -m pip install --upgrade pip
pip install mlagents
pip install protobuf==3.20.3
pip install packaging
mlagents-learn help //for checking missing libraries
```
## How to train an agent

To train a neural network, simply create an agent in Unity that uses ML Agents classes. 
Then follow these steps:

```
mlagents-learn
```
If you want to run a specific ID, type:

```
$mlagents-learn --run-id=IdUsed
```
If you want to run a specific configuration, type:
```
mlagents-learn config/moveToGoal.yaml --run-id=IdUsed
```
  
