Originally written by Jack Chessa, paper online can be found at https://www.math.purdue.edu/~caiz/math615/matlab_fem.pdf.  

Modified by Liskelleo, and naturally, by interest. Click `fem-report.pdf` for details of this work.  

Updated Contents are as follow.  
> ---fix certain bugs  
> ---add the boundary of the top edge and the bottom edge  
> ---stress boundaries are given based on elasticity solution of beam  
> ---consider the influence of the beam weight, however may lead to distortion of the left boundary mesh because the stress boundaries are determined with no consideration of gravity (improvement still needed)  
> ---based on the above, when applying gravity, you need to first reset the displacement boundary from few points to full points on the left edge given the structure is shallow cantilever beam (line 189-190 in `beam.m`)

**main program**

---`beam.m`

**additional files of necessity**

---`square_node_array.m`  
---`make_elem.m`  
---`plot_mesh.m`  
---`plot_field.m`  
---`quadrature.m`  
---`lagrange_basis.m`
