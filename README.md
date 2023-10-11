# WAF20 - Secure a development lifecycle

**NOTE:** 
This content below is supposed to be part of the WAF 20 document, to be embedded in the chapter "Recommendations>SE02:Secure a development lifecycle".
https://review.learn.microsoft.com/en-us/azure/well-architected/security/secure-development-lifecycle?branch=collab-waf-2-0-1

## Intro / Use case
Let's consider the below use case (diagram) and WAF baseline to demonstrate and explain how Microsoft recommends you build a **Secure Development Lifecycle**.

In this use case, we are considering an IT environment, the reference presented in the chapter "Baseline" (add a link here).



To explain the recommendations to have a Secure development lifecycle, let's consider the following:

1. Developers, being external or internal, may access a couple of Azure services including the Azure DevOps portal. So, Developers are potential threat actors, mainly if they have their credentials stolen.
2. Once Developers have a draft version of the App, Tester users will have access to it, so they can test the application, or Security professionals may start penetration tests on the app.
3. Regardless, of the user role, they will be authenticated against Azure AD, in case the app developed works with OAuth, other than, they will be authenticated against ADDS (Kerberos).
4. Depends on the number and type of resources the solution (apps) are being developed, but they may contain different types of Azure resources or on-premises resources. So, Developers and Testers may continue being a possible threat if you don't protect your environment. That is the reason, you may continue considering different security services, even during the development lifecycle.

This chapter will describe below important security recommendations to make your development lifecycle more secure including not only security solutions but best practices and behaviors that will help you have a development journey with security in mind.

Developers and Tester users will have additional layers of protection, so their credentials may not be stolen by anonymous hackers. Many solutions that may add additional protection to the secure development lifecycle will be described in the other Recommended sessions in this document.

**From this point, we would add the document draft that is already written**
