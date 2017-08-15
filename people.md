---
layout: page
title: People
subtitle: Parsa Team
---

<div class="people">

  {% for person in site.people %}
    <div class="person">
        <div class="p-pic">
          <a href="{{ person.website }}">
              <img src="{{ site.baseurl }}/img/people/{{ person.image }}" width="100" height="150" border="0">
          </a> 
        </div>
        <div class="p-name">
          <a href="{{ person.website }}">{{ person.name }}</a> <br>
          {{ person.title }}
        </div>
    </div>
  {% endfor %}
</div>

### Technical Staff

<table class="invis-tab" >
  <tbody>
   <tr>
      <td><a href="https://people.epfl.ch/rodolphe.buret?lang=en">Rodolphe Buret</a></td>
      <td>System Administrator</td>
    </tr>
  </tbody>
</table>

### Almuni

<table class="invis-tab" >
  <tbody>
    <tr>
      <td>Damien Hilloulin</td>
      <td>Master, Sept. 2016</td>
    </tr>
    <tr>
      <td>Onur Kocberber</td>
      <td>PhD, Sept. 2015</td>
    </tr>
    <tr>
      <td>Stavros Volos</td>
      <td>PhD, Sept. 2015</td>
    </tr>
    <tr>
      <td>Djordje Jevdjic</td>
      <td>PhD, Sept. 2015</td>
    </tr>
    <tr>
      <td>Cansu Kaynak</td>
      <td>PhD, Sept. 2015</td>
    </tr>
    <tr>
      <td>Sotiria Fytraki</td>
      <td>PhD, Oct. 2014</td>
    </tr>
    <tr>
      <td>Boris Grot</td>
		  <td>Postdoc,  Nov. 2013 </td>
		</tr>
    <tr>
      <td>Pejman Lotfi-Kamran</td>
		  <td>PhD,  Aug. 2013</td>
		</tr>
    <tr>
      <td>Evangelos Vlachos</td>
		  <td>PhD,  July 2013</td>
		</tr>
    <tr>
      <td>Mike Ferdman</td>
		  <td>PhD,  June 2012</td>
		</tr>
    <tr>
      <td>Jennifer Sartor</td>
		  <td>Postdoc, Oct. 2011</td>
		</tr>
  </tbody>
</table>
