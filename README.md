# TemplaterForMendix
Templater module for Mendix (+7.18.1) is a module so that anyone can use Templater in their Mendix projects.
Templater is a product from New Generation Software Ltd (https://templater.info/). The version of Templater in this module is V3.10. When no license information is provided the generated documents will contain text stating that a license is needed. 

This module gives you the ability to use tokens in Word, Excel or text documents. Demo is available on https://templaterformendix-sandbox.mxapps.io That version is the same as the full project you can download here. 
The basic examples works the same as the EmailTemplate module from Mendix only now the template can be a Word, Excel or text file. In the more advanced examples you can feed a list of objects to the template so tables can be filled in the templates. You can also feed JSON to the template but note that such a sollution currently can not be defined on runtime and should be modeled in your Mendix model. 

# How to use
The module has two main Java actions. One where a tokenlist can be passed and one where a JSON string can be passed. In the demo I have one microflow example on how to create JSON from a Mendix token list. But offcourse Mendix provides more reliable means of creating a JSON string. Only those need to be modeled out while tokens can be created at runtime. Check out the demo project for microflow examples.

#Dependencies
MxModelReflection

Regards,

Ronald

