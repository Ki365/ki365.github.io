+++
title = "Journey to... Engineering through Collaboration "
date = 2024-07-01
authors = [ {name = "OfficialKris", link = "https://github.com/OfficialKris", image = "https://github.com/OfficialKris.png"} ]
tags = ["Engineering", "Software", "Collaboration"]
excludeSearch = false
draft = true
+++

## The Reason

There is a very real need for collaboration-across disciplines, but in my opinion engineering discipline the most. I come from a background of intense collaboration to achieve seemingly impossible tasks. After completing that project, I have moved to other endevours. This has left me with not too many options in the field of engineering software management.

While there are many open source (or some optionally freeware) software to manage specfic engineering disciplines (electrical, mechanical, etc). There was no great platform for sharing these creations. Of course there was online sharing platforms like GrabCad (and I have used it extensively in the past), there was no platform for AUTHORING data. Where can I just push my engineering documents and be done with it?

In traditional engineering (cars, spacecraft, tanks), engineering documents are pushed to a centralized repository with a dedicated staff performing critical maintence (archives, updates, security). However, I believe there is a segment of the engineering community which wants an easy to use platform for managing their content. But how could this happen?

## The Software

Let me introduce you to some amazing software:

```
git
KiCad
FreeCAD
```

These three pieces of software are the user facing programs in the program called Ki365 (provide link). These softwares make Ki365 worthwhile. I have used KiCad for professional level projects and am blown away by the value provided. FreeCAD, although as of writing this, not yet at version 1.0 (refering to "ready to use in production", although rapidly approaching (hopefully the end of this month) provides an incredible data format openness (in contrast to the rest of the industry). And Git. What more do I have to say? This software is the leader in Version Control Systems (VCS) and underpins the entire software economy.

## What Can be Done?

We can build a next generation engineering collaboration software package. A system not dependendent on one point of failure but truly BUILT TO SCALE (vertically AND horizontally). Look at the following diagram for a better description:

[INSERT DIAGRAM]

This system builds upon giants. Decentralized engineering. The technology stack is incredible, perforant, reliable, and and awesome to use.

The current state of Ki365 includes most of the foundational pieces. However, I will not start accepting any potential PR requests until a v0.0.1 or our Minimal Viable Product (MVP) release. This release will signify a baseline of usability (add a project, view a project, project structure stable).

## The Future

Beyond that, I want to look towards new features:

- Federation (sharing projects via integration of Git/AT Protocol with Ki365)
- Project release (works with git tags)
- FreeCAD support
- Diff merge
- Component storage (part data, footprints, schematics, mechanical components)
- and many more!

However, Ki365 is not there yet. In fact, as of writing this post, I have only just pushed changes moving the eye candy project listing from an internal, fixed, json mapping to a dynamically generated REST API call. That took over 24hrs of work (including going from implementing React promises with toasting support to building the golang API function performing the zipped project files extraction and validation).

## A New Problem

What I am saying is quality, useful, software requires an uncountable amount of man hours to build. Even though I may want to, I can't build it all. So far, this project has one contributor. I want that number to increase so the mission of this project is fulfilled. If anything, let this blog post serve as a call to action.

As of this writing, Ki365 is taking GitHub donations (link). I am pouring into this project because of the open source projects that came before it. If you think this

The following software projects make Ki365 possible:

- [KiCanvas](http://github.com/)
- React
- TailWindCSS
- Golang
- ThreeJS
- GoGit
- and many more to come!
