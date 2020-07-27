---
extends: _layouts.documentation
title: "Overscroll"
description: "Utilities for controlling how the browser handles scrolling past the boundary of the scrolling area."
features:
  responsive: true
  customizable: false
  hover: false
  focus: false
---

@include('_partials.class-table', [
  'rows' => [
    [
      '.overscroll-auto',
      'overscroll-behavior: auto;',
      "Maintain default scrolling behavior.",
    ],
    [
      '.overscroll-contain',
      'overscroll-behavior: contain;',
      "Maintain default scrolling behavior in this element only.",
    ],
    [
      '.overscroll-none',
      'overscroll-behavior: none;',
      "Disable all scroll chaining and prevent default scroll overflow behavior.",
    ],
    [
      '.overscroll-x-auto',
      'overscroll-behavior-x: auto;',
      "Maintain default scrolling behavior on the x-axis.",
    ],
    [
      '.overscroll-x-contain',
      'overscroll-behavior-x: contain;',
      "Maintain default x-axis scrolling behavior in this element only.",
    ],
    [
      '.overscroll-x-none',
      'overscroll-behavior-x: none;',
      "Disable all scroll chaining and prevent default scroll overflow behavior on the y-axis.",
    ],
    [
      '.overscroll-y-auto',
      'overscroll-behavior-y: auto;',
      "Maintain default scrolling behavior on the y-axis.",
    ],
    [
      '.overscroll-y-contain',
      'overscroll-behavior-y: contain;',
      "Maintain default y-axis scrolling behavior in this element only.",
    ],
    [
      '.overscroll-y-none',
      'overscroll-behavior-y: none;',
      "Disable all scroll chaining and prevent default scroll overflow behavior on the y-axis.",
    ],
  ]
])

## Customizing

@include('_partials.variants-and-disabling', [
    'utility' => [
        'name' => 'overscroll',
        'property' => 'overscroll-behavior',
    ],
    'variants' => [
        'responsive',
    ],
])
