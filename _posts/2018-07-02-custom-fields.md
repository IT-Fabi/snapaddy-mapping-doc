---
layout: post
title:  "Section: customFields"
date:   2018-07-02 14:20:18 +0200
permalink: custom-fields
category: general
---
The "customFields"-section allows you to add custom fields to the snapADDY Grabber UI.
You can access the created custom fields by using the "id" in the mapping. The "id" always has to start with "c_".

Examples:

{% highlight json %}{% raw %}
    {
    "customFields": [
        {
            "type": "INPUT",
            "id": "c_description",
            "label": {
                "DE": "Beschreibung",
                "GB": "Description"
            },
            "properties": {
                "defaultValue": ""
            }
        },
        {
            "type": "SELECT",
            "id": "c_productInterest",
            "label": {
                "DE": "Produktinteresse",
                "GB": "Product interest"
            },
            "properties": {
                "defaultValue": "",
                "options": [
                    {
                        "label": {
                            "DE": "",
                            "GB": ""
                        },
                        "value": ""
                    },
                    {
                        "label": {
                            "DE": "snapADDY Grabber",
                            "GB": "snapADDY Grabber"
                        },
                        "value": "snapaddy_grabber"
                    },
                              {
                        "label": {
                            "DE": "snapADDY VisitReport",
                            "GB": "snapADDY VisitReport"
                        },
                        "value": "snapaddy_visitreport"
                    }
                ]
            }
        },
        {
            "type": "MULTI_SELECT",
            "id": "c_followup",
            "label": {
                "DE": "Nächste Schritte",
                "GB": "Next Steps"
            },
            "properties": {
                "defaultValue": "",
                "options": [
                    {
                        "label": {
                            "DE": "Angebot zusenden",
                            "GB": "Send offer"
                        },
                        "value": "send_offer"
                    },
                    {
                        "label": {
                            "DE": "Termin vereinbaren",
                            "GB": "Schedule appoinment"
                        },
                        "value": "schedule_appoinment"
                    },
                    {
                        "label": {
                            "DE": "Kundenbesuch",
                            "GB": "Customer visit"
                        },
                        "value": "customer_visit"
                    }
                ]
            }
        },
        {
            "type": "DATE",
            "id": "c_date",
            "label": {
                "DE": "Follow-Up Termin",
                "GB": "Follow-Up Appointment"
            },
            "properties": {
                "defaultValue": ""
            }
        }
    ]
}
{% endraw %}{% endhighlight %}


