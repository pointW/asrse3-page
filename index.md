In the spatial action representation, the action space spans the space of target poses for robot motion commands, i.e. SE(2) or SE(3). This approach has been used to solve challenging robotic manipulation problems and shows promise. However, the method is often limited to a three dimensional action space and short horizon tasks. This paper proposes ASRSE3, a new method for handling higher dimensional spatial action spaces that transforms an original MDP with high dimensional action space into a new MDP with reduced action space and augmented state space. We also propose SDQfD, a variation of DQfD designed for large action spaces. ASRSE3 and SDQfD are evaluated in the context of a set of challenging block construction tasks. We show that both methods outperform standard baselines and can be used in practice on real robotics systems.

<div style="text-align:center">
	<img src="img/alg_overview.png" alt="alg" height="300"/>
</div>

Our model learns to select action sequentially. q<sub>1</sub> maps the heightmap image onto a \|X\| X \|Y\| map of Q values with a maximum at a<sub>xy</sub>. Given that selection of a<sub>xy</sub>, q<sub>2</sub> predicts Q values for a<sub>theta</sub>. Similarly, q<sub>3</sub>, q<sub>4</sub>, and q<sub>5</sub> predicts Q values for a<sub>z</sub>, a<sub>phi</sub>, and a<sub>psi</sub>, respectively.

## Paper
[arXiv:2010.02798[cs.RO]](https://arxiv.org/abs/2010.02798)

[Dian Wang](https://pointw.github.io), 
[Colin Kohler](https://www.khoury.northeastern.edu/people/colin-kohler/), 
[Robert Platt](http://www.ccs.neu.edu/home/rplatt/)

Northeastern University

```
@article{wang2020policy,
  title={Policy learning in SE (3) action spaces},
  author={Wang, Dian and Kohler, Colin and Platt, Robert},
  journal={arXiv preprint arXiv:2010.02798},
  year={2020}
}
```

## Video

<div style="text-align:center">
	<iframe width="853" height="480" src="https://www.youtube.com/embed/FiHoIF1oLZs" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

## Contact
If you have any questions, please feel free to contact [Dian Wang](https://pointw.github.io) at wang[dot]dian[at]northeastern[dot]edu.