# React Native FlatList Crash: Handling Null Items

This repository demonstrates a common error in React Native's FlatList component: crashing when rendering a null or undefined item.  The example shows how to reproduce the error and provides a solution to handle null or undefined items gracefully.

## Problem

The FlatList component in React Native expects each item in the `data` array to have a valid key and structure. If a null or undefined item is present, attempting to access properties of that item will lead to a runtime error and app crash.

## Solution

The provided solution ensures that only valid items are rendered by checking for null or undefined values before accessing properties. This prevents crashes and maintains application stability.  Consider using a more robust keyExtractor to avoid index-related issues.