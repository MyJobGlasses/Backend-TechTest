# Json2Csv

This repository is part of: [MyJobGlasses](https://www.myjobglasses.com/) - Technical Test

The goal of this test is to write a small Ruby lib aiming to convert JSON files composed of arrays of objects to a flat CSV file where one line equals one object.

## Test instructions

Here is the input schema (GraphQL-like) of what our app is expected to process correctly

```
type Profile {
  id: String!
  email: String!
  tags: [String]
  profiles: [SocialProfile]
}

type SocialProfile {
  id: String!
  picture: String
}

```

Some sample files are located in `./input_json_files` and  `./output_csv_files`. Assume they are user provided files from the internet.

You can start by writing a `main.rb` (feel free to change this name) that will perform the conversion when running `ruby main.rb [input_dir] [output_dir]` of all the files of the input directory into the output dir

## Test rating criteria

- clean
- extensible
- robust (don't overlook edge cases, use exceptions where needed, ...)
- tested

You have no limitation of time, what we expect is to have a discussion about your choices and your code implementation.

To share your code, it's your choice again: send us a zip or a GitHub link!

## Tools & Test debrief

You are free to use whatever tool at your disposal to develop the application, please however indicate which tools have been used in your readme (you do not need to mention your editor and basic plugins like linters).

If the code passes the test, keep in mind that during the test debrief, you'll be asked to alter your program (please come with your laptop and development environment). During the test, internet access is not guaranteed to work at 100%, but otherwise you'll be able to use any resources you can access.

Good luck!
