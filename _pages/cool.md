---
layout: single
title: "The Computational Oceanography Lab at MLML"
permalink: /cool/
author_profile: true
---

In 2023 when I was hired at the Moss Landing Marine Labs, I started up the Computational Oceanography Lab (CoOL). This new lab was formed to supplement the other marine science efforts in the 8 central labs at MLML and the other affiliated labs - you can read more about those on the [MLML Site](https://mlml.sjsu.edu/). On this page, I'll introduce the CoOL group members and what we're all about.


## Who's the CoOL Group?


<style>
.people-card {
  display: flex;
  gap: 24px;
  background: #111111;
  border: 1px solid #1f3b5c;
  border-radius: 18px;
  padding: 24px;
  margin-bottom: 28px;
  align-items: flex-start;
  box-shadow: 0 4px 14px rgba(0,0,0,0.25);
}

.people-card img {
  width: 140px;
  height: 140px;
  border-radius: 50%;
  object-fit: cover;
  border: 3px solid #4da3ff;
  flex-shrink: 0;
}

.people-card-content {
  flex: 1;
}

.people-card-content h3 {
  margin-top: 0;
  margin-bottom: 6px;
  color: #ffffff;
}

.people-role {
  color: #7db8ff;
  font-weight: 600;
  margin-bottom: 14px;
}

.people-interests {
  margin-top: 14px;
  font-size: 0.95em;
}

.people-links a {
  margin-right: 14px;
}

@media (max-width: 700px) {
  .people-card {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }

  .people-card-content {
    width: 100%;
  }
}
</style>

### Graduate Students

<div class="people-card">

<img src="/images/people/brandon.jpg" alt="Brandon Castillo">

<div class="people-card-content">

<div class="people-role">
Brandon Castillo
</div>

Brandon Castillo is a current graduate student in the Computational Oceanography lab. He earned a B.S. in Electrical Engineering and Computer Science from UC Berkeley, focusing on data modeling and machine learning. Brandon is interested in finding ways to use deep learning with numerical modeling to better predict changes in the ocean. At MLML, Brandon plans to study how to implement deep learning with numerical modeling on glacier-sea interactions for accurately predicting changes in sea rise. Outside of work, Brandon likes to backpack, work out, and go cycling.

</div>
</div>

<div class="people-card">

<img src="/images/people/megan.jpg" alt="Megan Sharkey">

<div class="people-card-content">

<div class="people-role">
Megan Sharkey
</div>

Megan Sharkey is a current graduate student in the Computational Oceanography lab. She earned her B.A. in Environmental Studies from Boston College, where she specialized in GIS, environmental justice, and geology. Her passion lies in exploring how marine ecosystems, climate change, and coastal communities are interconnected. At MLML, Megan plans to study the evolving dynamics of the Greenland Ice Sheet using spatial data analysis, remote sensing, and numerical ocean modeling. When she’s not in the lab, she enjoys practicing yoga, hiking, and hanging out at the beach.

</div>
</div>

### Undergraduate Students

<div class="people-card">

<img src="/images/people/sherine.jpeg" alt="Sherine Aldrin">

<div class="people-card-content">

<div class="people-role">
Sherine Aldrin
</div>

Sherine is a fourth-year Data Science major at San José State University. She is passionate about how data can help us better understand our oceans and is spending the summer conducting data analysis and numerical modeling research on the Greenland Ice Sheet. In her free time, she enjoys baking, spending time with her dog, staying active, reading, and being with friends.

</div>
</div>

### Staff

<div class="people-card">

<img src="/images/people/sweet.jpg" alt="Sweet Zhang">

<div class="people-card-content">

<div class="people-role">
Sweet Zhang
</div>

Sweet Zhang is a recent graduate from SJSU’s Computer Science department and a software developer in the CoOL group. She works closely with oceanographers at NASA’s Jet Propulsion Laboratory, writing code to process data from Argo floats and support new ocean model developments. Outside of work, she likes to spend her time in the mountains climbing or snowboarding.

</div>
</div>


## What's Computational Oceanography?

In the years since I've started, I've spread the word about the Computational Oceanography Lab and gotten lots of question about what we do. My favorite question has been: *Isn't all oceanography "computational oceanography"?* I agree a lot with this sentiment! However, the goal of the new group is to provide some new directions for MLML that can also help support existing research efforts.

The focus of the Computational Oceanography Lab is in three central areas:
1. Ocean Modeling

    Numerical ocean models use physical equations of motion to simulate circulation and heat transport. The CoOL group primarily uses the MIT General Circulation Model (MITgcm) for our simulations as well as MITgcm-derived ocean state estimates provided by the Estimating the Circulation and Climate of the Ocean (ECCO) consortium.

2. Remote Sensing

    Remote sensing observations refer to measurements of the ocean from satellite or aircraft. Remote sensing observations use electromagnetic radiation such light from the sun, radio waves emitted by satellites, or even green-light lasers to infer information about processes in the ocean. There are a wide range of variables which can be observed from space including temperature, salinity, chlorophyll concentration, wind speed and direction, sea surface height, shallow water bathymetry and much more. Together, these observations enable us to learn about the entire ocean over years or even decades.

3. Machine Learning

    Like all other fields these days, machine learning algorithms and the hardware that powers them are helping to open up new directions for oceanographic research. In the CoOL group, we're working to explore new ways to apply these techniques to our research for a variety of applications including "seeing through" clouds that obscure satellite retrievals and emulating numerical models for faster ocean simulations.

You can read more about these efforts in both the Research Areas and Teaching sections of this site.