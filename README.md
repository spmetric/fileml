FileML
======

A basic XML syntax which allows the embedding of files into an XML structure.

    :::xml
    <d n="foo">
      <f n="bar">zap</f>
      <f n="blat" id="foo_blat">zip</f>
      <d n="blort">
        <f n="bong" ref="foo_blat"/>
      </d>
      <f n="big">
    <![CDATA[
    if (a < b && a < 0) then
      {
      return 1;
      }
    else
      {
      return 0;
      }
    }
    ]]>
      </f>
    </d>

Namespace
---------
FileML can be used without namespaces, but if you want to nest XML inside
files, it will probably be valuable to distinguish FileML from the nested XML,
and the namespace urn:xmlns:spmetric.com:fileml:1.0 can be used for this
purpose.
