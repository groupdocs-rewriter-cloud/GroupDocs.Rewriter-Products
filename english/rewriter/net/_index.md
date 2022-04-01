---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Rewriter"
product_tag: "rewriter"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET Word & PDF Document Rewriting SDK & REST API"
head_description: ".NET document paraphrasing Cloud SDK & REST API. Rewrite English text and text content of Microsoft Word and PDF documents."

############################# Header ############################
title: ".NET Cloud SDK for Document Rewriting"
description: "Paraphrase plain text and text content from Microsoft Word and PDF documents using documents rewriting Cloud SDK & REST API."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Rewriter Cloud SDK for .NET"
        image: "/sdk/272x272/groupdocs_rewriter-for-net.png"
        product: "GroupDocs.Rewriter"
        platform: ".NET"

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
      GroupDocs.Rewriter Cloud SDK for .NET helps developers to add text and document paraphrasing features in any type of .NET based application without using external software. The API extracts text content from Microsoft Word and PDF documents, uses modern machine learning techniques to efficiently rewrite the on-page contents of Microsoft Word and PDF documents and inserts paraphrased text back to the document.

      GroupDocs.Rewriter Cloud is a true REST API thus offering flexibility to use it with any language or platform that supports REST. It easily integrates with other cloud services to provide an ideal document paraphrasing experience across web, mobile desktop or cloud platforms.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the main features supported by GroupDocs.Rewriter Cloud.
      
        left:
          enable: true
          icon: "fas fa-crop"
          title: "Documents Rewriting"
          content: |
            * Translate Plain Text
            * Translate Word Documents
            * Translate PDF Documents
        right:
          enable: true
          icon: "fas fa-file-alt"
          title: "Supported Languages"
          content: |
            * English
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Rewriter Cloud SDK for .NET supports a number of document formats.

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
          GroupDocs.Rewriter Cloud for .NET - some of the supported languages and platforms.
      
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
      - title: "Quick Start with Document Rewriting REST API"
        content: "GroupDocs.Rewriter Cloud API comes with detailed developer guides and live code examples for all major programming languages to start working with API features in no time. Simply create a free account at GroupDocs Cloud, get APP SID & Key information to communicate with GroupDocs Cloud API and you are ready to make an API request on any platform using cURL commands or the SDKs of your choice."

      # more_feature_loop
      - title: "Rewrite Word document - .NET"
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
      - title: "Any Language, Platform and Storage Service Provider"
        content: "GroupDocs.Rewriter for Cloud is a REST based API that can easily be integrated with any language or platform, capable to manage HTTP requests and responses. It supports all popular cloud storage services such as Google Cloud, Drive, DropBox and Amazon S3 to interact without any dependencies."

      # more_feature_loop
      - title: "Rewrite plain text - .NET"
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
    title: "GroupDocs.Rewriter Cloud also offers document paraphrasing SDKs for other languages as listed below:"

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