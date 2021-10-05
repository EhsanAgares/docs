---
title: Quickstart
intro: 'Get started using {% data variables.product.product_name %} to manage Git repositories and collaborate with others.'
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
topics:
  - Pull requests
  - Issues
  - Notifications
  - Accounts
children:
  - /set-up-git
  - /create-a-repo
  - /fork-a-repo
  - /github-flow
  - /be-social
  - /communicating-on-github
  - /github-glossary
  - /git-cheatsheet
  - /git-and-github-learning-resources
redirect_from:
  - /github/getting-started-with-github/quickstart/
---
bool isMapVisible = false;

AnimatedOpacity(
  opacity: isMapVisible ? 1.0 : 0,
  duration: Duration(milliseconds: 600),
  child: GoogleMap(
    initialCameraPosition: CameraPosition(
      target: LatLng(
        37.4503622703105, 127.12989966313339),
        zoom: 16,
    ),
    onMapCreated: (GoogleMapController controller) {
      _controller.complete(controller);
      Future.delayed(
          const Duration(milliseconds: 550),
          () => setState(() {isMapVisible = true;}));
    },
))
