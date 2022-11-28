---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Rewriter"
product_tag: "rewriter"
platform: "Python"
platform_tag: "python"

############################# Head ############################
head_title: "Paraphrase content and documents in your Python applications"
head_description: "Create cross-platform data science, AI, and automation solutions in Python based on GroupDocs.Rewriter API. Focus on business logic rather than the technical details."

############################# Header ############################
title: "Python Cloud SDK for document paraphrasing"
description: "Create cross-platform data science, AI, and automation solutions in Python based on GroupDocs.Rewriter API. Focus on business logic rather than the technical details."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Rewriter Cloud SDK for Python"
        image: "/sdk/272x272/groupdocs_rewriter-for-net.png"
        product: "GroupDocs.Rewriter"
        platform: "Python"

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
      GroupDocs.Rewriter is an easy-to-use and versatile online service for rephrasing the texts with full preservation of the meaning. Its advanced AI reads and understands the text and then rephrases it in various wordings, providing a plagiarism-free result without losing the original meaning. While the background process is very complex and resource-intensive, you do not have to worry about formulas, machine learning, and load – our cloud services do all the work.

      This SDK greatly simplifies the interaction with GroupDocs.Rewriter Cloud services from Python code, allowing you to focus on business logic rather than the technical details. It handles all the routine operations such as establishing connections, sending API requests, and parsing responses, wrapping all these tasks into a few simple methods that can be used in any Python application or workbook. The Python SDK, demo applications, documentation, and examples are open source distributed under the MIT license. You can use them for any purpose and change any part of the code.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Main capabilities of GroupDocs.Rewriter Cloud
      
        left:
          enable: true
          icon: "fas fa-crop"
          title: "Supported content"
          content: |
            * Plain text
            * Microsoft Office
            * OpenOffice
            * PDF
        right:
          enable: true
          icon: "fas fa-file-alt"
          title: "Supported languages"
          content: |
            * Arabic
            * English
            * Russian
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
          GroupDocs.Rewriter Cloud for Python works on any device or platform with Internet connection
      
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
    title: "Advanced Document Rewriting REST API Features"

    feature:
      # feature loop
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
      - title: "Quick start with document rewriting REST API"
        content: "GroupDocs.Rewriter Cloud API for Python comes with detailed developer guides and live code examples for all major programming languages to start working with API features in no time. Simply create a free account at GroupDocs Cloud, get APP SID & Key information to communicate with GroupDocs Cloud API and you are ready to use the SDK."

      # more_feature_loop
      - title: "Rewrite Word document - Python"
        content: |
          
          
          ```cs
            //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).

            public FileResponse RewriteDocument(Configuration conf)
            {    
                string name = "test.docx";
                string folder = "";
                string language = "en";
                string format = "docx";
                string storage = "First Storage";
                string saveFile = "translation.docx";
                string savePath = "";
                
                RewriterApi api = new RewriterApi(conf);
                RewriteDocumentRequest request = api.CreateDocumentRequest(name, folder, language, format, storage, saveFile, savePath, masters, elements);
                FileResponse response = api.RunRewritingTask(request);
                return response;
            }
          ```
      # more_feature_loop
      - title: "Any language, platform and storage service provider"
        content: "GroupDocs.Rewriter Cloud is a REST based API that can easily be integrated with any language or platform, capable to manage HTTP requests and responses. It supports all popular cloud storage services such as Google Cloud, Drive, DropBox and Amazon S3 to interact without any dependencies."

      # more_feature_loop
      - title: "Rewrite plain text - Python"
        content: |
          
          
          ```cs
            //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).

            public TextResponse TranslateText(Configuration conf)
            {
                string language = "en";
                string text = "The client’s mission is to make the world a healthier place and to make traveling and visiting public places safer and more comfortable for people.";
                
                RewriterApi api = new RewriterApi(conf);
                RewriteTextRequest request = api.CreateTextRequest(language, text);
                TextResponse response = api.RunRewritingTextTask(request);
                return response;
            }
          ```
      # more_feature_loop
      - title: "Security and Authentication"
        content: "The GroupDocs.Rewriter Cloud API is SSL secured and the authentication requests require a signature and AppSID query parameters or OAuth 2.0 authorization header."
      

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