---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "CAPTRA: CAtegory-level Pose Tracking for Rigid and Articulated Objects from Point Clouds"
authors: [He Wang$^*$, "Yijia Weng$^*$", Qiang Zhou, Yuzhe Qin, Yueqi Duan, Qingnan Fan, Baoquan Chen, Hao Su, Leonidas Guibas]
date: "2020-11-17T20:00:00+08:00"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "preprint"
publication_short: "**preprint**"

abstract: "In this work, we tackle the problem of category-level online pose tracking for objects from uncolored point cloud sequences. For the first time, we propose a unified framework that handles both 9DoF rigid object pose tracking and per-part pose tracking for articulated objects and works for novel object instances from known categories. Here the 9DoF pose is composed of 3D size and 6D pose and equivalent to a 3D free amodal bounding box representation. Given the depth point cloud at current frame and the estimated pose from the last frame, our novel end-to-end differentiable pipeline can accurately predict the updated pose. \n\n Our pipeline is composed of three modules: 1) a pose canonicalization module that canonicalizes the pose of input depth point cloud making the following steps easier; 2) a RotationNet directly regresses interframe delta rotations; 3) a CoordinateNet that predicts the normalized coordinates and analytically computes the updated scale and translation. Leveraging the small pose regime in the pose-canonicalized point clouds, our method enables the accurate rotation regression and can avoid the non-differentiable RANSAC step used in coordinate-based voting approach.
Taking the best of both worlds, our method combines the coorindate based voting and direct regression and features an end-to-end 9DoF pose prediction directly optimized for pose accuracy. Our extensive experiments demonstrate that our method achieves a new state-of-the-art performance on both category-level rigid and articulated pose benchmarks while being the fastest category-level pose estimation method with a FPS ~12. "

# Summary. An optional shortened abstract.
summary: "In this work, we tackle the problem of category-level online pose tracking for objects from uncolored point cloud sequences. For the first time, we propose a unified framework that handles both 9DoF rigid object pose tracking and per-part pose tracking for articulated objects and works for novel object instances from known categories. Our pipeline performs a fast, end-to-end pose prediction directly optimized for pose accuracy by combining the strengths of coordinate-based approach and direct regression. Our extensive experiments demonstrate that our method achieves a new state-of-the-art performance on both category-level rigid and articulated pose benchmarks while being the fastest category-level pose estimation method with a FPS ~12."



tags: []
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: 
url_code: 
url_dataset:
url_poster:
url_project: 
url_slides:
url_source:
url_video: 

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: "Smart"
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
