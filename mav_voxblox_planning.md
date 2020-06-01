**Extra repos to be cloned**  
```catkin_boost_python_buildtool, numpy_eigen, protobuf_catkin, yaml_cpp_catkin```  

**Possible errors while building**  

Issue finding OMPL.  
-> Make appropriate changes int the following files : 
```mav_planning_benchmark CmakeLists, mav_planning_benchmark package.xml, voxblox_rrt_planner CMakeLists``` 

-> Updated ```voxblox``` changes are possibly not reflected in mav_voxblox_planning.  
Revert to commit ```f32a952``` in voxblox  
```git checkout f32a952``` inside voxblox 
