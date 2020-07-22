---
# Display name
title: Online Judge System

# Username (this should match the folder name)
authors:
- x-lab

# Is this the primary user of the site?
superuser: true

# Role/position
role: 技术传播文明，践行同步世界

# Organizations/Affiliations
organizations:
- name: East China Normal University
  url: "http://www.ecnu.edu.cn/"

# Short bio (displayed in user profile at end of posts)
bio: 拥抱开源，热爱生活

interests[]:
- Advocating lofty academic feelings and technical feelings!
- Encourage highly respected, open and innovative geek culture!
- Rejecting the “sophisticated egoism”!
- Adhering to the “open”, “equal”, ”positive”, ”mutual respect”, “mutual support” culture!
- Stay hungry, stay foolish

education[]:
  courses:
  - course: PhD in Artificial Intelligence
    institution: Stanford University
    year: 2012
  - course: MEng in Artificial Intelligence
    institution: Massachusetts Institute of Technology
    year: 2009
  - course: BSc in Artificial Intelligence
    institution: Massachusetts Institute of Technology
    year: 2008

# Social/Academic Networking
# For available icons, see: https://sourcethemes.com/academic/docs/page-builder/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "#contact" for contact widget.
social:
- icon: envelope
  icon_pack: fas
  link: '#contact'  # For a direct email link, use "mailto:test@example.org".
- icon: twitter
  icon_pack: fab
# link: https://twitter.com/GeorgeCushen
- icon: google-scholar
  icon_pack: ai
# link: https://scholar.google.co.uk/citations?user=sIwtMXoAAAAJ
- icon: github
  icon_pack: fab
  link: https://github.com/X-lab2017
# Link to a PDF of your resume/CV from the About widget.
# To enable, copy your resume/CV to `static/files/cv.pdf` and uncomment the lines below.
# - icon: cv
#   icon_pack: ai
#   link: files/cv.pdf

# Enter email to display Gravatar (if Gravatar enabled in Config)
email: "wwang@dase.ecnu.edu.cn"

# Organizational groups that you belong to (for People widget)
#   Set this to `[]` or comment out if you are not using People widget.
user_groups:
- admin
---

**项目内容**：搭建一个**推荐式在线评测系统**。根据每一个学习者的历史刷题记录以及其学习反馈，个性化地为他们推荐利于他们高效学习的练习题并依据知识点制定一套合适的学习路线。实现一个不仅可以让用户自己寻找合适的题目进行自主学习，而且能为每个用户提供一个精准的个性化在线学习系统。

**用户画像**：我们的目标群体是**C语言初学者**。疫情期间的编程学习，比以往更注重自主的题目练习。目前所使用的在线判题系统存在着题目难度与知识点分布广、错误类型不明确等问题，使得用户在做题过程中遇到题目难度不符合自身情况、遇到未知的知识点、调试困难等问题。我们的用户也是我们自己，因此我们更加深刻的理解用户所面临的困难。

**问题定义**：当前国内高校计算机通识教育课程普及程度高但学生总体的学习体验一般。学生对传统的教授方式不感兴趣，在实训过程中遇到问题后无法及时获得帮助。我们小组经研究认为，使用一套基于“在线裁判”的编程学习系统辅助计算机教育的开展。该系统鼓励学生在已经搭建好的环境中进行自主学习，反馈学习进展，并且能为有困难的学生提供及时的帮助。

**算法设计**：根据我们的调查结果和用户需求分析，我们需要实现题目推荐系统，错误原因分析等功能。为了指导用户入门程序设计并有效提高，我们会使用推荐系统基于用户的历史行为来为用户推荐合适的题目。推荐系统使用的是基于物品的协同过滤算法，首先要根据题目自身的标签和用户完成情况计算出题目标签向量之间的余弦相似度。在用户完成一道题目之后，检查他本次和之前完成的题目为其推荐相似度较高的题目。根据用户提交的程序的运行结果和代码，内置一部分常见的错误原因，并使用神经网络算法进行学习，从而为用户的调试提供指导。

**代码协作**：我们计划与学院的题库进行合作，在已有的题目和用户数据上进行推荐。我们可以借助题库中提供的接口构造新的适合初学者学习的模块。利用<font color='orangered'>*git</font>，<font color='orangered'>*anaconda</font>等工具进行代码的协作编写。

**测试**：我们计划在原型创建后，通过反复迭代优化这个在线判题系统。第一版上线后，第一批使用它的C语言初学者将是和我们一样的在校大学生，而测试场景则是大学生们初入大学校园在计算机公选课上遇到困难的场景。反馈表收集的信息包括用户想到的任何新的点子和A/B测试，比如我们的系统在判断用户答题错误后，应该给出出错的地方还是解决方案，就需要我们在测试迭代和回溯中找准用户偏好。
