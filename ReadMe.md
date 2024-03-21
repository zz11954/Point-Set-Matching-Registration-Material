# Point Set Matching/Registration Material

A list of point set matching / point set registration resources. 

## Table of Contents

- [Point Set Matching/Registration Material](#point-set-matchingregistration-material)
  - [Table of Contents](#table-of-contents)
  - [Point Set Matching/Registration Methods](#point-set-matchingregistration-methods)
    - [Point Matching/Registration Methods](#point-matchingregistration-methods)
    - [Mismatch Removal/Correspondence Pruning Methods](#mismatch-removalcorrespondence-pruning-methods)
    - [Graph Matching Methods](#graph-matching-methods)
    - [Misc](#misc)
    - [Deep Features](#deep-features)
  - [Applications](#applications)
    - [Remote Sensing Image Registration](#remote-sensing-image-registration)
    - [Retinal Image Registration](#retinal-image-registration)
    - [Palmprint Image Registration](#palmprint-image-registration)
    - [Visual Homing Navigation](#visual-homing-navigation)
    - [HDR Imaging](#hdr-imaging)
    - [Misc](#misc-1)
  - [Databases](#databases)
    - [General databases](#general-databases)
    - [Other databases](#other-databases)
  - [Tools](#tools)


<a name="pm1"></a>
## Point Set Matching/Registration Methods


<a name="pm"></a>
### Point Matching/Registration Methods

- [MCT] A mathematical analysis of the motion coherence theory, IJCV'1989 [[pdf]](http://www.cs.jhu.edu/~ayuille/PubsJournal/J16YuilleGrzywacz89.pdf)
- [ICP: point-to-point] Method for Registration of 3-D Shapes, Robotics-DL tentative'1992 [[pdf]](http://www.cs.virginia.edu/~mjh7v/bib/Besl92.pdf) [[code]](http://staffhome.ecm.uwa.edu.au/~00053650/code/icp.m)[[code]](http://www.open3d.org/docs/tutorial/Basic/icp_registration.html) [[code]](https://ww2.mathworks.cn/matlabcentral/fileexchange/27804-iterative-closest-point) [[material]](http://ais.informatik.uni-freiburg.de/teaching/ss12/robotics/slides/17-icp.pdf) [[tutorial]](http://www.sci.utah.edu/~shireen/pdfs/tutorials/Elhabian_ICP09.pdf)
- [ICP: point-to-plane] Object modeling by registration of multiple range images, IVC'1992 [[pdf]](http://graphics.stanford.edu/courses/cs348a-17-winter/Handouts/chen-medioni-align-rob91.pdf)
- [ICP] Iterative point matching for registration of free-form curves and surfaces, IJCV'1994 [[pdf]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.175.770&rep=rep1&type=pdf)
- [RPM/Softassign] New algorithms for 2d and 3d point matching: pose estimation and correspondence, PR'1998 [[pdf]](http://cmp.felk.cvut.cz/~amavemig/softassign.pdf) [[code]](https://www.cise.ufl.edu/~anand/students/chui/rpm/TPS-RPM.zip) [[code]](https://github.com/tttamaki/cuda_emicp_softassign)
- [MultiviewReg] Multiview registration for large data sets, 3DDIM'1999 [[pdf]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.50.2416&rep=rep1&type=pdf)
- [SC] Shape matching and object recognition using shape contexts, TPAMI'2002 [[pdf]](https://apps.dtic.mil/dtic/tr/fulltext/u2/a640016.pdf)[[wiki]](https://en.wikipedia.org/wiki/Shape_context) [[project]](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/shape/sc_digits.html) [[code]](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/code/sc_demo/)
- [EM-ICP] Multi-scale EM-ICP: A Fast and Robust Approach for Surface Registration, ECCV'2002 [[pdf]](ftp://ftp-sop.inria.fr/epidaure/Publications/Granger/eccv-2002.pdf) [[code]](https://github.com/tttamaki/cuda_emicp_softassign)
- [LM-ICP] Robust registration of 2D and 3D point sets, IVC'2003 [[pdf]](http://luthuli.cs.uiuc.edu/~daf/courses/Opt-2019/Papers/sdarticle.pdf) [[code]](http://research.microsoft.com/~awf/lmicp/)
- [TPS-RPM] A new point matching algorithm for non-rigid registration, CVPR'2000 [[pdf]](https://ieeexplore.ieee.org/abstract/document/854733/) CVIU'2003 [[pdf]](http://www.cvl.iis.u-tokyo.ac.jp/class2013/2013w/paper/correspondingAndRegistration/05_RPM-TPS.pdf) [[project]](https://www.cise.ufl.edu/~anand/students/chui/tps-rpm.html) [[code]](https://www.cise.ufl.edu/~anand/students/chui/rpm/TPS-RPM.zip)
- [Survey] Image registration methods: a survey, IVC'2003 [[pdf]](https://www.researchgate.net/profile/Jan_Flusser/publication/222648347_Image_Registration_Methods_A_Survey/links/5ba9f31c92851ca9ed238b48/Image-Registration-Methods-A-Survey.pdf)
- [KCReg] A correlation-based approach to robust point set registration, ECCV'2004 [[pdf]](http://www.cs.cmu.edu/afs/.cs.cmu.edu/Web/People/ytsin/research/kcreg.pdf) [[chp]](http://www.cs.cmu.edu/~ytsin/thesis/chap2.pdf) [[code]](http://www.cs.cmu.edu/~ytsin/KCReg/)
- [3DSC] Recognizing objects in range data using regional point descriptors, ECCV'2004 [[pdf]](http://www.cs.jhu.edu/~misha/Papers/Frome04.pdf) [[code_pcl]](https://github.com/PointCloudLibrary/pcl/blob/master/examples/features/example_shape_contexts.cpp)
- [RGR] Robust Global Registration, ESGP'2005 [[pdf]](http://vecg.cs.ucl.ac.uk/Projects/SmartGeometry/global_registration/paper_docs/global_registration_sgp_05.pdf)
- [RPM-LNS] Robust point matching for nonrigid shapes by preserving local neighborhood structures, TPAMI'2006 [[pdf]](https://www.researchgate.net/profile/Yefeng_Zheng/publication/7211798_Robust_point_matching_for_nonrigid_shapes_by_preserving_local_neighborhood_structures/links/0deec527101e1d3269000000/Robust-point-matching-for-nonrigid-shapes-by-preserving-local-neighborhood-structures.pdf) [[code]](http://www.umiacs.umd.edu/user.php?path=zhengyf/PointMatching.htm)
- [IT-FFD] Shape registration in implicit spaces using information theory and free form deformations, TPAMI'2006 [[pdf]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.60.2593&rep=rep1&type=pdf)
- [Rigid] Rigid Body Registration, 2007 [[ch02]](https://www.fil.ion.ucl.ac.uk/spm/doc/books/hbf2/pdfs/Ch2.pdf)
- [CDC] Simultaneous covariance driven correspondence (cdc) and transformation estimation in the expectation maximization framework, CVPR'2007 [[pdf]](http://www.cs.rpi.edu/~sofka/pdfs/sofka-cvpr07.pdf) [[project]](https://msofka.github.io/projects/cdc/)
- [Nonrigid-ICP] Optimal step nonrigid icp algorithms for surface registration, CVPR'2007 [[pdf]](https://gravis.dmi.unibas.ch/publications/2007/CVPR07_Amberg.pdf) [[code]](https://ww2.mathworks.cn/matlabcentral/fileexchange/54077-optimal-step-nonrigid-icp) [[code]](https://github.com/charlienash/nricp)
- [GNA] Global non-rigid alignment of 3D scans, TOG'2007 [[pdf]](http://www.academia.edu/download/30932674/10.1.1.93.609.pdf)
- [PF] Particle filtering for registration of 2D and 3D point sets with stochastic dynamics, CVPR'2008 [[pdf]](https://smartech.gatech.edu/bitstream/handle/1853/28587/2008_IEEE_CCVPR.pdf?sequence=1&isAllowed=y)
- [JS] Simultaneous nonrigid registration of multiple point sets and atlas construction, TPAMI'2008 [[pdf]](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2921641/)
- [4PCS] 4-points congruent sets for robust pairwise surface registration, TOG'2008 [[pdf]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.140.4881&rep=rep1&type=pdf) [[project]](http://graphics.stanford.edu/~niloy/research/fpcs/fpcs_sig_08.html)
- [GICP] Generalized ICP, RSS'2009 [[pdf]](http://www.robots.ox.ac.uk/~avsegal/resources/papers/Generalized_ICP.pdf) [[code]](https://github.com/avsegal/gicp)
- [MP] 2D-3D registration of deformable shapes with manifold projection, ICIP'2009 [[pdf]](https://www.researchgate.net/profile/Alessio_Del_Bue/publication/223134711_2D-3D_Registration_Of_Deformable_Shapes_With_Manifold_Projection/links/0912f50d0a439af072000000.pdf)
- [SMM] The mixtures of Student’s t-distributions as a robust framework for rigid registration, IVC'2009 [[pdf]](http://www.academia.edu/download/45493807/imavis09.pdf)
- [Algebraic-PSR] An Algebraic Approach to Affine Registration of Point Sets, ICCV'2009 [[pdf]](https://www.researchgate.net/profile/Anand_Rangarajan/publication/221111832_An_Algebraic_Approach_to_Affine_Registration_of_Point_Sets/links/0c960520d3ec57741c000000.pdf)
- [SM] Subspace matching: Unique solution to point matching with geometric constraints, ICCV'2009 [[pdf]](http://www.isr.ist.utl.pt/~manuel/pubs/iccv09.pdf)
- [FPFH] Fast Point Feature Histograms (FPFH) for 3D Registration, ICRA'2009 [[pdf]](http://www.cvl.iis.u-tokyo.ac.jp/class2016/2016w/papers/6.3DdataProcessing/Rusu_FPFH_ICRA2009.pdf) [[code]](http://pointclouds.org/documentation/tutorials/fpfh_estimation.php)
- [GO] Global optimization for alignment of generalized shapes, CVPR'2009 [[pdf]](http://projectsweb.cs.washington.edu/research/insects/CVPR2009/optim_learning/glbloptim_alignshape.pdf)
- [ISO] Isometric registration of ambiguous and partial data, CVPR'2009 [[pdf]](http://www.tevs.eu/files/cvpr09.pdf)
- [GF] A new method for the registration of three-dimensional point-sets: The Gaussian fields framework, IVC'2010 [[pdf]](https://www.researchgate.net/profile/Faysal_Boughorbel/publication/222524708_A_new_method_for_the_registration_of_three-dimensional_point-sets_The_Gaussian_Fields_framework/links/59e8a674a6fdccfe7f8ea302/A-new-method-for-the-registration-of-three-dimensional-point-sets-The-Gaussian-Fields-framework.pdf)
- [RotInv] Rotation invariant non-rigid shape matching in cluttered scenes, ECCV'2010 [[pdf]](https://pdfs.semanticscholar.org/6131/9215b7934ca4e7262fd67f7d6a493665d258.pdf) [[code]](https://matlab1.com/shop/matlab-code/rotation-invariant-non-rigid-shape-matching-in-cluttered-scenes/)
- [CDFHC] Group-wise point-set registration using a novel cdf-based havrda-charvát divergence, IJCV'2010 [[pdf]](https://www.cise.ufl.edu/~anand/pdf/CDFHC.pdf) [[code]](http://www.cise.ufl.edu/~tichen/cdfHC.zip)
- [QPCCP] A quadratic programming based cluster correspondence projection algorithm for fast point matching, CVIU'2010 [[pdf]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.231.3553&rep=rep1&type=pdf) [[code]](http://www.voidcn.com/link?url=http://www4.comp.polyu.edu.hk/~cslzhang/code/QPCCP.zip)
- [CPD] Point set registration: Coherent point drift, NIPS'2007 [[pdf]](http://papers.nips.cc/paper/2962-non-rigid-point-set-registration-coherent-point-drift.pdf) TPAMI'2010 [[pdf]](https://arxiv.org/pdf/0905.2635) [[code]](https://sites.google.com/site/myronenko/research/cpd)
- [PFSD] Point set registration via particle filtering and stochastic dynamics, TPAMI'2010 [[pdf]](http://iss.bu.edu/tannenba/publications/papers/sandhu-pami09-pointset.pdf)
- [ECMPR] Rigid and articulated point registration with expectation conditional maximization, TPAMI'2011 [[pdf]](https://hal.inria.fr/docs/00/43/57/72/PDF/RR-7114.pdf) [[project]](https://team.inria.fr/perception/research/ecmpr/) [[code]](https://team.inria.fr/perception/files/2015/04/ecmpr_demo.zip)
- [GMMReg/TPS-L2] Robust point set registration using gaussian mixture models, ICCV'2005 TPAMI'2011 [[pdf]](https://ieeexplore.ieee.org/abstract/document/5674050/) [[code]](https://github.com/bing-jian/gmmreg)
- [TPRL] Topology preserving relaxation labeling for nonrigid point matching, TPAMI'2011 [[pdf]](https://ieeexplore.ieee.org/abstract/document/5590251/)
- [OOH] Robust point set registration using EM-ICP with information-theoretically optimal outlier handling, CVPR'2011 [[pdf]](https://ieeexplore.ieee.org/abstract/document/5995744)
- [SGO] Stochastic global optimization for robust point set registration, CVIU'2011
- [survey] 3D Shape Registration, 3DIAA'2012
- [3DNDT-D2D/P2D] Fast and accurate scan registration through minimization of the distance between compact 3D NDT representations, IJRR'2012 [[pdf]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.817.5962&rep=rep1&type=pdf) [[project]](http://wiki.ros.org/ndt_registration)
- [Multiview LM-ICP] Accurate and automatic alignment of range surfaces, 3DIMPVT'2012 [[pdf]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.403.2173&rep=rep1&type=pdf) [[code]](https://github.com/adrelino/mv-lm-icp)
- [ISC] Intrinsic shape context descriptors for deformable shapes, CVPR'2012 [[pdf]](http://www0.cs.ucl.ac.uk/staff/I.Kokkinos/pubs/KokkinosBronstein_ISC_CVPR12.pdf)
- [RPM-Concave] Robust point matching revisited: A concave optimization approach, ECCV'2012 [[pdf]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.297.8822&rep=rep1&type=pdf) [[code]](http://www.voidcn.com/link?url=http://www4.comp.polyu.edu.hk/~cslzhang/code/RPM_concave.rar)
- [RINPSM] Rotation Invariant Nonrigid Point Set Matching in Cluttered Scenes, TIP'2012 [[pdf]](http://azadproject.ir/wp-content/uploads/2014/07/2011-Rotation-Invariant-Nonrigid-Point-Set-Matching-in-Cluttered-Scenes.pdf) [[code]](http://www4.comp.polyu.edu.hk/~cslzhang/code/dynamProg_minSpanTreeTri_shapCont_TIP.rar)
- [RPM-L2E] Robust estimation of nonrigid transformation for point set registration, CVPR'2013 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2013/papers/Ma_Robust_Estimation_of_2013_CVPR_paper.pdf) [[code]](https://github.com/jiayi-ma?tab=repositories)
- [GO-ICP] Go-ICP: Solving 3D Registration Efficiently and Globally Optimally, ICCV'2013 [[pdf]](https://www.cv-foundation.org/openaccess/content_iccv_2013/papers/Yang_Go-ICP_Solving_3D_2013_ICCV_paper.pdf) TPAMI'2016 [[pdf]](https://arxiv.org/pdf/1605.03344) [[code]](https://github.com/yangjiaolong/Go-ICP)
- [Survey] Registration of 3D point clouds and meshes: a survey from rigid to nonrigid, TVCG'2013 [[pdf]](https://orca.cf.ac.uk/47333/1/ROSIN%20registration%20of%203d%20point%20clouds%20and%20meshes.pdf)
- [NMM] Diffeomorphic Point Set Registration Using Non-Stationary Mixture Models, ISBI'2013 [[pdf]](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3886289/)
- [Sparse-ICP] Sparse Iterative Closest Point, ESGP'2013 [[pdf]](https://dl.acm.org/citation.cfm?id=2600305) [[project]](http://jlyang.org/go-icp/) [[code]](https://lgg.epfl.ch/sparseicp)
- [IRLS] Robust registration of point sets using iteratively reweighted least squares, COA'2014 [[pdf]](https://link.springer.com/article/10.1007/s10589-014-9643-2) [[code]](https://ww2.mathworks.cn/matlabcentral/fileexchange/12627-iterative-closest-point-method?s_tid=FX_rc3_behav)
- [JRMPC] A Generative Model for the Joint Registration of Multiple Point Sets, ECCV'2014 [[pdf]](https://hal.archives-ouvertes.fr/docs/01/01/96/61/PDF/main_cr.pdf) [[project]](https://team.inria.fr/perception/research/jrmpc/) [[code&data]](https://team.inria.fr/perception/files/2015/05/JRMPC_v0.9.4.zip)
- [RPM-VFC] Robust Point Matching via Vector Field Consensus, TIP'2014 [[pdf]](http://or.nsfc.gov.cn/bitstream/00001903-5/99530/1/1000009269450.pdf) [[code]](https://github.com/jiayi-ma?tab=repositories)
- [GLTP] Non-rigid Point Set Registration with Global-Local Topology Preservation, CVPRW'2014 [[pdf]](https://www.cv-foundation.org/openaccess/content_cvpr_workshops_2014/W04/papers/Ge_Non-rigid_Point_Set_2014_CVPR_paper.pdf)
- [color-GICP] Color supported generalized-ICP, VISAPP'2014 [[pdf]](https://pdfs.semanticscholar.org/1560/394a1d34567e7434b8188df59af8103b233f.pdf)
- [RPM-Concave] Point Matching in the Presence of Outliers in Both Point Sets: A Concave Optimization Approach, CVPR'2014 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2014/papers/Lian_Point_Matching_in_2014_CVPR_paper.pdf) [[code]](http://www.voidcn.com/link?url=http://www4.comp.polyu.edu.hk/~cslzhang/code/RPM_concave.rar)
- [super4PCS] Super 4pcs fast global pointcloud registration via smart indexing, CGF'2014 [[pdf]](https://hal.archives-ouvertes.fr/hal-01538738/document) [[code]](https://github.com/nmellado/Super4PCS) [[OpenGR]](https://github.com/STORM-IRIT/OpenGR)
- [SDTM] A Riemannian framework for matching point clouds represented by the Schrodinger distance transform, CVPR'2014 [[pdf]](https://www.cv-foundation.org/openaccess/content_cvpr_2014/papers/Deng_A_Riemannian_Framework_2014_CVPR_paper.pdf)
- [GLMD-TPS] A robust global and local mixture distance based non-rigid point set registration, PR'2015 [[pdf]](https://www.researchgate.net/profile/Yang_Yang634/publication/266562735_A_robust_global_and_local_mixture_distance_based_non-rigid_point_set_registrationincluding_source_codes-link_data/links/5abda9d60f7e9bfc0457c21d/A-robust-global-and-local-mixture-distance-based-non-rigid-point-set-registrationincluding-source-codes-link-data.pdf) [[code]](https://ww2.mathworks.cn/matlabcentral/fileexchange/47409-glmdtps-registration-method)
- [CSM] Non-rigid point set registration via coherent spatial mapping, SP'2015 [[pdf]](http://matlabtools.com/wp-content/uploads/p410-5.pdf)
- [ADR/SVR] An Adaptive Data Representation for Robust Point-Set Registration and Merging, ICCV'2015 [[pdf]](http://openaccess.thecvf.com/content_iccv_2015/papers/Campbell_An_Adaptive_Data_ICCV_2015_paper.pdf) [[code]](https://www.google.com/url?q=https%3A%2F%2Fresearch.csiro.au%2Fdata61%2Fwp-content%2Fuploads%2Fsites%2F85%2F2016%2F02%2Fsvr.zip&sa=D&sntz=1&usg=AFQjCNFq89C_xVHCbvvtcnBZA4yyGNdMpg) [[code]](https://github.com/neka-nat/probreg)
- [MLMD] MLMD: Maximum likelihood mixture decoupling for fast and accurate point cloud registration, 3DV'2015 [[pdf]](http://jankautz.com/publications/MLMD_3DV15.pdf) [[project]](https://www.cc.gatech.edu/~kihwan23/)
- [APSR] Non-rigid Articulated Point Set Registration for Human Pose Estimation, WACV'2015 [[pdf]](https://www.researchgate.net/profile/Guoliang_Fan2/publication/274955205_Non-rigid_Articulated_Point_Set_Registration_for_Human_Pose_Estimation/links/552d199a0cf29b22c9c4ad61.pdf)
- [RegGF] Non-rigid visible and infrared face registration via regularized Gaussian fields criterion, PR'2015 [[pdf]](https://www.researchgate.net/profile/Jiayi_Ma/publication/268882090_Non-rigid_visible_and_infrared_face_registration_via_regularized_Gaussian_fields_criterion/links/5bb4ba0c45851574f7f7c1b8/Non-rigid-visible-and-infrared-face-registration-via-regularized-Gaussian-fields-criterion.pdf) [[code]](https://github.com/jiayi-ma?tab=repositories)
- [LLT] Robust feature matching for remote sensing image registration via locally linear transforming, TGRS'2015 [[pdf]](https://yuan-gao.net/pdf/TGRS2015.pdf) [[code]](https://github.com/jiayi-ma?tab=repositories)
- [RPM-L2E] Robust L2E estimation of transformation for non-rigid registration, TSP'2015 [[pdf]](https://www.researchgate.net/profile/Jiayi_Ma/publication/273176803_Robust_L2E_Estimation_of_Transformation_for_Non-Rigid_Registration/links/552142f10cf2f9c130512304.pdf) [[code]](https://github.com/jiayi-ma?tab=repositories)
- [GLR] Robust Nonrigid Point Set Registration Using Graph-Laplacian Regularization, WACV'2015 [[pdf]](https://ieeexplore.ieee.org/abstract/document/7046010/)
- [FPPSR] Aligning the dissimilar: A probabilistic method for feature-based point set registration, ICPR'2016 [[pdf]](https://ieeexplore.ieee.org/abstract/document/7899641/)
- [IPDA] Point Clouds Registration with Probabilistic Data Association, IROS'2016 [[pdf]](https://ieeexplore.ieee.org/abstract/document/7759602/) [[code]](https://github.com/ethz-asl/robust_point_cloud_registration)
- [CPPSR] A probabilistic framework for color-based point set registration, CVPR'2016 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2016/papers/Danelljan_A_Probabilistic_Framework_CVPR_2016_paper.pdf) [[project]](http://www.cvl.isy.liu.se/research/cogvis/colored-point-set-registration/index.html)
- [GOGMA] GOGMA: Globally-optimal gaussian mixture alignment, CVPR'2016 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2016/papers/Campbell_GOGMA_Globally-Optimal_Gaussian_CVPR_2016_paper.pdf) [[project]](https://sites.google.com/view/djcampbell/research-software)
- [GO-APM] An Efficient Globally Optimal Algorithm for Asymmetric Point Matching, TPAMI'2016 [[pdf]](http://www4.comp.polyu.edu.hk/~cslzhang/APM_files/data/APM.pdf) [[project]](http://www4.comp.polyu.edu.hk/~cslzhang/APM.htm) [[code]](http://www4.comp.polyu.edu.hk/~cslzhang/APM_files/data/RPM_COV_source_code.rar)
- [PR-GLS] Non-Rigid Point Set Registration by Preserving Global and Local Structures, TIP'2016 [[pdf]](https://www.researchgate.net/profile/Jiayi_Ma/publication/281082006_Non-Rigid_Point_Set_Registration_by_Preserving_Global_and_Local_Structures/links/55e6478108aecb1a7ccd6883.pdf) [[code]](https://github.com/jiayi-ma?tab=repositories)
- [conreg] Non-iterative rigid 2D/3D point-set registration using semidefinite programming, TIP'2016 [[pdf]](https://arxiv.org/pdf/1501.00630)
- [PM] Probabilistic Model for Robust Affine and Non-rigid Point Set Matching, TPAMI'2016 [[pdf]](https://ieeexplore.ieee.org/abstract/document/7439870/)
- [SPSR] A Stochastic Approach to Diffeomorphic Point Set Registration With Landmark Constraints, TPAMI'2016 [[pdf]](https://ieeexplore.ieee.org/abstract/document/7130637/)
- [FRSSP] Fast Rotation Search with Stereographic Projections for 3D Registration, TPAMI'2016 [[pdf]](https://www.cv-foundation.org/openaccess/content_cvpr_2014/papers/Bustos_Fast_Rotation_Search_2014_CVPR_paper.pdf)
- [VBPSM] Probabilistic Model for Robust Affine and Non-rigid Point Set Matching, TPAMI'2016 [[pdf]](https://ieeexplore.ieee.org/abstract/document/7439870/) [[code]](https://www.computer.org/csdl/trans/tp/2016/12/07416224-abs.html)
- [MFF] Image Correspondences Matching Using Multiple Features Fusion, ECCV'2016 [[pdf]](http://icvl.ee.ic.ac.uk/DescrWorkshop/featw-papers/Paper_0005.pdf) [[code]](http://press.liacs.nl/researchdownloads)
- [FGR] Fast Global Registration, ECCV'2016 [[pdf]](https://link.springer.com/chapter/10.1007/978-3-319-46475-6_47) [[code]](https://github.com/intel-isl/FastGlobalRegistration)
- [HMRF ICP] Hidden Markov Random Field Iterative Closest Point, arxiv'2017 [[pdf]](https://arxiv.org/pdf/1711.05864) [[code]](https://github.com/JStech/ICP)
- [SSFR] Global Registration of 3D LiDAR Point Clouds Basedon Scene Features: Application toStructured Environments, RS'2017 [[pdf]](https://www.mdpi.com/2072-4292/9/10/1014/pdf)
- [color-PCR] Colored point cloud registration revisited, ICCV'2017 [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Park_Colored_Point_Cloud_ICCV_2017_paper.pdf)
- [CGF] Learning Compact Geometric Features, ICCV'2017 [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Khoury_Learning_Compact_Geometric_ICCV_2017_paper.pdf) [[code]](https://github.com/marckhoury/CGF)
- [dpOptTrans] Efficient Globally Optimal Point Cloud Alignment using Bayesian Nonparametric Mixtures, CVPR'2017 [[pdf]](https://www.researchgate.net/profile/Jonathan_How/publication/301839970_Efficient_Globally_Optimal_Point_Cloud_Alignment_using_Bayesian_Nonparametric_Mixtures/links/5744700508ae9f741b3f0aa0/Efficient-Globally-Optimal-Point-Cloud-Alignment-using-Bayesian-Nonparametric-Mixtures.pdf) [[code]](https://github.com/jstraub/dpOptTrans)
- [DO] Discriminative Optimization: Theory and Applications to Point Cloud Registration, CVPR'2017 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2017/papers/Vongkulbhisal_Discriminative_Optimization_Theory_CVPR_2017_paper.pdf) [[arxiv]](https://www.youtube.com/redirect?event=video_description&v=br0ZAhLAbWg&q=https%3A%2F%2Farxiv.org%2Fabs%2F1707.04318&redir_token=nPJirhhzMzIQBudyujEVxs064jh8MTU1NzI0Mjk2OEAxNTU3MTU2NTY4) [[code]](https://github.com/jayakornv/discriminative-optimization)
- [GORE] Guaranteed Outlier Removal for Point Cloud Registration with Correspondences, TPAMI'2017 [[pdf]](https://arxiv.org/pdf/1711.10209)
- [CSGM] A systematic approach for cross-source point cloud registration by preserving macro and micro structures, TIP'2017 [[pdf]](https://arxiv.org/pdf/1608.05143)
- [FDCP] Fast descriptors and correspondence propagation for robust global point cloud registration, TIP'2017 [[pdf]](https://ieeexplore.ieee.org/abstract/document/7918612/)
- [RSWD] Multiscale Nonrigid Point Cloud Registration Using Rotation-Invariant Sliced-Wasserstein Distance via Laplace-Beltrami Eigenmap, SIAM JIS'2017 [[pdf]](https://epubs.siam.org/doi/abs/10.1137/16M1068827)
- [MR] Non-Rigid Point Set Registration with Robust Transformation Estimation under Manifold Regularization, AAAI'2017 [[pdf]](https://www.aaai.org/ocs/index.php/AAAI/AAAI17/paper/download/14188/14303) [[code]](https://github.com/jiayi-ma?tab=repositories)
- [LPM] Locality Preserving Matching, IJCAI'2017 [[pdf]](https://www.ijcai.org/proceedings/2017/0627.pdf) IJCV'2019 [[pdf]](https://link.springer.com/article/10.1007/s11263-018-1117-z)  [[code]](https://github.com/jiayi-ma?tab=repositories)
- [DARE] Density adaptive point set registration, CVPR'2018 [[pdf]](https://arxiv.org/pdf/1804.01495.pdf) [[code]](https://github.com/felja633/DARE)
- [GC-RANSAC] Graph-Cut RANSAC, CVPR'2018 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Barath_Graph-Cut_RANSAC_CVPR_2018_paper.pdf) [[code]](https://github.com/danini/graph-cut-ransac)
- [Ppfnet] Ppfnet: Global context aware local features for robust 3d point matching, CVPR'2018 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2018/html/Deng_PPFNet_Global_Context_CVPR_2018_paper.html)
- [3D-CODED] 3D-CODED: 3D correspondences by deep deformation, ECCV'2018 [[pdf]](http://openaccess.thecvf.com/content_ECCV_2018/papers/Thibault_Groueix_Shape_correspondences_from_ECCV_2018_paper.pdf) [[project]](http://imagine.enpc.fr/~groueixt/3D-CODED/) [[code]](https://github.com/ThibaultGROUEIX/3D-CODED)
- [GPCReg-TS] Efficient global point cloud registration by matching rotation invariant features through translation search, ECCV'2018 [[pdf]](http://openaccess.thecvf.com/content_ECCV_2018/html/Yinlong_Liu_Efficient_Global_Point_ECCV_2018_paper.html)
- [N3Net] Neural Nearest Neighbors Networks, NeurIPS'2018 [[pdf]](https://arxiv.org/pdf/1810.12575) [[code]](https://github.com/visinf/n3net)
- [3DFeat-NET] 3dfeat-net: Weakly supervised local 3d features for point cloud registration, ECCV'2018 [[pdf]](https://arxiv.org/pdf/1807.09413) [[code]](https://github.com/yewzijian/3DFeatNet)
- [MVDesc-RMBP] Learning and Matching Multi-View Descriptors for Registration of Point Clouds, ECCV'2018 [[pdf]](http://openaccess.thecvf.com/content_ECCV_2018/papers/Lei_Zhou_Learning_and_Matching_ECCV_2018_paper.pdf)
- [HGMR] HGMR: Hierarchical Gaussian Mixtures forAdaptive 3D Registration, ECCV'2018 [[pdf]](http://openaccess.thecvf.com/content_ECCV_2018/papers/Benjamin_Eckart_Fast_and_Accurate_ECCV_2018_paper.pdf) 
- [GMM-Tree] Fast and Accurate Point Cloud Registration using Trees of Gaussian Mixtures, arxiv'2018 [[pdf]](https://arxiv.org/abs/1807.02587) [[code]](https://github.com/neka-nat/probreg)
- [SWS] Nonrigid Points Alignment with Soft-weighted Selection, IJCAI'2018 [[pdf]](https://www.ijcai.org/proceedings/2018/0111.pdf)
- [DLD] Dependent landmark drift: robust point set registration with a Gaussian mixture model and a statistical shape model, arxiv'2018 [[pdf]](https://arxiv.org/pdf/1711.06588) [[code]](https://github.com/ohirose/dld)
- [DeepMapping] DeepMapping: Unsupervised Map Estimation From Multiple Point Clouds, arxiv'2018 [[pdf]](https://arxiv.org/pdf/1811.11397) [[project]](https://ai4ce.github.io/DeepMapping/)
- [APSR] Adversarial point set registration, arxiv'2018 [[pdf]](https://arxiv.org/abs/1811.08139)
- [3DIV] Fast and Globally Optimal Rigid Registration of 3D Point Sets by Transformation Decomposition, arxiv'2018 [[pdf]](https://arxiv.org/pdf/1812.11307)
- [Analysis] Analysis of Robust Functions for Registration Algorithms, arxiv'2018 [[pdf]](https://arxiv.org/pdf/1810.01474)
- [MVCNN] Learning Local Shape Descriptors from Part Correspondences with Multiview Convolutional Networks, TOG'2018 [[pdf]](https://arxiv.org/pdf/1706.04496) [[project]](https://people.cs.umass.edu/~hbhuang/local_mvcnn/)
- [CSCIF] Cubature Split Covariance Intersection Filter-Based Point Set Registration, TIP'2018 [[pdf]](https://ieeexplore.ieee.org/abstract/document/8332952/)
- [FPR] Efficient Registration of High-Resolution Feature Enhanced Point Clouds, TPAMI'2018 [[pdf]](https://ieeexplore.ieee.org/abstract/document/8352814/)
- [DFMM-GLSP] Non-rigid point set registration using dual-feature finite mixture model and global-local structural preservation, PR'2018 [[pdf]](https://www.researchgate.net/profile/Yang_Yang634/publication/323843423_Non-rigid_point_set_registration_using_dual-feature_finite_mixture_model_and_global-local_structural_preservation/links/5abda92545851584fa6fc44a/Non-rigid-point-set-registration-using-dual-feature-finite-mixture-model-and-global-local-structural-preservation.pdf)
- [PR-Net] Non-Rigid Point Set Registration Networks, arxiv'2019 [[pdf]](https://arxiv.org/pdf/1904.01428) [[code]](https://github.com/Lingjing324/PR-Net)
- [3DRegNet] 3DRegNet: A Deep Neural Network for 3D Point Registration, arxiv'2019 [[pdf]](https://arxiv.org/pdf/1904.01701.pdf)
- [RPM-MR] Nonrigid Point Set Registration with Robust Transformation Learning under Manifold Regularization, TNNLS'2019 [[pdf]](https://pdfs.semanticscholar.org/e8c9/75165ffc5af6cad6961b25f29ea112ae50dd.pdf) [[code]](https://github.com/jiayi-ma?tab=repositories)
- [FGMM] Feature-guided Gaussian mixture model for image matching, PR'2019 [[pdf]](https://www.sciencedirect.com/science/article/pii/S0031320319301414)
- [LSR-CFP] Least-squares registration of point sets over SE (d) using closed-form projections, CVIU'2019 [[pdf]](https://arxiv.org/pdf/1904.04218)
- [TEASER] Teaser: Fast and certifiable point cloud registration, T-Robotics'2020 [[pdf]](https://arxiv.org/pdf/2001.07715.pdf) [[code]](https://github.com/MIT-SPARK/TEASER-plusplus)
- [FPR] Efficient Registration of High-Resolution Feature Enhanced Point Clouds, TPAMI'2019 [[pdf]](https://ieeexplore.ieee.org/abstract/document/8352814/)
- [DCP] Deep Closest Point: Learning Representations for Point Cloud Registration, arxiv'2019 [[pdf]](https://arxiv.org/pdf/1905.03304.pdf) [[code]](https://github.com/WangYueFt/dcp)
- [DeepICP] DeepICP: An End-to-End Deep Neural Network for 3D Point Cloud Registration, arxiv'2019 [[pdf]](https://arxiv.org/pdf/1905.04153)
- [RelativeNet] 3D Local Features for Direct Pairwise Registration, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Deng_3D_Local_Features_for_Direct_Pairwise_Registration_CVPR_2019_paper.pdf) 
- [aff+vSVF] Networks for Joint Affine and Non-Parametric Image Registration, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Shen_Networks_for_Joint_Affine_and_Non-Parametric_Image_Registration_CVPR_2019_paper.pdf)
- [localReg+vSVF] Metric Learning for Image Registration, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Niethammer_Metric_Learning_for_Image_Registration_CVPR_2019_paper.pdf) [[code]](https://github.com/uncbiag/registration)
- [PointNetLK] PointNetLK: Robust & Efficient Point Cloud Registration using PointNet, CVPR'2019 [[pdf]](https://arxiv.org/pdf/1903.05711) [[code]](https://github.com/hmgoforth/PointNetLK)
- [SDRSAC] SDRSAC: Semidefinite-Based Randomized Approach for Robust Point Cloud Registration without Correspondences, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Le_SDRSAC_Semidefinite-Based_Randomized_Approach_for_Robust_Point_Cloud_Registration_Without_CVPR_2019_paper.pdf) [[code]](https://github.com/intellhave/SDRSAC)
- [FilterReg] FilterReg: Robust and Efficient Probabilistic Point-Set Registration using Gaussian Filter and Twist Parameterization, CVPR'2019 [[pdf]](https://arxiv.org/pdf/1811.10136) [[project]](https://sites.google.com/view/filterreg/home) [[code]](https://bitbucket.org/gaowei19951004/poser/src/master/) [[code]](https://github.com/neka-nat/probreg/blob/)
- [POINT2] Multiview 2D/3D Rigid Registration via a Point-Of-Interest Network for Tracking and Triangulation, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Liao_Multiview_2D3D_Rigid_Registration_via_a_Point-Of-Interest_Network_for_Tracking_CVPR_2019_paper.pdf)
- [Geo-CNN] Modeling Local Geometric Structure of 3D Point Clouds using Geo-CNN, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Lan_Modeling_Local_Geometric_Structure_of_3D_Point_Clouds_Using_Geo-CNN_CVPR_2019_paper.pdf)
- [GFrames] GFrames: Gradient-Based Local Reference Framefor 3D Shape Matching, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Melzi_GFrames_Gradient-Based_Local_Reference_Frame_for_3D_Shape_Matching_CVPR_2019_paper.pdf)
- [3DSmoothNet] The Perfect Match: 3D Point Cloud Matching with Smoothed Densities, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Gojcic_The_Perfect_Match_3D_Point_Cloud_Matching_With_Smoothed_Densities_CVPR_2019_paper.pdf) [[code]](https://github.com/zgojcic/3DSmoothNet)
- [LPS] A Robust Local Spectral Descriptor for Matching Non-Rigid Shapes with Incompatible Shape Structures, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Wang_A_Robust_Local_Spectral_Descriptor_for_Matching_Non-Rigid_Shapes_With_CVPR_2019_paper.pdf)
- [RF-Net] RF-Net: An End-to-End Image Matching Network based on Receptive Field, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Shen_RF-Net_An_End-To-End_Image_Matching_Network_Based_on_Receptive_Field_CVPR_2019_paper.pdf)
- [QATM] QATM: Quality-Aware Template Matching For Deep Learning, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Cheng_QATM_Quality-Aware_Template_Matching_for_Deep_Learning_CVPR_2019_paper.pdf) [[code]](https://github.com/cplusx/QATM)
- [VBPSR] Robust Variational Bayesian Point Set Registration, ICCV'2019 [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhou_Robust_Variational_Bayesian_Point_Set_Registration_ICCV_2019_paper.pdf)
- [BCPD] A Bayesian Formulation of Coherent Point Drift, TPAMI'2020 [[pdf]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8985307) [[code]](https://github.com/ohirose/bcpd)
- [StickyPillars] StickyPillars: Robust feature matching on point clouds using Graph Neural Networks, arXiv'2020 [[pdf]](https://arxiv.org/pdf/2002.03983)
- [Pointpwc-net] Pointpwc-net: Cost volume on point clouds for (self-) supervised scene flow estimation, ECCV'2020 [[code](https://github.com/DylanWusee/PointPWC)]
- [DGR] Deep Global Registration, CVPR'2020 [[code](https://github.com/chrischoy/DeepGlobalRegistration)]
- [LearningMultiview] Learning multiview 3D point cloud registration, CVPR'2020 [[code](https://github.com/zgojcic/3D_multiview_reg)]
- [CG-SAC] Compatibility-Guided Sampling Consensus for 3-D Point Cloud Registration, TGRS'2020 
- [RPM-Net] RPM-Net: Robust Point Matching using Learned Features, CVPR'2020 [[code]](https://github.com/yewzijian/RPMNet)
- [SpinNet] SpinNet: Learning a General Surface Descriptor for 3D Point Cloud Registration, CVPR'2021 [[code]](https://github.com/QingyongHu/SpinNet)
- [PointDSC] PointDSC: Robust Point Cloud Registration using Deep Spatial Consistency, CVPR'2021 [[code]](https://github.com/XuyangBai/PointDSC/)
- [ReAgent] ReAgent: Point Cloud Registration using Imitation and Reinforcement Learning, CVPR'2021 [[code]](https://github.com/dornik/reagent)
- [RGM] Robust Point Cloud Registration Framework Based on Deep Graph Matching, CVPR'2021 [[code]](https://github.com/fukexue/RGM)
- [PREDATOR] PREDATOR: Registration of 3D Point Clouds with Low Overlap, CVPR'2021 [[code]](https://github.com/overlappredator/OverlapPredator)
- [COTR] COTR: Correspondence Transformer for Matching Across Images, ICCV'2021 [[code]](https://github.com/ubc-vision/COTR)
- [DFM] DFM: A Performance Baseline for Deep Feature Matching, CVPR'2021 [[code]](https://github.com/ufukefe/DFM)
- [FastRobustICP] Fast and Robust Iterative Closest Point, TPAMI'2021 [[code](https://github.com/yaoyx689/Fast-Robust-ICP)]
- [GeoTransformer] Geometric Transformer for Fast and Robust Point Cloud Registration, CVPR'2022 [[code]](https://github.com/qinzheng93/GeoTransformer)
- [CFI2P] CFI2P: Coarse-to-Fine Cross-Modal Correspondence Learning for Image-to-Point Cloud Registration, arxiv'2023
- [GraphSCNet] Deep Graph-based Spatial Consistency for Robust Non-rigid Point Cloud Registration, CVPR'2023 [[code]](https://github.com/qinzheng93/GraphSCNet)



<a name="mrm"></a>
### Feature Matching/Mismatch Removing/Correspondence Learning/Pruning

- [RANSAC] Random sample consensus: a paradigm for model fitting with applications to image analysis and automated cartography, 1981 [[pdf]](https://apps.dtic.mil/dtic/tr/fulltext/u2/a460585.pdf) [[wiki]](https://en.wikipedia.org/wiki/Random_sample_consensus)
- [MLESAC] MLESAC: A new robust estimator with application to estimating image geometry, CVIU'2000 [[pdf]](http://www.academia.edu/download/3436793/torr_mlesac.pdf) [[code_pcl]](https://github.com/PointCloudLibrary/pcl/tree/master/sample_consensus/include/pcl/sample_consensus)
- [PROSAC] Matching with PROSAC-progressive sample consensus, CVPR'2005 [[pdf]](https://dspace.cvut.cz/bitstream/handle/10467/9496/2005-Matching-with-PROSAC-progressive-sample-consensus.pdf?sequence=1) [[code_pcl]](https://github.com/PointCloudLibrary/pcl/tree/master/sample_consensus/include/pcl/sample_consensus)
- [ICF/SVR] Rejecting mismatches by correspondence function, IJCV'2010 [[pdf]](http://www.nlpr.ia.ac.cn/2010papers/kz/gk24.pdf)
- [GS] Common visual pattern discovery via spatially coherent correspondences, CVPR'2010 [[pdf]](http://www.jdl.ac.cn/project/faceId/paperreading/Paper/Common%20Visual%20Pattern%20Discovery%20via%20Spatially%20Coherent%20Correspondences.pdf) [[code]](https://sites.google.com/site/lhrbss/home/papers/SimplifiedCode.zip?attredirects=0)
- [KC-CE] A novel kernel correlation model with the correspondence estimation, JMIV'2011 [[pdf]](https://www.researchgate.net/profile/P_Chen2/publication/225191068_A_Novel_Kernel_Correlation_Model_with_the_Correspondence_Estimation/links/02e7e5232cd89055ab000000/A-Novel-Kernel-Correlation-Model-with-the-Correspondence-Estimation.pdf) [[code]](http://web.nchu.edu.tw/~pengwen/WWW/Code.html)
- [VFC] A robust method for vector field learning with application to mismatch removing, CVPR'2011 [[pdf]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.721.5913&rep=rep1&type=pdf) [[code]](https://github.com/jiayi-ma?tab=repositories)
- [DefRANSAC] In defence of RANSAC for outlier rejection in deformable registration, ECCV'2012 [[pdf]](https://media.adelaide.edu.au/acvt/Publications/2012/2012-In%20Defence%20of%20RANSAC%20for%20Outlier%20Rejection%20in%20Deformable%20Registration.pdf) [[code]](https://cs.adelaide.edu.au/~tjchin/lib/exe/fetch.php?media=code:eccv12code.zip)
- [CM] Robust Non-parametric Data Fitting for Correspondence Modeling, ICCV'2013 [[pdf]](https://mmcheng.net/mftp/Papers/DataFittingICCV13.pdf) [[code]](https://sites.google.com/site/laoszefei81/home/code-1/code-curve-fitting)
- [AGMM] Asymmetrical Gauss Mixture Models for Point Sets Matching, CVPR'2014 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2014/papers/Tao_Asymmetrical_Gauss_Mixture_2014_CVPR_paper.pdf)
- [TC] Epipolar geometry estimation for wide baseline stereo by Clustering Pairing Consensus, PRL'2014 [[pdf]](http://or.nsfc.gov.cn/bitstream/00001903-5/96605/1/1000007190373.pdf)
- [BF] Bilateral Functions for Global Motion Modeling, ECCV'2014 [[pdf]](http://mftp.mmcheng.net/Papers/CoherentModelingS.pdf) [[project]](https://mmcheng.net/bfun/) [[code]](http://mftp.mmcheng.net/Data/eccv_2014_release.zip)
- [WxBS] WxBS: Wide Baseline Stereo Generalizations, BMVC'2015 [[pdf]](https://arxiv.org/pdf/1504.06603) [[project]](http://cmp.felk.cvut.cz/wbs/)
- [RepMatch] RepMatch: Robust Feature Matching and Posefor Reconstructing Modern Cities, ECCV'2016 [[pdf]](http://www.kind-of-works.com/papers/eccv_2016_repmatch.pdf) [[project]](http://www.kind-of-works.com/RepMatch.html) [[code]](http://www.kind-of-works.com/code/repmatch_code_bf_small.zip)
- [SIM] The shape interaction matrix-based affine invariant mismatch removal for partial-duplicate image search, TIP'2017 [[pdf]](http://www.cis.pku.edu.cn/faculty/vision/zlin/Publications/2017-TIP-SIM.pdf) [[code]](https://github.com/lylinyang/demo_SIM)
- [DSAC] DSAC: differentiable RANSAC for camera localization, CVPR'2017 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2017/papers/Brachmann_DSAC_-_Differentiable_CVPR_2017_paper.pdf) [[code]](https://github.com/cvlab-dresden/DSAC)
- [GMS] GMS: Grid-based Motion Statistics for Fast, Ultra-robust Feature Correspondence, CVPR'2017 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2017/papers/Bian_GMS_Grid-based_Motion_CVPR_2017_paper.pdf) [[code]](https://github.com/JiawangBian/GMS-Feature-Matcher)
- [LMI] Consensus Maximization with Linear Matrix Inequality Constraints, CVPR'2017 [[pdf]](https://www.cvg.ethz.ch/research/conmax/paper/PSpeciale2017CVPR.pdf) [[project]](https://www.cvg.ethz.ch/research/conmax/) [[code]](https://www.cvg.ethz.ch/research/conmax/paper/PSpeciale2017CVPR_code_sample.tar.gz)
- [GOPAC] Globally-Optimal Inlier Set Maximisation for Simultaneous Camera Pose and Feature Correspondence, ICCV'2017 [[pdf]](https://drive.google.com/open?id=0BwzhzqTiWNEWTzE3ZW1lNnhBTUE) TPAMI'2018 [[pdf]](https://drive.google.com/open?id=1FV_SFoxVvsspK3uh9lRYsJPUSX0kuI_L) [[code]](https://drive.google.com/open?id=1H7gOQz7CAXSat56OPTgV2lOLUSI4D_vG)
- [LFGC] Learning to Find Good Correspondences, CVPR'2018 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2018/CameraReady/1453.pdf) [[code]](https://github.com/vcg-uvic/learned-correspondence-release)
- [GC-RANSAC] Graph-Cut RANSAC, CVPR'2018 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Barath_Graph-Cut_RANSAC_CVPR_2018_paper.pdf) [[code]](https://github.com/danini/graph-cut-ransac)
- [KCNet] Mining Point Cloud Local Structures by Kernel Correlation and Graph Pooling, CVPR'2018 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Shen_Mining_Point_Cloud_CVPR_2018_paper.pdf) [[code]](http://www.merl.com/research/license#KCNet)
- [SRC] Consensus Maximization for Semantic Region Correspondences, CVPR'2018 [[pdf]](https://www.cvg.ethz.ch/research/secon/paper/PSpeciale2018CVPR.pdf) [[code]](https://www.cvg.ethz.ch/research/secon/paper/PSpeciale2018CVPR_code_sample.zip)
- [CODE] Code: Coherence based decision boundaries for feature correspondence, TPAMI'2018 [[pdf]](https://ora.ox.ac.uk/objects/uuid:0e5a62ab-fb69-472f-a1e1-49d49595db62/download_file?safe_filename=matching.pdf&file_format=application%2Fpdf&type_of_work=Journal+article) [[project]](http://www.kind-of-works.com/CODE_matching.html)
- [DFE] Deep fundamental matrix estimation, ECCV'2018 [[code]](https://github.com/isl-org/DFE)
- [N3Net] Neural Nearest Neighbors Networks, NeurIPS'2018 [[code]](https://github.com/visinf/n3net/)
- [OANet] Learning Two-View Correspondences and Geometry Using Order-Aware Network ICCV'2019 [[code]](https://github.com/zjhthu/OANet)
- [LPM] Locality preserving matching, IJCV'2019 [[pdf]](https://link.springer.com/article/10.1007/s11263-018-1117-z) [[code]](https://github.com/jiayi-ma?tab=repositories)
- [LMR] LMR: Learning A Two-class Classifier for Mismatch Removal, TIP'2019 [[pdf]](https://ieeexplore.ieee.org/abstract/document/8672170/) [[code]](https://github.com/StaRainJ/LMR)
- [PFFM] Progressive Filtering for Feature Matching, ICASSP'2019 [[pdf]](https://ieeexplore.ieee.org/abstract/document/8682372/)
- [NM-Net] NM-Net: Mining Reliable Neighbors for Robust Feature Correspondences, arXiv'2019 [[pdf]](https://arxiv.org/pdf/1904.00320)
- [NG-RANSAC] Neural-Guided RANSAC: Learning Where to Sample Model Hypotheses, ICCV'2019 [[pdf](https://arxiv.org/pdf/1905.04132.pdf)] [[code](https://github.com/vislearn/ngransac)] [[project](https://hci.iwr.uni-heidelberg.de/vislearn/research/neural-guided-ransac/)]
- [MAGSAC] MAGSAC: Marginalizing Sample Consensus, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Barath_MAGSAC_Marginalizing_Sample_Consensus_CVPR_2019_paper.pdf) [[code]](https://github.com/danini/magsac)
- [DLCM] Unsupervised Learning of Consensus Maximization for 3D Vision Problems, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Probst_Unsupervised_Learning_of_Consensus_Maximization_for_3D_Vision_Problems_CVPR_2019_paper.pdf)
- [ACNe] ACNe: Attentive context normalization for robust permutation-equivariant learning, CVPR'2020[[code]](https://github.com/vcg-uvic/acne)
- [SuperGlue] SuperGlue: Learning Feature Matching with Graph Neural Networks, CVPR'2020 [[code]](https://github.com/magicleap/SuperGluePretrainedNetwork)
- [EifficientDeterministicSearch] Efficient Deterministic Search with Robust Loss Functions for Geometric Model Fitting, TPAMI'2021 [[code]](https://github.com/AoxiangFan/EifficientDeterministicSearch)
- [LoFTR] Detector-free local feature matching with transformers, CVPR'2021 [[code]](https://github.com/zju3dv/LoFTR)
- [GLOF] Robust Feature Matching Using Guided Local Outlier Factor, PR'2021 [[pdf](https://www.sciencedirect.com/science/article/pii/S0031320321001734)] [[code](https://github.com/gwang-cv/GLOF)]
- [CAT] Correspondence Attention Transformer: A Context-sensitive Network for Two-view Correspondence Learning, TMM'2022 [[code]](https://github.com/jiayi-ma/CorresAttnTransformer)
- [TransMVSNet] TransMVSNet: Global Context-aware Multi-view Stereo Network with Transformers, CVPR'2022 [[code]](https://github.com/MegviiRobot/TransMVSNet)
- [ConvMatch] ConvMatch: Rethinking Network Design for Two-View Correspondence Learning, AAAI'2023 [[code]](https://github.com/SuhZhang/ConvMatch)
- [LightGlue] LightGlue: Local Feature Matching at Light Speed, arxiv'2023 [[pdf]](https://arxiv.org/pdf/2306.13643.pdf) [[code]](https://github.com/cvg/LightGlue)
- [GlueStick] GlueStick: Robust Image Matching by Sticking Points and Lines Together, ICCV'2023 [[pdf]](https://arxiv.org/pdf/2304.02008.pdf) [[code]](https://github.com/cvg/GlueStick)
- [DKM] DKM: Dense Kernelized Feature Matching for Geometry Estimation, CVPR'2023 [[code]](https://github.com/Parskatt/DKM)
- [ASTR] ASTR: Adaptive Spot-Guided Transformer for Consistent Local Feature Matching, CVPR'2023 [[code]](https://astr2023.github.io/)
- [IMP] IMP: Iterative Matching and Pose Estimation with Adaptive Pooling, CVPR'2023 [[code]](https://github.com/feixue94/imp-release)
- [PATS] PATS: Patch Area Transportation with Subdivision for Local Feature Matching, CVPR'2023 [[code]](https://zju3dv.github.io/pats/)
- [NCMNet] Progressive Neighbor Consistency Mining for Correspondence Pruning, CVPR'2023 [[code]](https://github.com/xinliu29/NCMNet)
- [AdaMatcher] Adaptive Assignment for Geometry Aware Local Feature Matching, CVPR'2023 [[code]](https://github.com/AbyssGaze/AdaMatcher)
- [SEM] Structured Epipolar Matcher for Local Feature Matching, CVPR'2023 [[code]](https://sem2023.github.io/)
- [FSNet] Two-View Geometry Scoring Without Correspondences, CVPR'2023 [[code]](https://github.com/nianticlabs/scoring-without-correspondences)
- [RoMa] RoMa: Robust Dense Feature Matching, CVPR'2024 [[pdf]](https://arxiv.org/abs/2305.15404) [[code]](https://github.com/Parskatt/RoMa)
- [Efficient LoFTR] Efficient LoFTR: Semi-Dense Local Feature Matching with Sparse-Like Speed, CVPR'2024 [[pdf]](https://zju3dv.github.io/efficientloftr/files/EfficientLoFTR.pdf) [[code]](https://github.com/zju3dv/efficientloftr)
- [MESA] MESA: Matching Everything by Segmenting Anything, CVPR'2024 [[pdf]](https://arxiv.org/abs/2401.16741)


<a name="Mismatch Remo"></a>
#### Mismatch Removing
- 123

<a name="gmm"></a>
### Graph Matching Methods

- [SM] A spectral technique for correspondence problems using pairwise constraints, ICCV'2005 [[pdf]](https://kilthub.figshare.com/articles/A_Spectral_Technique_for_Correspondence_Problems_Using_Pairwise_Constraints/6551327/files/12031808.pdf) [[code]](https://sites.google.com/site/graphmatchingmethods/Code_including_Spectral_Matching.zip?attredirects=0)
- [SM-MAP] Efficient MAP approximation for dense energy functions, ICML'2006 [[pdf]](https://kilthub.figshare.com/articles/Efficient_MAP_Approximation_For_Dense_Energy_Functions/6554678/files/12036863.pdf) [[code]](https://sites.google.com/site/graphmatchingmethods/Code_including_IPFP_and_L2QP_for_MAP_Inference.zip?attredirects=0)
- [SMAC] Balanced Graph Matching, NIPS'2006 [[pdf]](http://papers.nips.cc/paper/2960-balanced-graph-matching.pdf) [[code]](http://www.timotheecour.com/software/graph_matching/graph_matching.html)
- [FCGM] Feature correspondence via graph matching: Models and global optimization, ECCV'2008 [[pdf]](https://www.microsoft.com/en-us/research/wp-content/uploads/2008/10/TR-2008-101.pdf)
- [PM] Probabilistic Graph and Hypergraph Matching, CVPR'2008 [[pdf]](https://www.researchgate.net/profile/Amnon_Shashua/publication/221361679_Probabilistic_graph_and_hypergraph_matching/links/55cc5f3008aeca747d6c288d/Probabilistic-graph-and-hypergraph-matching.pdf)
- [IPFP] An Integer Projected Fixed Point Method for Graph Matching and MAP Inference, NIPS'2009 [[pdf]](http://papers.nips.cc/paper/3756-an-integer-projected-fixed-point-method-for-graph-matching-and-map-inference.pdf) [[code]](https://sites.google.com/site/graphmatchingmethods/Code_including_IPFP.zip?attredirects=0)
- [RRWM] Reweighted Random Walks for Graph Matching, ECCV'2010 [[pdf]](https://link.springer.com/chapter/10.1007/978-3-642-15555-0_36)
- [FGM] Factorized graph matching, CVPR'2012 [[pdf]](https://kilthub.figshare.com/articles/Factorized_Graph_Matching/6554858/files/12037043.pdf) [[code]](http://www.f-zhou.com/gm_code.html)
- [DGM] Deformable Graph Matching, CVPR'2013 [[pdf]](https://www.cv-foundation.org/openaccess/content_cvpr_2013/papers/Zhou_Deformable_Graph_Matching_2013_CVPR_paper.pdf) [[code]](https://github.com/zhfe99/fgm)
- [MS] Progressive mode-seeking on graphs for sparse feature matching, ECCV'2014 [[pdf]](http://ro.uow.edu.au/cgi/viewcontent.cgi?article=5118&context=eispapers) [[code]](https://download.csdn.net/download/family0823/9366365?fps=1&locationNum=1)
- [MGM] A convex relaxation for multi-graph matching, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Swoboda_A_Convex_Relaxation_for_Multi-Graph_Matching_CVPR_2019_paper.pdf)


<a name="misc1"></a>
### Misc

- [ASIFT] ASIFT: An Algorithm for Fully Affine Invariant Comparison, IPOL'2011 [[pdf]](http://www.ipol.im/pub/art/2011/my-asift/article.pdf) [[project]](http://www.cmap.polytechnique.fr/~yu/research/ASIFT/demo.html#SIFT%20and%20ASIFT%20---%20online%20demo%20:%20try%20if%20your%20images%20match!) [[online demo]](http://demo.ipol.im/demo/my_affine_sift/)
- [RootSIFT] Three things everyone should know to improve object retrieval, CVPR'2012 [[pdf]](http://www.cs.sfu.ca/CourseCentral/820/li/material/source/papers/3things-retrieval-2012.pdf) [[related code]](https://www.pyimagesearch.com/2015/04/13/implementing-rootsift-in-python-and-opencv/#)
- [DM-CNN] Descriptor Matching with Convolutional Neural Networks: a Comparison to SIFT, arXiv'2014 [[pdf]](https://www.researchgate.net/profile/Alexey_Dosovitskiy/publication/262568634_Descriptor_Matching_with_Convolutional_Neural_Networks_a_Comparison_to_SIFT/links/541fe8dc0cf2218008d41617.pdf)
- [DASC] DASC: Robust Dense Descriptor for Multi-modal and Multi-spectral Correspondence Estimation, TPAMI'2017 [[pdf]](https://arxiv.org/pdf/1604.07944) [[project]](http://diml.yonsei.ac.kr/~srkim/DASC/)
- [MODS] MODS: Fast and Robust Method for Two-View Matching, CVIU'2015 [[pdf]](https://arxiv.org/pdf/1503.02619) [[project]](http://cmp.felk.cvut.cz/wbs/) [[code]](https://github.com/ducha-aiki/mods)
- [Elastic2D3D] Efficient Globally Optimal 2D-to-3D Deformable Shape Matching, CVPR'2016 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2016/papers/Lahner_Efficient_Globally_Optimal_CVPR_2016_paper.pdf) [[project]](https://vision.in.tum.de/~laehner/Elastic2D3D/)
- [TCDCN] Facial Landmark Detection by Deep Multi-task Learning, ECCV'2014 [[pdf]](http://home.ie.cuhk.edu.hk/~ccloy/files/eccv_2014_deepfacealign.pdf) [[project]](http://mmlab.ie.cuhk.edu.hk/projects/TCDCN.html)
- [LAI] Object matching using a locally affine invariant and linear programming techniques, TPAMI'2013 [[pdf]](https://ieeexplore.ieee.org/abstract/document/6189359/)
- [HPatches] HPatches: A benchmark and evaluation of handcrafted and learned local descriptors, CVPR'2017 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2017/html/Balntas_HPatches_A_Benchmark_CVPR_2017_paper.html)
- [GeoDesc] GeoDesc: Learning Local Descriptors by Integrating Geometry Constraints, ECCV'2018 [[pdf]](http://openaccess.thecvf.com/content_ECCV_2018/papers/Zixin_Luo_Learning_Local_Descriptors_ECCV_2018_paper.pdf) [[code]](https://github.com/lzx551402/geodesc)
- [MIRROR] Matchable Image Retrieval by Learning from Surface Reconstruction ACCV'2018 [[pdf]](http://arxiv.org/abs/1811.10343) [[code]](https://github.com/hlzz/mirror)
- [NDDR-CNN] NDDR-CNN: Layerwise Feature Fusing in Multi-Task CNNsby Neural Discriminative Dimensionality Reduction, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Gao_NDDR-CNN_Layerwise_Feature_Fusing_in_Multi-Task_CNNs_by_Neural_Discriminative_CVPR_2019_paper.pdf) [[code]](https://github.com/ethanygao/NDDR-CNN)
- [ContextDesc] ContextDesc: Local Descriptor Augmentation with Cross-Modality Context, CVPR'2019 [[pdf]](https://arxiv.org/abs/1904.04084) [[code]](https://github.com/lzx551402/contextdesc)
- [Evaluation] An Evaluation of Feature Matchers forFundamental Matrix Estimation, BMVC'2019 [[pdf]](https://jwbian.net/Papers/FM_BMVC19.pdf)

<a name="df"></a>
### Deep Features
- [TFeat] Learning local feature descriptors with triplets and shallow convolutional neural networks, BMVC'2016 [[pdf]](https://www.researchgate.net/profile/Krystian_Mikolajczyk/publication/317192886_Learning_local_feature_descriptors_with_triplets_and_shallow_convolutional_neural_networks/links/5a038dad0f7e9beb1770c3c2/Learning-local-feature-descriptors-with-triplets-and-shallow-convolutional-neural-networks.pdf) [[code]](https://github.com/vbalnt/tfeat)
- [L2-Net] L2-Net: Deep Learning of Discriminative Patch Descriptor in Euclidean Space, CVPR'2017 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2017/papers/Tian_L2-Net_Deep_Learning_CVPR_2017_paper.pdf) [[code]](https://github.com/yuruntian/L2-Net)
- [HardNet] Working hard to know your neighbor's margins: Local descriptor learning loss, CVPR'2018 [[pdf]](http://papers.nips.cc/paper/7068-working-hard-to-know-your-neighbors-margins-local-descriptor-learning-loss.pdf) [[code]](https://github.com/DagnyT/hardnet/tree/master)
- [AffNet] Repeatability Is Not Enough: Learning Discriminative Affine Regions via Discriminability, ECCV'2018 [[pdf]](http://openaccess.thecvf.com/content_ECCV_2018/papers/Dmytro_Mishkin_Repeatability_Is_Not_ECCV_2018_paper.pdf) [[code]](https://github.com/ducha-aiki/affnet)
- [GCNv2] GCNv2: Efficient Correspondence Prediction for Real-Time SLAM, ICLR'2019 [[pdf]](https://arxiv.org/pdf/1902.11046.pdf) [[code]](https://github.com/jiexiong2016/GCNv2_SLAM)
- [D2-Net] D2-Net: A Trainable CNN for Joint Detection and Description of Local Features, CVPR'2019 [[pdf]](https://dsmn.ml/files/d2-net/d2-net.pdf) [[project]](https://dsmn.ml/publications/d2-net.html) [[code]](https://github.com/mihaidusmanu/d2-net)
- [SDC] Stacked Dilated Convolution: A Unified Descriptor Network for Dense Matching Tasks, CVPR'2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Schuster_SDC_-_Stacked_Dilated_Convolution_A_Unified_Descriptor_Network_for_CVPR_2019_paper.pdf)
- [GIFT] GIFT: Learning transformation-invariant dense visual descriptors via group cnns, NeurIPS'2019 [[code]](https://github.com/zju3dv/GIFT)
- [DISK] DISK: Learning local features with policy gradient, NeurIPS'2020 [[code]](https://github.com/cvlab-epfl/disk)
- [ASLFeat] ASLFeat: Learning Local Features of Accurate Shape and Localization, CVPR'2020 [[code]](https://github.com/lzx551402/aslfeat)
- [DualRC-Net] Dual-Resolution Correspondence Networks, NeurIPS'2020 [[code]](https://github.com/ActiveVisionLab/DualRC-Net)
- [GLU-Net] GLU-Net: Global-local universal network for dense flow and correspondences, CVPR'2020 [[code]](https://github.com/PruneTruong/GLU-Net)
- [GOCor] GOCor: Bringing globally optimized correspondence volumes into your neural network, NeurIPS'2020 [[code]](https://github.com/PruneTruong/GOCor)
- [XResolution] X Resolution Correspondence Networks, arXiv'2020 [[code]](https://xyz-r-d.github.io/xrcnet)
- [Sparse-ncnet] Efficient neighbourhood consensus networks via submanifold sparse convolutions, ECCV'2020 [[code]](https://github.com/ignacio-rocco/sparse-ncnet)
- [CaPS] Learning feature descriptors using camera pose supervision, ECCV'2020 [[code]](https://github.com/qianqianwang68/caps)
- [COTR] COTR: Correspondence Transformer for Matching Across Images, ICCV'2021 [[code]](https://github.com/ubc-vision/COTR)
- [CHM] Convolutional Hough Matching Networks, CVPR'2021 [[code]](https://github.com/juhongm999/chm)
- [Key.Net] Key.Net: Keypoint Detection by Handcrafted and Learned CNN Filters Revisited, TPAMI'2022 [[code]](https://github.com/axelBarroso/Key.Net-Pytorch)
- [DeDoDe] DeDoDe: Detect, Don't Describe -- Describe, Don't Detect for Local Feature Matching, arxiv'2023 [[pdf]](https://arxiv.org/pdf/2308.08479.pdf) [[code]](https://github.com/Parskatt/DeDoDe)
- [DarkFeat] DarkFeat: Noise-Robust Feature Detector and Descriptor for Extremely Low-Light RAW Images, AAAI'2023 [[code]](https://github.com/THU-LYJ-Lab/DarkFeat)
- [RELF] Learning Rotation-Equivariant Features for Visual Correspondence, CVPR'2023 [[code]](http://cvlab.postech.ac.kr/research/RELF/)
  






<a name="app"></a>
## Applications

<a name="rsir"></a>
### Remote Sensing Image Registration
- [GLPM] Guided Locality Preserving Feature Matching for Remote Sensing Image Registration, TGRS'2018 [[pdf]](https://ieeexplore.ieee.org/abstract/document/8340808/)

<a name="rir"></a>
### Retinal Image Registration
- [DB-ICP] The dual-bootstrap iterative closest point algorithm with application to retinal image registration, TMI'2003 [[pdf]](http://www.cs.rpi.edu/~stewart/papers/dual_bootstrap_icp.pdf)
- [GDB-ICP] Registration of Challenging Image Pairs: Initialization, Estimation, and Decision, TPAMI'2007 [[pdf]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.226.2782&rep=rep1&type=pdf) [[project]](http://www.vision.cs.rpi.edu/gdbicp/)     
- [ED-DB-ICP] The edge-driven dual-bootstrap iterative closest point algorithm for registration of multimodal fluorescein angiogram sequence, TMI'2010 [[pdf]](https://ieeexplore.ieee.org/abstract/document/5223602/)

<a name="pir"></a>
### Palmprint Image Registration
- Robust and efficient ridge-based palmprint matching, TPAMI'2012 [[pdf]](https://ieeexplore.ieee.org/abstract/document/6112761/)
- Palmprint image registration using convolutional neural networks and Hough transform, arxiv'2019 [[pdf]](https://arxiv.org/pdf/1904.00579)

<a name="vhn"></a>
### Visual Homing Navigation
- Visual Homing via Guided Locality Preserving Matching, ICRA'2018 [[pdf]](https://ieeexplore.ieee.org/abstract/document/8460935/)

<a name="hi"></a>
### HDR Imaging
- Locally non-rigid registration for mobile HDR photography, CVPRW'2015 [[pdf]](https://www.cv-foundation.org/openaccess/content_cvpr_workshops_2015/W12/papers/Gallo_Locally_Non-Rigid_Registration_2015_CVPR_paper.pdf)

<a name="misc2"></a>
### Misc
- Hand Motion from 3D Point Trajectories and a Smooth Surface Model, ECCV'2004 [[pdf]](https://hal.inria.fr/inria-00262293/document) [[project]](http://www.inrialpes.fr/movi)
- A robust hybrid method for nonrigid image registration, PR'2011 [[pdf]](https://www.sciencedirect.com/science/article/pii/S0031320310004930)
- Aligning Images in the Wild, CVPR'2012 [[pdf]](https://www.comp.nus.edu.sg/~lowkl/publications/aligning_images_cvpr2012.pdf) [[code]](https://sites.google.com/site/laoszefei81/home/code-1/code-for-aligning-images-in-the-wild)
- Robust feature set matching for partial face recognition, CVPR'2013 [[pdf]](http://openaccess.thecvf.com/content_iccv_2013/papers/Weng_Robust_Feature_Set_2013_ICCV_paper.pdf)
- Multi-modal and Multi-spectral Registrationfor Natural Images, ECCV'2014 [[pdf]](http://www.cse.cuhk.edu.hk/~leojia/projects/multimodal/papers/multispectral_registration.pdf) [[project]](http://www.cse.cuhk.edu.hk/~leojia/projects/multimodal/)
- Articulated and Generalized Gaussian KernelCorrelation for Human Pose Estimation, TIP'2016 [[pdf]](https://www.researchgate.net/publication/286510775_Articulated_and_Generalized_Gaussian_Kernel_Correlation_for_Human_Pose_Estimation?enrichId=rgreq-1fc1a14d1ced5b1cefa92e498e22f862-XXX&enrichSource=Y292ZXJQYWdlOzI4NjUxMDc3NTtBUzozMzg0NjEwNTc1MzE5MDRAMTQ1NzcwNjgxMjgwMQ%3D%3D&el=1_x_3&_esc=publicationCoverPdf)
- Infrared and visible image fusion via gradient transfer and total variation minimization, Information Fusion'2016 [[pdf]](https://www.researchgate.net/profile/Chang_Li37/publication/292680729_Infrared_and_visible_image_fusion_via_gradient_transfer_and_total_variation_minimization/links/5a10e6cca6fdccc2d7999da3/Infrared-and-visible-image-fusion-via-gradient-transfer-and-total-variation-minimization.pdf) [[code]](https://github.com/jiayi-ma?tab=repositories)
- [Workshop] [Image Matching: Local Features & Beyond](https://image-matching-workshop.github.io/), CVPR'2021 
- [Challenge] [Image Matching Challenge 2021](https://www.cs.ubc.ca/research/image-matching-challenge/current)

<a name="db"></a>
## Databases

### General databases

- [MegaDepth](https://www.cs.cornell.edu/projects/megadepth/)
- [ScanNet](https://github.com/ScanNet/ScanNet#scannet-data)
- [2D Synthesized Chui-Rangarajan Dataset (deformation, noise, and outliers)](https://www.cise.ufl.edu/~anand/students/chui/research.html)
- [TOSCA](http://tosca.cs.technion.ac.il/book/resources_data.html)
- [Multi-View Stereo Dataset](http://vision.middlebury.edu/mview/data/)
- [Multi-View Stereo for Community Photo Collections](http://grail.cs.washington.edu/projects/mvscpc/)
- [Multi-View Stereo](https://cvlab.epfl.ch/data/data-strechamvs/)
- [VGG Affine Datasets](http://www.robots.ox.ac.uk/~vgg/data/data-aff.html)
- [Multi-view VGG's Dataset](http://www.robots.ox.ac.uk/~vgg/data1.html)
- [Oxford Building Reconstruction](http://www.robots.ox.ac.uk/~vgg/data2.html)
- [IMM Datasets](http://www.imm.dtu.dk/~aam/datasets/datasets.html)
- [MPEG7 CE Shape-1 Part B](http://www.imageprocessingplace.com/downloads_V3/root_downloads/image_databases/MPEG7_CE-Shape-1_Part_B.zip)
- [Leaf Shapes Database](http://www.imageprocessingplace.com/downloads_V3/root_downloads/image_databases/leaf%20shape%20database/leaf_shapes_downloads.htm)
- [CMU House/Hotel Sequence Images](http://vasc.ri.cmu.edu/idb/html/motion/house/index.html)
- [Generated Matching Dataset](https://lmb.informatik.uni-freiburg.de/resources/datasets/genmatch.en.html)
- [Image Sequences](https://lmb.informatik.uni-freiburg.de/resources/datasets/sequences.en.html) 
- [Mythological creatures 2D](http://tosca.cs.technion.ac.il/book/resources_data.html)
- [Tools 2D](http://tosca.cs.technion.ac.il/book/resources_data.html)
- [Human face](http://tosca.cs.technion.ac.il/book/resources_data.html)
- [Cars & Motorbikes](https://drive.google.com/drive/folders/0B7CshFGxfi_5RVoyYzFyMUhuZnM)
- [DIML Multimodal Benchmark](http://diml.yonsei.ac.kr/~srkim/DASC/DIMLmultimodal/)
- [Street View Dataset](http://3drepresentation.stanford.edu/) [[github]](https://github.com/amir32002/3D_Street_View) [[data]](https://console.cloud.google.com/storage/browser/streetview_image_pose_3d)
- [EVD: Extreme View Dataset](http://cmp.felk.cvut.cz/wbs/datasets/EVD.zip) [[EVD_tentatives]](http://cmp.felk.cvut.cz/wbs/datasets/EVD_tentatives.zip) [[EZD]](http://cmp.felk.cvut.cz/wbs/datasets/ExtremeZoomDataset.zip)
- [WxBS: Wide Baseline Dataset](http://cmp.felk.cvut.cz/wbs/datasets/WxBS-dataset.zip) [[W1BS]](http://cmp.felk.cvut.cz/wbs/datasets/W1BS.tar.gz)
- [Stanford 3D Scanning](http://graphics.stanford.edu/data/3Dscanrep/)
- [MPI FAUST Dataset](http://faust.is.tue.mpg.de/)
- [Mikolajczyk Database](http://lear.inrialpes.fr/people/mikolajczyk/Database/index.html)
- [Panoramic Image Database](http://www.ti.uni-bielefeld.de/html/research/avardy/index.html)
- [PS-Dataset (A Large Dataset for improving Patch Matching, PhotoSynth Dataset for improving local patch Descriptors)](https://github.com/rmitra/PS-Dataset)
- [Two-view Geometry](http://cmp.felk.cvut.cz/data/geometry2view/index.xhtml)
- [Point clouds data sets for 3D registration](https://projet.liris.cnrs.fr/pcr/)
- [IMW CVPR 2019: Challenge](https://image-matching-workshop.github.io/challenge/)
- [Robotic 3D Scan Repository](http://kos.informatik.uni-osnabrueck.de/3Dscans/)
- [Database for 3D surface registration](http://staffhome.ecm.uwa.edu.au/~00053650/3Dmodeling.html)
- [Large Geometric Models Archive](https://www.cc.gatech.edu/projects/large_models/)
- [Laser scanner point clouds](http://www.prs.igp.ethz.ch/research/completed_projects/automatic_registration_of_point_clouds.html)

### Other databases

- [FIRE: Fundus Image Registration Dataset](https://www.ics.forth.gr/cvrl/fire/)
- [DRIVE (Retinal Images)](http://www.isi.uu.nl/Research/Databases/DRIVE/)
- [DRIONS-DB (Retinal Images)](http://www.ia.uned.es/~ejcarmona/DRIONS-DB.html)
- [STARE (Retinal Images)](http://cecas.clemson.edu/~ahoover/stare/)
- [Plant Images](https://www.plant-phenotyping.org/datasets-download)
- [MR Prostate Images](https://bigr-xnat.erasmusmc.nl/)
- [CV Images](http://www.cs.cmu.edu/afs/cs/project/cil/www/v-images.html)
- [ETHZ Datasets](http://www.vision.ee.ethz.ch/en/datasets/)
- [CVPapers](http://www.cvpapers.com/datasets.html)
- [YACVID](https://riemenschneider.hayko.at/vision/dataset)
- [Intelligent remote sensing data analyis](http://mplab.sztaki.hu/remotesensing/index.html)

<a name="tools"></a>
## Tools

- [VLFeat](http://www.vlfeat.org/)
- [PCL: Point Cloud Library](https://github.com/PointCloudLibrary/pcl)
- [Pointmatcher: a modular library implementing the ICP algorithm for aligning point clouds](https://github.com/ethz-asl/libpointmatcher)
- [Open3D: A Modern Library for 3D Data Processing](http://www.open3d.org/docs/index.html)
- [3D keypoints (MeshDOG) and local descriptors (MeshHOG)](http://mvviewer.gforge.inria.fr/)
- [COLMAP](https://colmap.github.io/)
- [OpenMVG: open Multiple View Geometry](https://github.com/openMVG/openMVG)
- [VisualSFM : A Visual Structure from Motion System](http://ccwu.me/vsfm/)
- [Medical Image Registration Toolbox](https://sites.google.com/site/myronenko/research/mirt)
- [Graph Matching Toolbox in MATLAB](http://www.timotheecour.com/software/graph_matching/graph_matching.html) 
- [FAIR: Flexible Algorithms for Image Registration](https://github.com/C4IR/FAIR.m) [[pdf]](http://www.siam.org/books/fa06/Modersitzki_FAIR_2009_FA06.pdf)
- [Range Image Registration Toolbox](http://eia.udg.es/~cmatabos/research.htm)
- [Image Matching WebUI find matches between 2 images](https://github.com/Vincentqyw/image-matching-webui)
- [hloc - the hierarchical localization toolbox](https://github.com/cvg/Hierarchical-Localization) 
