---
title: Тип ресурса Верифиедкустомдомаинцертификатесметадата
description: Представляет настраиваемые метаданные сертификат для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4f3dc4cbe1a68ae6f7c751c9b305f95901928d17
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402954"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a><span data-ttu-id="a189b-103">Тип ресурса Верифиедкустомдомаинцертификатесметадата</span><span class="sxs-lookup"><span data-stu-id="a189b-103">verifiedCustomDomainCertificatesMetadata resource type</span></span>

<span data-ttu-id="a189b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a189b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a189b-105">Представляет метаданные пользовательских сертификатов домена для ресурса [онпремисеспублишинг](onpremisespublishing.md) при публикации локального приложения с помощью прокси приложения.</span><span class="sxs-lookup"><span data-stu-id="a189b-105">Represents the custom domain certificate metadata for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Application Proxy.</span></span> <span data-ttu-id="a189b-106">Использование пользовательского домена позволяет использовать собственное доменное имя вместо домена по умолчанию (msappproxy.net) для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="a189b-106">Using a custom domain allows you to use your own domain name instead of the default domain, msappproxy.net, for your application.</span></span> <span data-ttu-id="a189b-107">Дополнительные сведения см. в разделе " [Настраиваемые домены" прокси-сервера приложений Azure AD](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).</span><span class="sxs-lookup"><span data-stu-id="a189b-107">To learn more see, [Custom domains in Azure AD Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).</span></span>

## <a name="properties"></a><span data-ttu-id="a189b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a189b-108">Properties</span></span>

| <span data-ttu-id="a189b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a189b-109">Property</span></span>     | <span data-ttu-id="a189b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a189b-110">Type</span></span>        | <span data-ttu-id="a189b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a189b-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a189b-112">експиридате</span><span class="sxs-lookup"><span data-stu-id="a189b-112">expiryDate</span></span>|<span data-ttu-id="a189b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a189b-113">DateTimeOffset</span></span>| <span data-ttu-id="a189b-114">Дата истечения срока действия сертификата настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="a189b-114">The expiry date of the custom domain certificate.</span></span> <span data-ttu-id="a189b-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a189b-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a189b-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a189b-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="a189b-117">иссуедате</span><span class="sxs-lookup"><span data-stu-id="a189b-117">issueDate</span></span>|<span data-ttu-id="a189b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a189b-118">DateTimeOffset</span></span>| <span data-ttu-id="a189b-119">Дата выпуска настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="a189b-119">The issue date of the custom domain.</span></span> <span data-ttu-id="a189b-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a189b-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a189b-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a189b-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="a189b-122">иссуернаме</span><span class="sxs-lookup"><span data-stu-id="a189b-122">issuerName</span></span>|<span data-ttu-id="a189b-123">String</span><span class="sxs-lookup"><span data-stu-id="a189b-123">String</span></span>| <span data-ttu-id="a189b-124">Имя поставщика сертификата настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="a189b-124">The issuer name of the custom domain certificate.</span></span> |
|<span data-ttu-id="a189b-125">subjectName</span><span class="sxs-lookup"><span data-stu-id="a189b-125">subjectName</span></span>|<span data-ttu-id="a189b-126">String</span><span class="sxs-lookup"><span data-stu-id="a189b-126">String</span></span>| <span data-ttu-id="a189b-127">Имя субъекта пользовательского сертификата домена.</span><span class="sxs-lookup"><span data-stu-id="a189b-127">The subject name of the custom domain certificate.</span></span> |
|<span data-ttu-id="a189b-128">отпечаток</span><span class="sxs-lookup"><span data-stu-id="a189b-128">thumbprint</span></span>|<span data-ttu-id="a189b-129">String</span><span class="sxs-lookup"><span data-stu-id="a189b-129">String</span></span>| <span data-ttu-id="a189b-130">Отпечаток, связанный с пользовательским сертификатом домена.</span><span class="sxs-lookup"><span data-stu-id="a189b-130">The thumbprint associated with the custom domain certificate.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a189b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a189b-131">JSON representation</span></span>

<span data-ttu-id="a189b-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a189b-132">The following is a JSON representation of the resource.</span></span>

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