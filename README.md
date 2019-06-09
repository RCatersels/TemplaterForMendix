# TemplaterForMendix
Templater module for Mendix (+7.18.1) is a module so that anyone can use Templater in their Mendix projects.
Templater is a product from New Generation Software Ltd (https://templater.info/). The version of Templater in this module is V3.10. When no license information is provided the generated documents will contain text stating that a license is needed. I would appreciate it when I license is bought that you learned of their product from this module.

This module gives you the ability to use tokens in Word, Excel or text documents. Demo is available on https://templaterformendix-sandbox.mxapps.io That version is the same as the full project you can download here. 
The basic examples works the same as the EmailTemplate module from Mendix only now the template can be a Word, Excel or text file. In the more advanced examples you can feed a list of objects to the template so tables can be filled in the templates. You can also feed JSON to the template but note that such a sollution currently can not be defined on runtime and should be modeled in your Mendix model. 

# How to use
1 Import MxModelReflection module from the appstore.

2 Open the MxModelReflection module and create a reference from MxObjetReference to the entity TemplateDocument in the TemplaterForMendix module. When you create this reference it will be called MxObjectReference_TemplateDocument_2 and you have to remove the underscore 2 at the end of the name to change it. Confirm the dialogue box.

![alt text](https://github.com/RCatersels/TemplaterForMendix/blob/master/MxObjectReference_TemplateDocument.png "Reference properties1")

3 The module has two main Java actions. One where a tokenlist can be passed and one where a JSON string can be passed. In the folder UseMe you will find three excluded microflows with examples on how to use these JAVA actions. The microflow Example3_List_TokenReplace_Template is an example on how to create JSON from a Mendix token list. But offcourse Mendix provides more reliable means of creating a JSON string. Only those need to be modeled out while tokens can be created at runtime.

4 To be able to enter license information hou have to connect the Microflow LicenseInformation_Retrieve to your navigation.

5 To be able to edit TemplateDocument objects a snippet is provided in th UseMe folder.

# Dependencies
MxModelReflection

Regards,

Ronald

