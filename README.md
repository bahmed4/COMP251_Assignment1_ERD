# Assignment 1 - Creating an ER Diagram for MPLSRenters.com
This assignment will meet each of the objectives below:
1. Translate business use cases for data into entity relationships

2. Determine appropriate entity structure for relational databases

3. Apply the correct terminology to a ER Model

4. Design an ER model

## Instructions
For this assignment, your task is to analyze the provided business description and identify the necessary business rules to create an ER diagram. These rules will encompass relationships, constraints, and data requirements.

You are required to compile a README.md file, which will detail each entity along with a brief description of its purpose and the data it collects. Additionally, identify the relationships between entities and note any assumptions or questions you may have for the client based on the business description. You will also decide the answers to your assumptions on behalf of the client.

After completing the README.md file, your next step is to construct an ER Diagram based on the identified relationships from the business description. This diagram should be created using a free web-based tool called 'draw.io.' You'll find the shapes needed for your ER diagram under the 'Entity Relation' tab. Instructions on how to operate draw.io can be found in the assignment resources section below. **DRAW.IO must be used as your ER diagram tool**

## Business Description
MPLSRenters.com is a website that allows prospective apartment renters to create a profile and have
high-end luxury apartments make offers to prospective renters.

1.  A property can have many high-end amenities associated with it. The amenities that are
associated with a property are preset amenities that can be added to a property.  Each amenity will have a name and description. 
 If properties have unique amenities that are not a part of the preset amenities, then those details will go into
the long description for each property. A property will contain information such as first and last name, email, phone, address, short and long description, longitude/latitude of property, and rent range (the lowest and highest amount you can expect to pay).
2. Prospective renters can add as many amenities to their profile as they deem necessary. The amenities will
be the same preset amenities that can be added to a property.  A renter will collect the same information a property would collect, but will also include a renter's decision date, the number of bedrooms and bathrooms, and the lower and max rent value they are willing to spend.  
3. Prospective renters can add as many properties to their profile as they desire. A prospective renter can exist in the system without having a property associated with a profile.
4. A property can have multiple property agents associated with a property. A property does not
have to be associated with a property agent to exist within the database. Property agents can
be activated and deactivated from the system based on whether or not payment for a monthly
package was made on time.
5. Both a profile and a property can receive a classification. There are only three pre-determined
classifications that can be associated with a profile or property. A profile is classified based on
the lower and upper range a prospective renter is looking to have for monthly rent. A
property is classified based on the select amenities, square footage, and lower/upper rent range. Each classification will contain a title, description, and a classification identifier (ex.  A high-luxury, B high - mid-luxury, or C luxury property)
6. A property agent can sign-up for one of three packages. All property agents must have an agent
package. An agent package determines how much access they will be granted to user profile
information.  An Agent package will contain a name, the package description, and an agent option selection (monthly payment package or yearly payment package)
7. Property agents are able to make multiple offers to those who have profiles in the system. A
profile can receive multiple offers from an agent. A profile can decline or entertain an offer.  An offer will contain information such as a description of the offer, the offer expiration date, and the property name for which the offer is being made.

## Submission Guidelines

For this assignment, you will submit 2 items to the repository that has been assigned to you.  The two items that you will need to submit are listed below: 
1. The README.MD file that identifies the various Entities and a brief description of the entity and possible attributes, relationships, and assumptions. 
   1. When identifying relationships be sure to bold and uppercase the entity name, underline the verb and make sure relationships are bi-directional. 
   2. When identifying assumptions, make sure to answer your assumption with either a Yes or No and make sure your response is properly reflected in the ER diagram.  
   3. You can override this README.MD file that contains the instructions or extend this README.MD file by listing your requirements below the Assignment Resources section.

2. The draw.io XML file that contains your ER Diagram.  You will also need to take a snippet of the ER Diagram and add it as an image in your README file.

Once you have completed both of the items above, you will need to submit the link to your repository for assignment 1 prior to the due date and time listed.  Make sure you receive an email confirmation notifying you that the assignment has been submitted.

### Rubric
| Criteria           | Description                             | Points |
| -------------------| --------------------------------------- | ------ |
|**Deliverable 1 - Write-up documented in README.md file**   | Write-up identifies the various entities with brief description (4pts) <br> Write-up identifies the various relationships that exist between the entities (6pt) <br> Write-up list assumptions that provides context for cardinality and entity strength (2 pts) <br> Write-up contains uppercase entity names, underlined verb and relationships are bi-directional (3 pts)  |   15   |
|**Deliverable 2 - Properly structured ER diagram** | All Entities identified in deliverable 1 are visually represented in Workbench ER diagram. (4pts) <br> Relationship strength is indicated by solid or dotted line (2pt) <br> Foreign keys and Primary keys are identified and correctly assigned (2 pts) <br> Each column name indicates null vs not null (2pt) <br> Image of ER diagram is depicted in README.MD file (2 pt) <br> Associative entities are identified and properly captures the relationship between the two entities(3 pts)   |   15   |
|           |        |**Total Points:   30**   |

<mxfile host="app.diagrams.net.">
  <diagram name="Lab 2 ERD" id="ND5k1XugLXEeYYsTM9-_">
    <mxGraphModel dx="1414" dy="743" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="850" pageHeight="1100" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-1" parent="1" style="swimlane;fontStyle=1;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=0;marginBottom=0;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" value="STUDENT" vertex="1">
          <mxGeometry height="108" width="210" x="380" y="120" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-2" parent="ZnV8sNZjAnpfgKRaxHct-1" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;fontStyle=1;" value="*student_id" vertex="1">
          <mxGeometry height="26" width="210" y="30" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-3" parent="ZnV8sNZjAnpfgKRaxHct-1" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="student_name" vertex="1">
          <mxGeometry height="26" width="210" y="56" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-4" parent="ZnV8sNZjAnpfgKRaxHct-1" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="student_address" vertex="1">
          <mxGeometry height="26" width="210" y="82" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-5" parent="1" style="swimlane;fontStyle=1;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=0;marginBottom=0;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" value="SEAT" vertex="1">
          <mxGeometry height="82" width="210" x="40" y="120" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-6" parent="ZnV8sNZjAnpfgKRaxHct-5" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;fontStyle=1;" value="*seat_no" vertex="1">
          <mxGeometry height="26" width="210" y="30" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-7" parent="ZnV8sNZjAnpfgKRaxHct-5" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="seat_position" vertex="1">
          <mxGeometry height="26" width="210" y="56" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-8" parent="1" style="swimlane;fontStyle=1;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=0;marginBottom=0;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" value="ENROLLMENT" vertex="1">
          <mxGeometry height="108" width="210" x="720" y="120" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-9" parent="ZnV8sNZjAnpfgKRaxHct-8" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="student_id (FK)" vertex="1">
          <mxGeometry height="26" width="210" y="30" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-10" parent="ZnV8sNZjAnpfgKRaxHct-8" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="course_name (FK)" vertex="1">
          <mxGeometry height="26" width="210" y="56" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-11" parent="ZnV8sNZjAnpfgKRaxHct-8" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="course_number (FK)" vertex="1">
          <mxGeometry height="26" width="210" y="82" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-12" parent="1" style="swimlane;fontStyle=1;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=0;marginBottom=0;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" value="COURSE" vertex="1">
          <mxGeometry height="82" width="210" x="1060" y="120" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-13" parent="ZnV8sNZjAnpfgKRaxHct-12" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;fontStyle=1;" value="*course_name" vertex="1">
          <mxGeometry height="26" width="210" y="30" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-14" parent="ZnV8sNZjAnpfgKRaxHct-12" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;fontStyle=1;" value="*course_number" vertex="1">
          <mxGeometry height="26" width="210" y="56" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-15" parent="1" style="swimlane;fontStyle=1;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=0;marginBottom=0;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" value="INSTRUCTOR" vertex="1">
          <mxGeometry height="108" width="210" x="1400" y="120" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-16" parent="ZnV8sNZjAnpfgKRaxHct-15" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;fontStyle=1;" value="*instructor_no" vertex="1">
          <mxGeometry height="26" width="210" y="30" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-17" parent="ZnV8sNZjAnpfgKRaxHct-15" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="instructor_name" vertex="1">
          <mxGeometry height="26" width="210" y="56" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-18" parent="ZnV8sNZjAnpfgKRaxHct-15" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="instructor_faculty" vertex="1">
          <mxGeometry height="26" width="210" y="82" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-19" parent="1" style="swimlane;fontStyle=1;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=0;marginBottom=0;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" value="COURSE_SECTION" vertex="1">
          <mxGeometry height="108" width="210" x="1060" y="400" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-20" parent="ZnV8sNZjAnpfgKRaxHct-19" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="course_name (FK)" vertex="1">
          <mxGeometry height="26" width="210" y="30" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-21" parent="ZnV8sNZjAnpfgKRaxHct-19" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="course_number (FK)" vertex="1">
          <mxGeometry height="26" width="210" y="56" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-22" parent="ZnV8sNZjAnpfgKRaxHct-19" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="section_number (FK)" vertex="1">
          <mxGeometry height="26" width="210" y="82" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-23" parent="1" style="swimlane;fontStyle=1;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=0;marginBottom=0;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" value="SECTION" vertex="1">
          <mxGeometry height="56" width="210" x="1060" y="660" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-24" parent="ZnV8sNZjAnpfgKRaxHct-23" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;fontStyle=1;" value="*section_number" vertex="1">
          <mxGeometry height="26" width="210" y="30" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-25" parent="1" style="swimlane;fontStyle=1;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=0;marginBottom=0;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" value="PROFESSOR" vertex="1">
          <mxGeometry height="108" width="210" x="1060" y="880" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-26" parent="ZnV8sNZjAnpfgKRaxHct-25" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;fontStyle=1;" value="*professor_id" vertex="1">
          <mxGeometry height="26" width="210" y="30" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-27" parent="ZnV8sNZjAnpfgKRaxHct-25" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="professor_name" vertex="1">
          <mxGeometry height="26" width="210" y="56" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-28" parent="ZnV8sNZjAnpfgKRaxHct-25" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;spacingLeft=6;html=1;" value="professor_faculty" vertex="1">
          <mxGeometry height="26" width="210" y="82" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-29" edge="1" parent="1" source="ZnV8sNZjAnpfgKRaxHct-1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;html=1;startArrow=ERmandOne;endArrow=ERmandOne;startFill=0;endFill=0;startSize=14;endSize=14;fontStyle=2;labelBackgroundColor=#ffffff;exitX=0;exitY=0.5;entryX=1;entryY=0.5;" target="ZnV8sNZjAnpfgKRaxHct-5" value="fills">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-30" edge="1" parent="1" source="ZnV8sNZjAnpfgKRaxHct-1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;html=1;startArrow=ERmandOne;endArrow=ERoneToMany;startFill=0;endFill=0;startSize=14;endSize=14;fontStyle=2;labelBackgroundColor=#ffffff;exitX=1;exitY=0.5;entryX=0;entryY=0.5;" target="ZnV8sNZjAnpfgKRaxHct-8" value="has">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-31" edge="1" parent="1" source="ZnV8sNZjAnpfgKRaxHct-12" style="edgeStyle=orthogonalEdgeStyle;rounded=0;html=1;startArrow=ERmandOne;endArrow=ERoneToMany;startFill=0;endFill=0;startSize=14;endSize=14;fontStyle=2;labelBackgroundColor=#ffffff;exitX=0;exitY=0.5;entryX=1;entryY=0.5;" target="ZnV8sNZjAnpfgKRaxHct-8" value="has">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-32" edge="1" parent="1" source="ZnV8sNZjAnpfgKRaxHct-15" style="edgeStyle=orthogonalEdgeStyle;rounded=0;html=1;startArrow=ERmandOne;endArrow=ERoneToMany;startFill=0;endFill=0;startSize=14;endSize=14;fontStyle=2;labelBackgroundColor=#ffffff;exitX=0;exitY=0.5;entryX=1;entryY=0.5;" target="ZnV8sNZjAnpfgKRaxHct-12" value="teaches">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-33" edge="1" parent="1" source="ZnV8sNZjAnpfgKRaxHct-12" style="edgeStyle=orthogonalEdgeStyle;rounded=0;html=1;startArrow=ERmandOne;endArrow=ERoneToMany;startFill=0;endFill=0;startSize=14;endSize=14;fontStyle=2;labelBackgroundColor=#ffffff;exitX=0.5;exitY=1;entryX=0.5;entryY=0;" target="ZnV8sNZjAnpfgKRaxHct-19" value="has">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-34" edge="1" parent="1" source="ZnV8sNZjAnpfgKRaxHct-23" style="edgeStyle=orthogonalEdgeStyle;rounded=0;html=1;startArrow=ERmandOne;endArrow=ERoneToMany;startFill=0;endFill=0;startSize=14;endSize=14;fontStyle=2;labelBackgroundColor=#ffffff;exitX=0.5;exitY=0;entryX=0.5;entryY=1;" target="ZnV8sNZjAnpfgKRaxHct-19" value="has">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-35" edge="1" parent="1" source="ZnV8sNZjAnpfgKRaxHct-25" style="edgeStyle=orthogonalEdgeStyle;rounded=0;html=1;startArrow=ERmandOne;endArrow=ERzeroToMany;startFill=0;endFill=0;startSize=14;endSize=14;fontStyle=2;labelBackgroundColor=#ffffff;exitX=0.5;exitY=0;entryX=0.5;entryY=1;" target="ZnV8sNZjAnpfgKRaxHct-23" value="teaches">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="ZnV8sNZjAnpfgKRaxHct-36" parent="1" style="text;html=1;fontSize=18;fontStyle=1;align=left;" value="Lab 2 – Conceptual ERD (School) – Bilal Ahmed" vertex="1">
          <mxGeometry height="40" width="600" x="40" y="40" as="geometry" />
        </mxCell>
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>

## Assignment Resources
- [Mark-down Syntax Cheat Sheet](https://enterprise.github.com/downloads/en/markdown-cheatsheet.pdf)
- [Make a ReadMe file Web-based Editor](https://www.makeareadme.com/)
- [Draw.io Web-based diagramming tool](https://app.diagrams.net/)
- [Creating Entity Relationship Diagrams using Draw.io](https://www.youtube.com/watch?v=lAtCySGDD48)
