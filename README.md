# ecse444-lab-0--blinky-blinky-solved
**TO GET THIS SOLUTION VISIT:** [ECSE444 Lab 0- Blinky! Blinky! Solved](https://www.ankitcodinghub.com/product/ecse-444-microprocessors-lab-0-blinky-blinky-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;132117&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ECSE444  Lab 0- Blinky! Blinky! Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
Abstract

In this lab you will confirm that you have installed the STM32Cube toolchain, can successfully configure your B-L475E-IOT01A or B-L4S5I-IOT01A development board, and deploy simple software to it, in this case, making an LED blink.

Deliverables None.

Grading

Not graded.

Changelog

Overview

In this first lab, we will build the canonical “hello world” program of development boards: we’ll make an LED blink on our STMicroelectronics B-L475E-IOT01A (B-L4S5I-IOT01A) Discovery kit for IoT development board.

First things first: there are several elements of the tool chain that must be downloaded and installed. This year, we’re using the STMicroelectronics tool chain, STM32Cube, which works in Windows, Linux, and OS X. For more information about this software ecosystem, go here.

You’ll need the following following hardware before beginning:

● STM development board.

● Micro USB data+charging cable; note, charging-only cables are not adequate.

You’ll need to install the following software before beginning:

● ST-LINK-Server

● STM32CubeIDE

Installation Notes

● The lab computers are running STM32CubeIDE v.1.13.1 this year. You should do the same to make your projects portable.

● You need to install ST-LINK-Server before STM32CubeIDE will be able to communicate with the development board. OS X: it is included as a separate package in the disk image; install it first!

● STM32CubeIDE runs slowly the first time you open it, begin a project, etc; the installation package is over 1 GB, but there are still more files to download! Be patient.

For more information on installation, follow the link for your operating system; common issues and fixes will appear there as they arise.

● Linux

● OS X

● Windows

All of our projects will start with creating a project in STM32CubeIDE and configuring our development board. The purpose of this software is to help us configure our development board: (a) we select our development board, (b) we configure our peripherals, and then the magic happens: (c) the software generates a code template, or skeleton, for us.

We’ll then edit and run this code in STM32CubeIDE. At its core, STM32CubeIDE is an Eclipse-based compilation, deployment, and debugging environment. We first make changes to our software, editing the skeleton previously generated for us, adding new source files, etc.

Then we can deploy the software to our development board and use a debugger to slowly step through the program, check the values of variables, etc. Finally, we can run the software at full speed on our development board once we are satisfied that it is operating correctly.

Our development board comes with a wide variety of peripherals; in this lab, we’ll use a timer to make an LED blink!

Because this is the first lab, it is structured more like a tutorial: we will walk through the steps required for configuration and coding, step by step. In the future, you will be expected to navigate the software more autonomously, with the assistance of the vast resources available to support professionals as they develop software for this platform.

The remainder of this document is organized as follows:

1. Board configuration and Code Generation

2. Writing, Deploying, Debugging, and Running Your Code

3. Additional Exercises

Board Configuration and Code Generation

First, we’ll create a new project for our development board and generate the skeleton code that will initialize its peripherals.

Selecting the Discovery kit for IoT Development Board

Open the software and Create a New STM32 project. This will open the Target Selector.

Note: the first time you do this, STM32CubeIDE will download the target selector database; this can take a while.

Search for your board, e.g., the B-L475E-IOT01A1. Check the bottom of the box it came in to see which you are using.

To make things easier in the future, mark it as a favorite by clicking the star.

Then click Next &gt;, and:

● Name the project,

● Select “C” as the target language,

● Select “Executable” as the targeted binary type, then click Finish.

Note: the first time you do this, STM32CubeIDE will download all the support software for the target you’ve selected; this can take a while.

You will be prompted: “Initialize all peripherals with their default Mode ?” Choose “yes.”

Configuring Peripherals

Our development board has a lot of peripherals. The view you’re greeted by when you start a project is showing you what each pin of the processor package is connected to.

Each configured pin (amongst other things) means more code to generate, making our first project harder to understand; for the sake of making things easier to understand, we’ll clear the configuration and only set up those two peripherals we need for this lab.

Configuring the Clock

First, however, we should confirm that the system clock is set correctly. Unless stated otherwise, the system clock for your processor should always be 80 MHz (or, 120 MHz for the

B-L4S5I-IOT01A), the maximum operating frequency available. Select the Clock Configuration tab. There are a number of clock sources available, and a lot of options here for configuring not only which clock drives the core, but which clocks drive peripherals. Choices here matter: timers count clock edges; whether these edges occur at 80 MHz (120 MHz) or not has consequences for system operation.

HCLK is key for now. If it isn’t set to 80 (MHz), do so. The tool will find the appropriate configuration of multiplexors and clock sources to reach the target.

Configuring LED2

Now return to the Pinout &amp; Configuration tab. We’re going to clear the pinout and set up individual pins, but before we do: find PB14, and observe its label LED2 [LED_GREEN]. You can find this by simply looking around the edge of the chip, or by searching for “LED” in the search box below the illustration of the pinout. The PB14 pin is by default configured to drive an LED; after clearing the pinout and resetting all pins, including this one, we’ll reconfigure it to drive the LED again.

Select the Pinout pulldown menu, and “clear pinouts.” This will reset the pins, remove the labels, and eliminate all associated skeleton code.

After confirmation, your pinout should look like this, and be ready for us to begin configuring.

Find PB14 again. How do we know this is connected to the LED? (a) It was before, and (b) reference material for the development board tells us so. For instance, the B-L475E-IOT01A user’s manual details the available peripherals, and their interface(s):

(The same specs appear in Table 4 of the B-L4S5I-IOT01A user’s manual.)

In order to connect PB14 to LED2, we need to set the mode of this pin to GPIO_Output. Left-click on the pin, and select this option.

It’s useful at this point to additionally label the pin. Labels make it easier to find things in (using the search feature below the pinout), and can also be used in STM32CubeIDE when we’re writing code. Right-click on PB14 and “Enter User Label.” Label the pin as “LED” and we’ll use this to access it when we write our code.

This is all that is necessary to set up our LED!

Configuring TIM17

Before configuring the timer that we’ll use to make our LED blink, there is one other change to make to how timer 17, TIM17, is being used.

Expand “System Core” on the left hand side, and select SYS. This will expand SYS Mode and

Configuration.

● In Mode, select “SysTick” from Timebase Source.

Configuring TIM2

Next, we’ll configure the timer that we’ll use to make our light blink. We’ll see over the course of the semester how this works, in detail. The short version: timers count clock edges, and take configurable action when the count reaches certain values. Our timer will count clock edges for 1 second, triggering an interrupt, which we will use to toggle the LED.

The timers are internal to the processor: i.e., they aren’t accessible through pins. To get started with configuring TIM2, we first select it from the timers. Expand “Timers” on the left hand side, and select “TIM2,” as illustrated below. This will expand TIM2 Mode and Configuration. Now we need to configure the clock used for counting, and configure the target value.

● In Mode, select “Internal Clock” from Clock Source. This means the timer will count processor clock edges at 80 MHz (120 MHz).

The prescaler is the number of clock cycles before the timer’s counter increments. The counter period is the number of counter increments before an interrupt is raised. If we set the prescalar to 40,000, and counter period to 2,000, after 40,000 clock cycles, the counter increments; after 2,000 increments (= 2,000 x 40,000 = 80,000,000 clock cycles), an interrupt is raised. If the clock runs at 80 MHz, this means the timer TIM2 will raise an interrupt every 1 second. We will use this to trigger code that will change the output of pin PB14, thereby changing whether LED2 is lit or not!

If you are using the B-L4S5I-IOT01A, you need to pick a prescaler and counter period that counts 120 million cycles instead! E.g., 40,000 and 3,000.

● In Configuration, under Parameter Settings, set Prescaler to 40000, and Counter Period to 2000 (3000).

● In Configuration, under NVIC Settings, tick “Enabled” for TIM2 global interrupt.

At this point, the configuration is complete, and we need to generate the code skeleton that we’ll modify to complete the project. There are a variety of ways to trigger code generation:

● Save the IOC file using the save icon. This will prompt you to generate code.

● Right-click the IOC file in the Project Explorer pane and select Generate Code. ● From the Project pull-down menu select Generate Code.

Writing, Deploying, Debugging, and Running Your Code

At this point, there is very little code that we need to write to finish our project: just three lines!

The first line of code turns on our timer. Look for USER CODE BEGIN 2. In this section, write:

HAL_TIM_Base_Start_IT(&amp;htim2);

and a comment.

This code takes the address of the timer’s configuration register (&amp;htim2, defined for you by the skeleton code), and uses a hardware abstraction layer (HAL) function call to direct the timer to start, triggering its interrupt (that’s the IT part of the function name) whenever the timer fills and resets.

Note: write your code between the BEGIN 2 and END 2 comments; that way, if you have to regenerate the skeleton code, your code will be preserved.

Now look for USER CODE BEGIN 4. In this section, write the following.

HAL_TIM_PeriodElapsedCallback is a virtual function that, when defined, is called by the interrupt handler for timers. More on that later. For now: when the timer reaches its maximum and resets, this function is called.

HAL_GPIO_TogglePin takes two inputs: a block of GPIO pins, or port, and a specific pin. Fortunately, we don’t need to know the memory addresses for either of these, or do the math to work it out from pin numbers: since we labeled the pin LED, we can simply use LED_GPIO_Port to refer to the port, and LED_Pin to refer to the pin. These macros have already been defined for us elsewhere in the skeleton code.

Deploying, Debugging, and Running Code

Now we’re ready to test our code! If you’ve used Eclipse before, the interface will be familiar.

Clicking the bug starts debugging (the program will be compiled, and started on the development board, with a breakpoint set at the first line of main). Clicking the play button starts the program without connecting a debugger (the program will be compiled, and started).

When you first click the bug or play button for any project, you’ll be prompted:

Click “OK” to continue.

Note: if STM32CubeIDE complains that ST-LINK-Server could not be found, please install this software and try again.

If you started the debugger, you can walk through the code until the infinite while loop using these controls.

Press the Resume button (left of pause, right of Terminate and Relaunch) to allow the program to run (until you pause it). The green LED should begin to blink, toggling on for one second, and then off again for one second!

Additional Exercises

Want to convince yourself that you understand everything that’s going on? Here are a few variations that you can explore.

1. Change the configuration of TIM2 in the board configuration (IOC file) so LED2 toggles four times faster.

2. Change the configuration of TIM2 in source files in STM32CubeIDE so that TIM2 toggles four times slower. Remember, the IOC file is just a fancy UI to facilitate code generation!

3. Change the configuration of the system so a different LED toggles.
