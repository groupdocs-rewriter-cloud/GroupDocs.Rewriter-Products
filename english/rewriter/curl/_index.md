---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Rewriter"
product_tag: "rewriter"
platform: "cURL"
platform_tag: "curl"

############################# Head ############################
head_title: "Paraphrase, simplify, summarize texts and documents from the command line"
head_description: "Interact with GroupDocs.Rewriter REST API directly from the command line or Bash scripts without installing any software. Automatically paraphrase, summarize or simplify texts and documents with the quality of the professional copyrighter."

############################# Header ############################
title: "Paraphrase, simplify, summarize texts and documents from the command line"
description: "Interact with GroupDocs.Rewriter REST API directly from the command line or Bash scripts without installing any software. Automatically paraphrase, summarize or simplify texts and documents with the quality of the professional copyrighter."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "Rewriter for Cloud"
        image: "/sdk/272x272/groupdocs_rewriter-for-curl.png"
        product: "GroupDocs.Rewriter"
        platform: "cURL"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"


            # button loop
            - link: "https://docs.groupdocs.cloud/rewriter/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-rewriter-cloud/"
        link_learn: "https://docs.groupdocs.cloud/rewriter/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Rewriter is an easy-to-use and versatile online service for summarizing, rephrasing or simplifying the texts with full preservation of the meaning. Its advanced AI reads and understands the text and then rephrases it in various wordings, providing a plagiarism-free result without losing the original meaning. While the background process is very complex and resource-intensive, you do not have to worry about formulas, machine learning, and load – our cloud services do all the work.

      The service provides a versatile and easy-to-use REST API, which can be accessed without installing any software. Just use cURL commands and combine them into scripts for complex tasks. You can also use third party REST API tools like Postman. This allows you to use GroupDocs.Rewriter on any platform with an internet connection, even those not yet covered by the SDK.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Main capabilities of GroupDocs.Rewriter Cloud
      
        left:
          enable: true
          icon: "fas fa-crop"
          title: "Supported features"
          content: |
            * Paraphrase
            * Summarize
            * Simplify
            * Synonymize
            * Detect paraphrasing
        right:
          enable: true
          icon: "fas fa-file-alt"
          title: "Supported languages"
          content: |
            * Arabic
            * English
            * French
            * German
            * Hindi
            * Indonesian
            * Italian
            * Portuguese
            * Russian
            * Slovak
            * Spanish
            * Thai
            * Ukrainian
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Rewriter Cloud supports most popular document formats

        left:
          enable: true
          table:
            # table loop
            - title: "Office documents"
              content: |
                * **Microsoft Word**
                * **OpenDocument**
                * **RTF**
                
        right:
          enable: true
          table:
            # table loop
            - title: "Other formats"
              content: |
                * **PDF**
                * **TXT**
        


      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Rewriter Cloud for cURL works on any device or platform with Internet connection
      
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Development Environments"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build Automation Tool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "Advanced features of document paraphrasing REST API"

    feature:
      # feature loop
      - icon: "fas fa-language"
        content: "Creates unique content while fully preserving the original message"

      # feature loop
      - icon: "fas fa-file"
        content: "Supports Microsoft Office, OpenOffice and PDF documents without additional software"

      # feature loop
      - icon: "fas fa-random"
        content: "Converts paraphrased documents to different formats"
      
      # feature loop
      - icon: "fas fa-link"
        content: "Processes files from URLs and public repositories"
        
      # feature loop
      - icon: "fas fa-mobile"
        content: "Works on any device and platform, including smartphones"
        
      # feature loop
      - icon: "fas fa-list"
        content: "API explorer based on Swagger collection"
    
    more_feature:
      # more_feature_loop
      - title: "Any language, platform and storage service provider"
        content: "GroupDocs.Rewriter is a REST API that can easily be integrated into any application written in any programming language capable of handling HTTP requests and responses. It natively supports all popular cloud storage services such as Google Cloud, Drive, DropBox and Amazon S3 to interact without any dependencies."

      # more_feature_loop
      - title: "Quick start with GroupDocs.Rewriter REST API"
        content: "GroupDocs.Rewriter Cloud API comes with detailed developer references and live code examples for all major programming languages to start working with API features in no time. Simply create a free account at GroupDocs Cloud, get APP SID & Key information to communicate with GroupDocs Cloud API and you are ready to make an API request on any platform using cURL commands."

      # more_feature_loop
      - title: "Rewrite plain text - cURL"
        content: |
          
          
          ```shell
            //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
            // Getting token
            curl --location --reqest POST 'https://id.groupdocs.cloud/connect/token' \
                --header 'Content-Type: application/x-www-form-urlencoded' \
                --data-urlencode 'grant_type=client_credentials' \
                --data-urlencode 'client_id=CLIENT-ID-VALUE' \
                --data-urlencode 'client_secret=CLIENT-SECRET-VALUE'
            //response
            {
                "access_token": "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9...LxLejtsVFwrZpHA",
                "expires_in": 3600,
                "token_type": "Bearer"
            }
            // Sending text for paraphrasing
            curl --location --request POST 'https://api.groupdocs.cloud/v2.0/rewriter/paraphrase/text' \
                --header 'Content-Type: application/json' \
                --header 'Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9...LxLejtsVFwrZpHA' \
                --data '{
                    "language": "en",
                    "text": "Hello, everyone! We will try to rephrase this text into something new.",
                    "suggestions": "One",
                    "diversityDegree": "Medium"
                }'
            //response
            {
                "status": 202,
                "message": "Starting",
                "id": "dae5390e-3658-4bff-85bf-4a77cc04eaa5_text"
            }
            //getting result
            curl --request GET --location ''https://api.groupdocs.cloud/v2.0/rewriter/paraphrase/text/dae5390e-3658-4bff-85bf-4a77cc04eaa5_text'' \
                --header 'Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9...LxLejtsVFwrZpHA'	
            //response
            {
                "statusCode": 200,
                "message": "Text processed successfully",
                "paraphraseReult": "Hello, everyone! We are going to try to recast this text as something new."
            }	
          ```
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Rewriter Cloud offers SDKs for popular programming languages and platforms:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Rewriter Cloud SDK for cURL"
          image: "/sdk/272x272/groupdocs_rewriter-for-curl.png"
          product: "GroupDocs.Rewriter"
          platform: "cURL"
          link: "/rewriter/curl/"

        # solution loop
        - img_alt: "GroupDocs.Rewriter Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_rewriter-for-net.png"
          product: "GroupDocs.Rewriter"
          platform: ".NET"
          link: "/rewriter/net/"

        # solution loop
        - img_alt: "GroupDocs.Rewriter Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_rewriter-for-python.png"
          product: "GroupDocs.Rewriter"
          platform: "Python"
          link: "/rewriter/python/"

############################# Back to top ###############################
back_to_top:
  enable: true
---