

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

1. What is the difference between an adaptive website and a fully responsive website?
An adaptive website uses breakpoints at certain screen sizes to change the layout, but everything is hard coded and not necessarily fluid. Adaptive combines fluid and adaptive to make a page that seamlessly transitions in all screen sizes using units that scale (like % and rem) as well as media breakpoints.

2. Describe what it means to be mobile first vs desktop first.
A mobile first design will start with a small screen with and use min-width media queries to scale up while desktop first will start with a large design using media query max-width to scale down.

3. What does `font-size: 62.5%` in the `html` tag do for us when using `rem` units?
setting the font-size to 62.5% makes it so the 1 rem equals 10 px and 1.6 rem makes 16 px, which is the default size of most browsers. It's more done for the ease of development.

4. How would you describe preprocessing to someone new to CSS?

Preprocessing is when you take data and filters it through a program before it goes through a compiler. In the case of CSS, we use preprocessing to filter our css data written in a different css language (Like LESS or SASS) which has javascript applied to it and feed it to a compiler so it produces vanilla css that the browser is then able to read.

5. What is your favorite concept in preprocessing? What is the concept that gives you the most trouble?

I like the concepts of mixins and variables, and also just the whole structure because they all come together to make coding a lot less repetitive and efficient. I don't like the idea of parametric mixins too much because if you define too many parametric mixins, you might have to backtrack a lot to remember what you used as a parameter and in what order.

You are expected to be able to answer all these questions. Your responses contribute to your Sprint Challenge grade. Skipping this section *will* prevent you from passing this challenge.

## Project Set Up

Follow these steps to set up your project:

### Git Set up

- [ x] Create a forked copy of this project.
- [ x] Add your project manager as collaborator on Github.
- [ x] Clone your OWN version of the repository (Not Lambda's by mistake!).
- [ x] Create a new branch: git checkout -b `<firstName-lastName>`.
- [ x] Implement the project on your newly created `<firstName-lastName>` branch, committing changes regularly.
- [x ] Push commits: git push origin `<firstName-lastName>`.

Follow these steps for completing your project.

- [ x] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo). **Please don't merge your own pull request**
- [ x] Add your project manager as a reviewer on the pull-request
- [ x] Your project manager will count the project as complete by merging the branch back into master.


### Preprocessor Set up

* [ x] Verify that you have LESS installed correctly by running `lessc -v` in your terminal, if you don't get a version message back, reach out to your project manager for help.
* [ x] Open your terminal and navigate to your preprocessing project by using the `cd` command
* [ x] Once in your project's root folder, run the following command `less-watch-compiler less css index.less`
* [ x] Verify your compiler is working correctly by changing the `background-color` on the `html` selector to `red` in your `index.less` file.
* [ x] Once you see the red screen, you can delete that style and you're ready to start on the next task

## Minimum Viable Product

Your finished project must include all of the following requirements:

### Import LESS Files

* [ x] Navigate to your `index.less` file. Notice the file is blank. You have been asked to use a certain import order. That order is as follows:

```markdown
1.variables.less
2.mixins.less
3.reset.less
4.global.less
5.navigation.less
6.footer.less
7.home-page.less
```

_You will know everything is working properly when you see the styles enabled for the provided content._  

### Home Page - Desktop HTML & LESS

* [x] Take 10 minutes to review the code that has already been provided for you. Take time to see how the home page was built.

* [x ] Add a viewport meta tag to the head of your index.html page

* [x ] [Review the provided home desktop design file](design-files/home-desktop.png). You are to build the missing navigation system and header image. You have been provided all content necessary in the [index.html file](index.html)

* [x ] Navigation Styles: Use the `navigation.less` file for styling.

* [x ] Main Content Styles: Use the `home-page.less` file for styling

* [x ] LESS Mixins: Create and use 2 different mixins to aid your styling. Use the `mixins.less` file for your mixins

* [x ] LESS Parametric Mixin: create a parametric mixin that is used to create the `sign up` button styles.

* [x ]  Use at least 2 parameters to create your button

* [x ] Create a hover state that swaps the background color and font color of the base button styles.

### Mobile Design

* [x ] Create a `@phone` variable that contains a `max-width: 500px` media query string. Use the `@phone` variable for all your nested mobile styling.

* [ x] [Review the provided home mobile design file](design-files/home-mobile.png). Match your mobile styling the best you can using the design file.

* [ x] Push your changes and create a pull request if you haven't already.

In your solution, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Stretch Problems

After finishing your required elements, you can push your work further. These goals may or may not be things you have learned in this module but they build on the material you just studied. Time allowing, stretch your limits and see if you can deliver on the following optional goals:

* [ ] Build a page of your choosing from the navigation items. Come up with content and images that fit the theme.

* [ ] Introduce CSS animations to your site.

* [ ] Create a fixed navigation and add some opacity to the background

* [ ] Create a form that would allow someone to sign up for a Spacewalkers Magazine subscription
