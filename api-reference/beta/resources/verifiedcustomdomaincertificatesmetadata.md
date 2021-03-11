---
title: verifiedCustomDomainCertificatesMetadata resource type
description: Представляет настраиваемые метаданные сертификации для локального приложения, опубликованного с помощью прокси-сервера приложения.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: eab6823bdd3ed6a822cbeabdebf0aedfb654b769
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721434"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a><span data-ttu-id="c43d7-103">verifiedCustomDomainCertificatesMetadata resource type</span><span class="sxs-lookup"><span data-stu-id="c43d7-103">verifiedCustomDomainCertificatesMetadata resource type</span></span>

<span data-ttu-id="c43d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c43d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c43d7-105">Представляет настраиваемые метаданные сертификата домена для ресурса [onPremisesPublishing](onpremisespublishing.md) при публикации локального приложения с помощью прокси-приложения.</span><span class="sxs-lookup"><span data-stu-id="c43d7-105">Represents the custom domain certificate metadata for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Application Proxy.</span></span> <span data-ttu-id="c43d7-106">Использование настраиваемого домена позволяет использовать собственное доменное имя вместо домена по умолчанию, msappproxy.net, для приложения.</span><span class="sxs-lookup"><span data-stu-id="c43d7-106">Using a custom domain allows you to use your own domain name instead of the default domain, msappproxy.net, for your application.</span></span> <span data-ttu-id="c43d7-107">Дополнительные дополнительные новости см. в [специально созданных доменах в Прокси-сервере приложений Azure AD.](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain)</span><span class="sxs-lookup"><span data-stu-id="c43d7-107">To learn more see, [Custom domains in Azure AD Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).</span></span>

## <a name="properties"></a><span data-ttu-id="c43d7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c43d7-108">Properties</span></span>

| <span data-ttu-id="c43d7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c43d7-109">Property</span></span>     | <span data-ttu-id="c43d7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c43d7-110">Type</span></span>        | <span data-ttu-id="c43d7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c43d7-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c43d7-112">expiryDate</span><span class="sxs-lookup"><span data-stu-id="c43d7-112">expiryDate</span></span>|<span data-ttu-id="c43d7-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c43d7-113">DateTimeOffset</span></span>| <span data-ttu-id="c43d7-114">Срок действия пользовательского сертификата домена.</span><span class="sxs-lookup"><span data-stu-id="c43d7-114">The expiry date of the custom domain certificate.</span></span> <span data-ttu-id="c43d7-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c43d7-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c43d7-116">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c43d7-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
|<span data-ttu-id="c43d7-117">issueDate</span><span class="sxs-lookup"><span data-stu-id="c43d7-117">issueDate</span></span>|<span data-ttu-id="c43d7-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c43d7-118">DateTimeOffset</span></span>| <span data-ttu-id="c43d7-119">Дата выпуска настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="c43d7-119">The issue date of the custom domain.</span></span> <span data-ttu-id="c43d7-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c43d7-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c43d7-121">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c43d7-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
|<span data-ttu-id="c43d7-122">issuerName</span><span class="sxs-lookup"><span data-stu-id="c43d7-122">issuerName</span></span>|<span data-ttu-id="c43d7-123">String</span><span class="sxs-lookup"><span data-stu-id="c43d7-123">String</span></span>| <span data-ttu-id="c43d7-124">Имя эмитента пользовательского сертификата домена.</span><span class="sxs-lookup"><span data-stu-id="c43d7-124">The issuer name of the custom domain certificate.</span></span> |
|<span data-ttu-id="c43d7-125">subjectName</span><span class="sxs-lookup"><span data-stu-id="c43d7-125">subjectName</span></span>|<span data-ttu-id="c43d7-126">String</span><span class="sxs-lookup"><span data-stu-id="c43d7-126">String</span></span>| <span data-ttu-id="c43d7-127">Имя субъекта пользовательского сертификата домена.</span><span class="sxs-lookup"><span data-stu-id="c43d7-127">The subject name of the custom domain certificate.</span></span> |
|<span data-ttu-id="c43d7-128">отпечатки пальцев</span><span class="sxs-lookup"><span data-stu-id="c43d7-128">thumbprint</span></span>|<span data-ttu-id="c43d7-129">String</span><span class="sxs-lookup"><span data-stu-id="c43d7-129">String</span></span>| <span data-ttu-id="c43d7-130">Отпечатки пальцев, связанные с пользовательским сертификатом домена.</span><span class="sxs-lookup"><span data-stu-id="c43d7-130">The thumbprint associated with the custom domain certificate.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c43d7-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c43d7-131">JSON representation</span></span>

<span data-ttu-id="c43d7-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c43d7-132">The following is a JSON representation of the resource.</span></span>

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
