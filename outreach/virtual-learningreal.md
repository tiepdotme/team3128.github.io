---
layout: single_page
title: 2019-2020 STEM Learning
permalink: /virtual-learning/
---

Welcome to Narwhal Code Day! Select one of the activities below and get started coding!

<br><br>

<table width="100%" border="0px" cellpadding="8px" cellspacing="0px">
    {% for week in site.data.lessons %}
    {% if week.title %}
    <tr>
        <td colspan="2" style="vertical-align: top; text-align: center">
            <span style="font-size: 40pt; line-height: 44px;">{{ week.name }}</span>
            <br>
            <span style="font-size: 16pt">{{ week.description }}</span>
        </td>
    </tr>
    {% else %}
    <tr>
        <td width="40%">
            <img src="/assets/ncd/{{ week.image }}" width="100%"/>
        </td>
        <td style="vertical-align: top">
            <span style="font-size: 40pt; line-height: 44px;">{{ week.name }}</span>
            <br>
            <span style="font-size: 16pt">{{ week.description }}</span>
        </td>
    </tr>
    <tr>
        <td colspan="2">
            <a href="{{ week.elementary }}">
                <div style="margin-top: 2px; margin-bottom: 24px;" class="button hover_animate" align="center">
                    Let's Go!
                </div>
            </a>
        </td>
    </tr>
    <tr>
        <td colspan="2">
            <a href="{{ week.middle }}">
                <div style="margin-top: 2px; margin-bottom: 24px;" class="button hover_animate" align="center">
                    Let's Go!
                </div>
            </a>
        </td>
    </tr>
    {% endif %}
    {% endfor %}
</table>
