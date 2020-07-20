---
title: Тип ресурса Верифиедкустомдомаинцертификатесметадата
description: Представляет настраиваемые метаданные сертификат для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4268c7d9faba8e744f7a6bd6a674ff680cb24346
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556440"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a><span data-ttu-id="0144c-103">Тип ресурса Верифиедкустомдомаинцертификатесметадата</span><span class="sxs-lookup"><span data-stu-id="0144c-103">verifiedCustomDomainCertificatesMetadata resource type</span></span>

<span data-ttu-id="0144c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0144c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0144c-105">Представляет метаданные пользовательских сертификатов домена для ресурса [онпремисеспублишинг](onpremisespublishing.md) при публикации локального приложения с помощью прокси приложения.</span><span class="sxs-lookup"><span data-stu-id="0144c-105">Represents the custom domain certificate metadata for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Application Proxy.</span></span> <span data-ttu-id="0144c-106">Использование пользовательского домена позволяет использовать собственное доменное имя вместо домена по умолчанию (msappproxy.net) для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="0144c-106">Using a custom domain allows you to use your own domain name instead of the default domain, msappproxy.net, for your application.</span></span> <span data-ttu-id="0144c-107">Дополнительные сведения см. в разделе " [Настраиваемые домены" прокси-сервера приложений Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).</span><span class="sxs-lookup"><span data-stu-id="0144c-107">To learn more see, [Custom domains in Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).</span></span>

## <a name="properties"></a><span data-ttu-id="0144c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0144c-108">Properties</span></span>

| <span data-ttu-id="0144c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0144c-109">Property</span></span>     | <span data-ttu-id="0144c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0144c-110">Type</span></span>        | <span data-ttu-id="0144c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0144c-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0144c-112">експиридате</span><span class="sxs-lookup"><span data-stu-id="0144c-112">expiryDate</span></span>|<span data-ttu-id="0144c-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0144c-113">DateTimeOffset</span></span>| <span data-ttu-id="0144c-114">Дата истечения срока действия сертификата настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="0144c-114">The expiry date of the custom domain certificate.</span></span> <span data-ttu-id="0144c-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0144c-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0144c-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0144c-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="0144c-117">иссуедате</span><span class="sxs-lookup"><span data-stu-id="0144c-117">issueDate</span></span>|<span data-ttu-id="0144c-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0144c-118">DateTimeOffset</span></span>| <span data-ttu-id="0144c-119">Дата выпуска настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="0144c-119">The issue date of the custom domain.</span></span> <span data-ttu-id="0144c-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0144c-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0144c-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0144c-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="0144c-122">иссуернаме</span><span class="sxs-lookup"><span data-stu-id="0144c-122">issuerName</span></span>|<span data-ttu-id="0144c-123">String</span><span class="sxs-lookup"><span data-stu-id="0144c-123">String</span></span>| <span data-ttu-id="0144c-124">Имя поставщика сертификата настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="0144c-124">The issuer name of the custom domain certificate.</span></span> |
|<span data-ttu-id="0144c-125">subjectName</span><span class="sxs-lookup"><span data-stu-id="0144c-125">subjectName</span></span>|<span data-ttu-id="0144c-126">String</span><span class="sxs-lookup"><span data-stu-id="0144c-126">String</span></span>| <span data-ttu-id="0144c-127">Имя субъекта пользовательского сертификата домена.</span><span class="sxs-lookup"><span data-stu-id="0144c-127">The subject name of the custom domain certificate.</span></span> |
|<span data-ttu-id="0144c-128">отпечаток</span><span class="sxs-lookup"><span data-stu-id="0144c-128">thumbprint</span></span>|<span data-ttu-id="0144c-129">String</span><span class="sxs-lookup"><span data-stu-id="0144c-129">String</span></span>| <span data-ttu-id="0144c-130">Отпечаток, связанный с пользовательским сертификатом домена.</span><span class="sxs-lookup"><span data-stu-id="0144c-130">The thumbprint associated with the custom domain certificate.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0144c-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0144c-131">JSON representation</span></span>

<span data-ttu-id="0144c-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0144c-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata",
  "baseType": null
}-->

```json
{
  "expiryDate": "String (timestamp)",
  "issueDate": "String (timestamp)",
  "issuerName": "String",
  "subjectName": "String",
  "thumbprint": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedCustomDomainCertificatesMetadata resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->