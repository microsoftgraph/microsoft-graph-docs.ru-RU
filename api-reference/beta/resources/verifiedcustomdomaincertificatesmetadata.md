---
title: Тип ресурса verifiedCustomDomainCertificatesMetadata
description: Представляет настраиваемые метаданные сертификата для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: bc0f839d91147f80d41dc48ee53c0f888aa35283
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137594"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a><span data-ttu-id="f4142-103">Тип ресурса verifiedCustomDomainCertificatesMetadata</span><span class="sxs-lookup"><span data-stu-id="f4142-103">verifiedCustomDomainCertificatesMetadata resource type</span></span>

<span data-ttu-id="f4142-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4142-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4142-105">Представляет метаданные сертификата настраиваемого домена для ресурса [onPremisesPublishing](onpremisespublishing.md) при публикации локального приложения с прокси-сервером приложения.</span><span class="sxs-lookup"><span data-stu-id="f4142-105">Represents the custom domain certificate metadata for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Application Proxy.</span></span> <span data-ttu-id="f4142-106">Использование настраиваемого домена позволяет использовать для приложения собственное доменное имя вместо домена по умолчанию msappproxy.net домена.</span><span class="sxs-lookup"><span data-stu-id="f4142-106">Using a custom domain allows you to use your own domain name instead of the default domain, msappproxy.net, for your application.</span></span> <span data-ttu-id="f4142-107">Чтобы узнать больше, [пользовательские домены в прокси приложения Azure AD.](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain)</span><span class="sxs-lookup"><span data-stu-id="f4142-107">To learn more see, [Custom domains in Azure AD Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).</span></span>

## <a name="properties"></a><span data-ttu-id="f4142-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4142-108">Properties</span></span>

| <span data-ttu-id="f4142-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4142-109">Property</span></span>     | <span data-ttu-id="f4142-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f4142-110">Type</span></span>        | <span data-ttu-id="f4142-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f4142-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4142-112">expiryDate</span><span class="sxs-lookup"><span data-stu-id="f4142-112">expiryDate</span></span>|<span data-ttu-id="f4142-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4142-113">DateTimeOffset</span></span>| <span data-ttu-id="f4142-114">Дата окончания срока действия сертификата настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="f4142-114">The expiry date of the custom domain certificate.</span></span> <span data-ttu-id="f4142-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f4142-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4142-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f4142-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="f4142-117">issueDate</span><span class="sxs-lookup"><span data-stu-id="f4142-117">issueDate</span></span>|<span data-ttu-id="f4142-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4142-118">DateTimeOffset</span></span>| <span data-ttu-id="f4142-119">Дата выдачи настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="f4142-119">The issue date of the custom domain.</span></span> <span data-ttu-id="f4142-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f4142-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4142-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f4142-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="f4142-122">issuerName</span><span class="sxs-lookup"><span data-stu-id="f4142-122">issuerName</span></span>|<span data-ttu-id="f4142-123">Строка</span><span class="sxs-lookup"><span data-stu-id="f4142-123">String</span></span>| <span data-ttu-id="f4142-124">Имя issuer сертификата настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="f4142-124">The issuer name of the custom domain certificate.</span></span> |
|<span data-ttu-id="f4142-125">subjectName</span><span class="sxs-lookup"><span data-stu-id="f4142-125">subjectName</span></span>|<span data-ttu-id="f4142-126">String</span><span class="sxs-lookup"><span data-stu-id="f4142-126">String</span></span>| <span data-ttu-id="f4142-127">Имя субъекта пользовательского сертификата домена.</span><span class="sxs-lookup"><span data-stu-id="f4142-127">The subject name of the custom domain certificate.</span></span> |
|<span data-ttu-id="f4142-128">thumbprint</span><span class="sxs-lookup"><span data-stu-id="f4142-128">thumbprint</span></span>|<span data-ttu-id="f4142-129">Строка</span><span class="sxs-lookup"><span data-stu-id="f4142-129">String</span></span>| <span data-ttu-id="f4142-130">Отпечаток, связанный с сертификатом пользовательского домена.</span><span class="sxs-lookup"><span data-stu-id="f4142-130">The thumbprint associated with the custom domain certificate.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f4142-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f4142-131">JSON representation</span></span>

<span data-ttu-id="f4142-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4142-132">The following is a JSON representation of the resource.</span></span>

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
