<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">
    <h3>Journal Papers</h3>
    <ol class="bibliography">
        {% for link in site.data.publications.journal %}
        <li>
            <div class="pub-row">
                <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
                    {% if link.image %}
                    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
                    {% endif %}
                </div>
                <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
                    <div class="title">{{ link.title }}</div>
                    <div class="author">{{ link.authors }}</div>
                    <div class="periodical"><em>{{ link.journal }}</em></div>
                </div>
            </div>
        </li>
        {% endfor %}
    </ol>

    <h3>International Conferences</h3>
    <ol class="bibliography">
        {% for link in site.data.publications.international %}
        <li>
            <div class="pub-row">
                <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
                    {% if link.conference_short %}
                    <abbr class="badge">{{ link.conference_short }}</abbr>
                    {% endif %}
                </div>
                <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
                    <div class="title">{{ link.title }}</div>
                    <div class="author">{{ link.authors }}</div>
                    <div class="periodical"><em>{{ link.conference }}</em></div>
                </div>
            </div>
        </li>
        {% endfor %}
    </ol>

    <h3>Domestic Conferences</h3>
    <ol class="bibliography">
        {% for link in site.data.publications.domestic %}
        <li>
            <div class="pub-row">
                <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
                    {% if link.conference_short %}
                    <abbr class="badge">{{ link.conference_short }}</abbr>
                    {% endif %}
                </div>
                <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
                    <div class="title">{{ link.title }}</div>
                    <div class="author">{{ link.authors }}</div>
                    <div class="periodical"><em>{{ link.conference }}</em></div>
                </div>
            </div>
        </li>
        {% endfor %}
    </ol>
</div>
