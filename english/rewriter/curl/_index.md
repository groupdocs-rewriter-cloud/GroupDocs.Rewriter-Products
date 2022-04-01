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
head_title: "Rewrite English Text from Word & PDF Documents via cURL Commands"
head_description: "Rewrite text from Word and PDF documents via cURL commands. Paraphrase english text and text content of your documents preserving its original sense."

############################# Header ############################
title: "Rewrite Documents using cURL"
description: "Paraphrase english text or text content of Microsoft Word and PDF documents via cURL commands without installing any external software."
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
      GroupDocs.Rewriter Cloud for cURL is a flexible text and documents paraphrasing solution to transform text or text-based content on your cloud-hosted Microsoft Word and PDF documents across 30 language pairs. Simply use cURL commands to send requests to the REST API and paraphrase English language content from the supported document types.

      The API precisely extracts the text within the contents of Word documents and PDF files, rewrites it and replaces the original document's content by the paraphrased one.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the main features supported by GroupDocs.Rewriter Cloud.
      
        left:
          enable: true
          icon: "fas fa-crop"
          title: "Documents Rewriter"
          content: |
            * Rewrite Plain Text
            * Rewrite Word Documents
            * Rewrite PDF Documents
        right:
          enable: true
          icon: "fas fa-file-alt"
          title: "Supported Languages"
          content: |
            * English
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Rewriter Cloud supports a number of document formats including almost all common business document file formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: DOC, DOCX, DOCM
                
        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **PDF**
        


      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Rewriter Cloud for cURL - some of the supported languages and platforms.
      
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
    title: "Advanced Rewriter REST API Features"

    feature:
      # feature loop
      - icon: "fas fa-language"
        content: "Supports English language paraphrasing"

      # feature loop
      - icon: "fas fa-copy"
        content: "Paraphrasing of Word documents"

      # feature loop
      - icon: "fas fa-file-alt"
        content: "Paraphrasing of PDF documents"
      
      # feature loop
      - icon: "fas fa-copy"
        content: "Plain text rewriting"
        
      # feature loop
      - icon: "fas fa-lock"
        content: "APIs are secured and require authentication"
        
      # feature loop
      - icon: "fas fa-list"
        content: "API explorer based on swagger collection"
    
    more_feature:
      # more_feature_loop
      - title: "Any Language, Platform and Storage Service Provider"
        content: "GroupDocs.Rewriter for Cloud is a REST based API that can easily be integrated with any language or platform, capable to manage HTTP requests and responses. It supports all popular cloud storage services such as Google Cloud, Drive, DropBox and Amazon S3 to interact without any dependencies. "

      # more_feature_loop
      - title: "Rewrite Word document - cURL"
        content: |
          
          
          ```shell
          //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
          curl -X POST "https://api.groupdocs.cloud/v1.0/rewriter/document" \
          -H "Authorization: Bearer TOKEN" \
          -H "Content-Type: application/json" \
          -d "'[{\"format\": \"docx\", \"language\": \"en\", \"name\": \"test.docx\", \"folder\": \"\", \"savepath\": \"\", \"savefile\": \"rewrited.docx\", \"storage\": \"First Storage\"}]'"

          and response

          {
              "status": "ok",
              "message": "word file saved successfully"
          }
          ```
      # more_feature_loop
      - title: "Quick Start with Document Paraphrasing REST API"
        content: "GroupDocs.Rewriter Cloud API comes with detailed developer guides and live code examples for all major programming languages to start working with API features in no time. Simply create a free account at GroupDocs Cloud, get APP SID & Key information to communicate with GroupDocs Cloud API and you are ready to make an API request on any platform using cURL commands or the SDKs of your choice."

      # more_feature_loop
      - title: "Rewrite plain text - cURL"
        content: |
          
          
          ```shell
            //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
            curl -X POST "https://api.groupdocs.cloud/v1.0/rewriter/text" \
            -H "Authorization: Bearer TOKEN" \
            -H "Content-Type: application/json" \
            -d "'[{\"language\": \"en-fr\", \"text\": \"The client’s mission is to make the world a healthier place and to make traveling and visiting public places safer and more comfortable for people.\"}]'"

            //and response

            {
                "status": "ok",
                "message": "Text rewrited successfully",
                "result": "The mission of the client is to make travel and visiting public spaces safer and more convenient for people."
            }
          ```
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Rewriter Cloud also offers individual document paraphrasing SDKs for other popular languages as listed below:"

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
          

############################# Back to top ###############################
back_to_top:
  enable: true
---