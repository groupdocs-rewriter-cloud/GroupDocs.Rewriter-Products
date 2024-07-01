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
head_title: "Paraphrase, simplify, summarize texts and documents in your .NET applications"
head_description: "Create .NET applications based on GroupDocs.Rewriter API focusing on business logic rather than the technical details."

############################# Header ############################
title: ".NET Cloud SDK for document paraphrasing, summarization and simplification"
description: "Create .NET applications based on GroupDocs.Rewriter API focusing on business logic rather than the technical details."
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
      GroupDocs.Rewriter is an easy-to-use and versatile online service for summarizing, rephrasing or simplifying the texts with full preservation of the meaning. Its advanced AI reads and understands the text and then rephrases it in various wordings, providing a plagiarism-free result without losing the original meaning. While the background process is very complex and resource-intensive, you do not have to worry about formulas, machine learning, and load – our cloud services do all the work.

      This SDK greatly simplifies the interaction of .NET code with GroupDocs.Rewriter Cloud services, allowing you to focus on business logic rather than the technical details. It handles all the routine operations such as establishing connections, sending API requests, and parsing responses, wrapping all these tasks into a few simple methods that can be used in any .NET application. The .NET SDK, demo applications, documentation, and examples are open source distributed under the MIT license. You can use them for any purpose and change any part of the code.
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
            * Compare
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
          GroupDocs.Rewriter Cloud for .NET works on any device or platform with Internet connection
      
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
        content: "GroupDocs.Rewriter Cloud API for .NET comes with detailed developer guides and live code examples for all major programming languages to start working with paraphrasing features in no time. Simply create a free account at GroupDocs Cloud, get APP SID & Key information to communicate with GroupDocs Cloud API and you are ready to use the SDK."

      # more_feature_loop
      - title: "Any language, platform and storage service provider"
        content: "GroupDocs.Rewriter Cloud is a REST API that can easily be integrated with any language or platform, capable to manage HTTP requests and responses. It supports all popular cloud storage services such as Google Cloud, Drive, DropBox and Amazon S3 to interact without any dependencies."

      # more_feature_loop
      - title: "Rewrite plain text - .NET"
        content: |
          
          
          ```cs
            using GroupDocs.Rewriter.Cloud.Sdk.Api;
            using GroupDocs.Rewriter.Cloud.Sdk.Client;
            using GroupDocs.Rewriter.Cloud.Sdk.Client.Auth;
            using GroupDocs.Rewriter.Cloud.Sdk.Model;
            using Configuration = GroupDocs.Rewriter.Cloud.Sdk.Client.Configuration;
            using System.Diagnostics;
            using System.IO;
            using System.Collections.Generic;
            using System.Net.Http;
            using HttpStatusCode = System.Net.HttpStatusCode;
            namespace GroupDocs.Rewriter.Cloud.Sdk
            {
                public class TextRewriter
                {
                    public TextRewriter()
                    {
                        string apiPath = "https://api.groupdocs.cloud/v2.0/rewriter";
                        string clientId = "YOUR_CLIENT_ID";
                        string clientSecret = "YOUR_CLIENT_SECRET";
                        Configuration conf = new Configuration();
                        conf.BasePath = apiPath;
                        conf.OAuthClientId = clientId;
                        conf.OAuthClientSecret = clientSecret;
                        conf.OAuthFlow = OAuthFlow.APPLICATION;
                        ParaphraseApi api = new ParaphraseApi(conf);
                        string srcText = "YOUR_TEXT";
                        ParaphraseTextResponse textResponse = new ParaphraseTextResponse();
                        ParaphraseTextRequest req = new ParaphraseTextRequest(
                            language: sourceLanguage,
                            text: srcText,
                            suggestions: ParaphraseTextRequest.SuggestionsEnum.One,
                            diversityDegree: DegreeEnum.Off);
                        StatusResponse responseId = await api.ParaphraseTextPostAsync(req);
                        try
                        {
                            if (responseId.Status.ToString() == "Accepted")
                            {
                                while(true)
                                {
                                    textResponse = await api.ParaphraseTextRequestIdGetAsync(responseId.Id);
                                    if (textResponse.Status.ToString() == "OK")
                                    {
                                        Console.WriteLine("Plain text paraphrasing: " + textResponse.ParaphraseReult);
                                        break;
                                    }
                                    else
                                         Thread.Sleep(2000);
                                }
                            }
                            else
                            {
                                textResponse = new ParaphraseTextResponse() { Status = responseId.Status, Message = responseId.Message };
                                Console.WriteLine("Text error: " + textResponse.Message);
                            }
                        }
                        catch (Exception ex)
                        {
                            Console.WriteLine("Text exception: " + ex.ToString());
                        }
                    }
                }
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