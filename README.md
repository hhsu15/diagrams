# Diagram 

Basics for making a process diagram

Reference links:

[part I](https://medium.com/doflowy/sop%E8%A3%BD%E4%BD%9C%E6%95%99%E5%AD%B8-%E6%96%B0%E6%89%8B%E9%81%A9%E7%94%A8-sop%E7%AF%84%E4%BE%8B-%E6%B5%81%E7%A8%8B%E5%9C%96-%E8%A3%BD%E4%BD%9C%E6%B5%81%E7%A8%8B%E5%85%A8%E5%85%AC%E9%96%8B-baaf6e90c578)

[part II](https://medium.com/doflowy/sop%E8%A3%BD%E4%BD%9C%E6%95%99%E5%AD%B8-%E6%B5%81%E7%A8%8B%E5%9C%96%E6%95%99%E5%AD%B8-%E9%87%8D%E9%BB%9E%E7%AF%84%E4%BE%8B-bpmn%E7%AC%A6%E8%99%9F%E4%BB%8B%E7%B4%B9-96499e91e5d4)

[part III](https://medium.com/doflowy/sop%E8%A3%BD%E4%BD%9C%E6%95%99%E5%AD%B8-%E6%B5%81%E7%A8%8B%E5%9C%96%E7%AC%A6%E8%99%9F%E6%95%B4%E7%90%86-bpmn2-0%E9%80%B2%E9%9A%8E%E7%AC%A6%E8%99%9F%E6%95%99%E5%AD%B8-aea950aab991)

## BPMN
BPMN (Business Process Model and Notation) uses some specific notations for different types of elements. 

[Official reference](https://www.omg.org/spec/BPMN/2.0/PDF)

### Basics

1. Event (Start event and End event) are noted as circle. An Event is something that “happens” during the course of a Process or a　Choreography. These Events affect the flow of the model and usually have a cause (trigger) or an impact (result).
  - there can be also other events such as 
    - message event (e.g., once message is delivered)
    - time event (e.g., wait for certain time)
2. Activity. An Activity is a generic term for work that company performs in a Process. An Activity can be atomic or non-atomic(compound).
  - Task (rectangle). A Task is an atomic Activity that is included within a Process. A Task is used when the work in the Process is not broken down to a finer level of Process detail.
  - Sub-process (rectangle with plus sign). A Sub-Process is a compound Activity that is included within a Process or Choreography. It is compound in that it can be broken down into a finer level of detail (a Process or Choreography) through a set of sub-Activities.
3. Swimlanes (pool) that distingush participants.
4. Sequence Flow (solid arrow ->) A Sequence Flow is used to show the order that Activities will be performed in a Process and in a Choreography.
5. Message Flow (doted arrow -->)A Message Flow is used to show the flow of Messages between two Participants that are prepared to send and receive them. In BPMN, two separate Pools in a Collaboration Diagram will represent the two Participants (e.g., PartnerEntities and/or PartnerRoles).
6. Gateway (Diamond)
  - exclusive gateway (with X). E.g., yes or no or unsure
  - inclusive gateway (with O). E.g., can go multiple ways at the same time
  - parallel gateway (with +). Do all multiple things

