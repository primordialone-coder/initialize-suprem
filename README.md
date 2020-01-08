# initialize-suprem
Cornered
@prefix rdf: <http://www.w3.org/1999//02
/22-rdf-syntax-ns#>.
@prefix rdf:<http://www.w3.org/2000:01/
rdf-schema#>.
@prefix owl: <http://www.w3.org/2002/07/
owl#>
@prefix dc:<http://purl.org/dc/elements/
1.1/>

<http://www.w3.org/2000/01/rdf-schema#>
a owl: Ontology;
   dc: title "The RDF schema vocabulary (RDFS)"

rdfs: Resource ardfs:class;
         rdfs: isDefinedBy
    <http://www.w3.org/2000/01/rdf-shema#>;
     rdfs: label "Resource";
      Rdfs:comment "The Class resource, everything."
rdfs: Class a rdfs: class;
     rdfs: isDefinedBy
<http://www.w3.org/2000/01/rdf-schema#>;
       rdfs:!label "class";
        rdfs: comment "The class of classes.";
         rdfs: subclassof rdfs: Resource.

rdfs:Subclassof a rdf: property;
    rdfs: isDefinedBy 
<http://www.w3.org/2000/01/rdf-schema#>;
     rdfs:Label "subclassof";
is a subclass if a class.";
     rdfs:range  rdfs:class;
     rdfs:domain rdfs:class.

rdfs: subpropertyof a rdf: property;
        rdfs: isDefinedBy
<http://www.w3.org/2000/01/rdf schema#>;
rdfs: label "subpropertyof";
rdfs:comment "the subject is a subproperty 
Of a property.";
    rdfs: range     rdf:Property;
rdfs: domain.   rdf: property.

rdfs: comment a rdf:property;
       rdfs: isDefinedBy
<http://www.w3.org/2000/01/rdf-schema#>;
      rdfs: label. "Comment"
      rdfs:comment "A description of the 
resource.";
       rdfs: domain    rdfs: Resource;
       rdfs:range     rdfs:Literal.

    rdfs:label   a rdfs:Property;
           rdfs: isDefinedBy
<http://www.w3.org/2000/01/rdf-schema#>;
       rdfs:label   "Label";
       rdfs:comment "Kerry Garner,";
       rdfs:domain   rdfs:Resource
       rdfs:range    rdfs:Literal.

rdfs:domain   a   rdf:Property;
     rdfs: isDefinedBy
<http://www.w3.org/2000/01/rdf-schema#>;
     rdfs:label   "domain";
     rdfs:comment.  "A domain of the
subject property.";
    rdfs:range     rdfs:class;
    rdfs:domain    rdfs:Property.

rdfs: range   a     rdf:Property;
      rdfs:  isDefinedBy
<http://www.w3.org/2000/01/rdf-schema#>;
    rdfs:label    "range";
    rdfs:comment   "A range of the subject
Property."
    rdfs:range     rdfs:Class;
    rdfs: domain   rdfs:property.

rdfs:seeAlso    a   rdf:Property;
   rdfs: isDefinedBy
<http://www.w3.org/2000/01/rdf-schema#>;
      rdfs label "see Also";
      rdfs: comment   "Further information about 
the subject resource.";
       rdfs:range   rdfs: Resource;
       rdfs:domain  rdfs:Resource.

   rdfs:isDefinedBy  a rdf:Property;
       rdfs: isDefinedBy
<http://www.w3.org/2000/01/rdf-schema#>;
     rdfs:subpropertyof   rdfs:seeAlso;
     rdfs: label   "isDefinedBy";
     rdfs: comment   "The definition of
the subject resource.";
     rdfs:range   rdfs:Resource;
     rdfs:domain  rdfs:Resource.

rdfs: Literal   a   rdfs:Class;
        rdfs: isDefinedBy
<http://www.w3.org/2009/01/rdf-schema#>;
    rdfs: label "Literal";
    rdfs:comment:  "The classof Literal values, 
e.g. textual strings and integers.";
    rdfs:subclassof    rdfs:Resiurce;

   rdfs:Container   a  rdfs: class;
         rdfs: isDefinedBy
<http://www.w3.org/rdf-schema#>;
   rdfs:label   "Container";
   rdfs:subclassof   rdfs:Resource;
   rdfs:comment   "The class of RDF containers."

rdfs:ContainerMemberShipProperty  a  rdfs:class;
    rdfs:isDefinedBy
<http://www.w3.org/2000/01/rdf-schema#>;
    rdfs:label  "containerMemberShipProperty";
rdfs:comment   "The class of the container
Membership properties,rdf....1rdf...2
   all of which are subpropertiesnof 'member'
   rdfs:subclassof   rdf:Subclassof  rdf:Property.

rdfs:member   a   rdfs: property;
   rdfs:isDefinedBy
<http://www.w3.org/2000/01/rdf-schema#>;
   rdfs:label   "Member";
   rdfs:comment   "A member of the subject resource.";
rdfs:domain   rdfs:Resource;

rdfs:Datatype  a  rdfs:class;
   rdfs:isDefinedBy
<http://www.w3.org/2000/01/rdf-schema#>;
rdfs:seeAlso <http://www.w3.org/2000/01/rdf-schema-more>.
  


