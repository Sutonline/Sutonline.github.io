---
layout: post
title:  "eclipse codestyle template"
date:   2016-09-18 16:33:23 +0800
categories: [eclipse]
---

用来设置代码格式.  

```xml
<?xml version="1.0" encoding="UTF-8"?><templates><template autoinsert="true" context="fieldcomment_context" deleted="false" description="Comment for fields" enable="true" id="org.eclipse.jdt.ui.text.codetemplates.fieldcomment" name="fieldcomment">/**
*
*/</template><template autoinsert="true" context="methodcomment_context" deleted="false" description="Comment for non-overriding methods" enabled="true" id="org.eclipse.jdt.ui.text.codetemplates.methodcomment" name="methodcomment">/**
* ${tags}
*/</template><template autoinsert="true" context="delegatecomment_context" deleted="false" description="Comment for delegate functions" enable="true" id="org.eclipse.wst.jsdt.ui.text.codetemplates.delegatecomment" name="delegatecomment">/**
* ${tags}
* ${see_to_target}
*/</template><template autoinsert="true" context="typecomment_context" deleted="true" description="Comment for created types" enabled="true" id="org.eclipse.jdt.ui.text.codetemplates.typecomment" name="typecomment">/**
* ${todo} plz add Comments
* @author ${user}
* @version $$Revision:$$
*/</template><template autoinsert="true" context="typecomment_context" deleted="false" description="Comment for created types" enabled="true" id="org.eclipse.wst.jsdt.ui.text.codetemplates.typecomment" name="typecomment">/**
* @author ${user}
*
* ${tags}
*/</template><template autoinsert="true" context="gettercomment_context" deleted="false" description="Comment fro getter method" enabled="true" id="org.eclipse.jdt.ui.text.codetemplates.gettrcomment_context" name="gettercomment">/**
* @return the ${bare_field_name}
*/</template><template autoinsert="true" context="overridecomment_context" deleted="false" description="Comment for overriding methods" enabled="true" id="org.eclipse.jdt.ui.text.codetemplates.overridecomment" name="overridecomment">/**
* ${see_to_overridden}
*/</template><template autoinsert="true" context="methodcomment_context" deleted="false" description="Comment for non-overriding functions" enabled="true" id="org.eclipse.wst.jsdt.ui.text.codetemplates.methodcomment" name="methodcomment">/**
* ${tags}
*/</template><template autoinsert="true" context="settercomment_context" deleted="false" description="Comment for setter function" enabled="true" id="org.eclipse.wst.jsdt.ui.text.codetemplates.settercomment" name="settercomment">/**
* @param ${param} the ${bare_field_name} to set
*/</template><template autoinsert="true" context="filecomment_context" deleted="false" description="Comment for created JavaScript files" enabled="true" id="org.eclipse.wst.jsdt.ui.text.codetemplates.filecomment" name="filecomment">/**
*
*/</template><template autoinsert="true" context="fieldcomment_context" deleted="false" description="Comment for overriding functions" enabled="true" id="org.eclipse.wst.jsdt.ui.text.codetemplates.overridecomment" name="overridecomment">/*(non-Jsdoc)
* ${see_to_overridden}
*/</template><template autoinsert="true" context="fieldcomment_context" deleted="false" description="Comment for vars" enabled="true" id="org.eclipse.wst.jsdt.ui.text.codetemplates.fieldcomment" name="fieldcomment">/**
*
*/</template><template autoinsert="true" context="gettercomment_context" deleted="false" description="Comment for getter function" enabled="true" id="org.eclipse.wst.jsdt.ui.text.codetemplates.gettercomment" name="gettercomment">/**
* @return the ${bare_field_name}
*/</template><template autoinsert="true" context="settercomment_context" deleted="false" description="Comment for setter method" enabled="true" id="org.eclipse.jdt.ui.text.codetemplates.settercomment" name="settercomment">/**
* @param ${param} the ${bare_field_name} to set
*/</template><template autoinsert="true" context="constructorcomment_context" deleted="false" description="Comment for created constructors" enabled="true" id="org.eclipse.jdt.ui.text.codetemplates.constructorcomment" name="constructorcomment">/**
* ${tags}
*/</template><template autoinsert="true" context="constructorcomment_context" deleted="false" description="Comment for created constructors" enabled="true" id="org.eclipse.wst.jsdt.ui.text.codetemplates.constructorcomment" name="constructorcomment">/**
* ${tags}
*/</template><template autoinsert="false" context="filecomment_context" deleted="false" description="Comment for created Java files" enabled="true" id="org.eclipse.jdt.ui.text.codetemplates.filecomment" name="filecomment">/**
* Copyright (c) ${year} sut
* All rights reserved.
*
* project : ${project_name}
* created : ${date} ${time}
* cvs: $$Id: $$
*/</template><template autoinsert="true" context="delegatecomment_context" deleted="false" description="Comment for delegate methods" enabled="true" id="org.eclipse.jdt.ui.text.codetemplates.delegatecomment" name="delegatecomment">/**
* ${tags}
* ${see_to_target}
*/</template>
</templates>
```