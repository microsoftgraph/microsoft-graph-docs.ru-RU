---
title: Тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 31a8096ebe5cb8aecba56a1a6f6c6367adf4b7af
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054877"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="62336-103">Тип ресурса informationalUrl</span><span class="sxs-lookup"><span data-stu-id="62336-103">informationalUrl resource type</span></span>

<span data-ttu-id="62336-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62336-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62336-105">Основные сведения о профиле приложения.</span><span class="sxs-lookup"><span data-stu-id="62336-105">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="62336-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="62336-106">Properties</span></span>

| <span data-ttu-id="62336-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="62336-107">Property</span></span> | <span data-ttu-id="62336-108">Тип</span><span class="sxs-lookup"><span data-stu-id="62336-108">Type</span></span> | <span data-ttu-id="62336-109">Описание</span><span class="sxs-lookup"><span data-stu-id="62336-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="62336-110">logoUrl</span><span class="sxs-lookup"><span data-stu-id="62336-110">logoUrl</span></span>|<span data-ttu-id="62336-111">String</span><span class="sxs-lookup"><span data-stu-id="62336-111">String</span></span>|<span data-ttu-id="62336-112">URL-адрес сети CDN для логотипа приложения и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62336-112">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="62336-113">маркетингурл</span><span class="sxs-lookup"><span data-stu-id="62336-113">marketingUrl</span></span>|<span data-ttu-id="62336-114">String</span><span class="sxs-lookup"><span data-stu-id="62336-114">String</span></span>| <span data-ttu-id="62336-115">Ссылка на маркетинговую страницу приложения.</span><span class="sxs-lookup"><span data-stu-id="62336-115">Link to the application's marketing page.</span></span> <span data-ttu-id="62336-116">Пример: https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="62336-116">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="62336-117">привацистатементурл</span><span class="sxs-lookup"><span data-stu-id="62336-117">privacyStatementUrl</span></span>|<span data-ttu-id="62336-118">String</span><span class="sxs-lookup"><span data-stu-id="62336-118">String</span></span>| <span data-ttu-id="62336-119">Ссылка на заявление о конфиденциальности приложения.</span><span class="sxs-lookup"><span data-stu-id="62336-119">Link to the application's privacy statement.</span></span> <span data-ttu-id="62336-120">Пример: https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="62336-120">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="62336-121">supportUrl</span><span class="sxs-lookup"><span data-stu-id="62336-121">supportUrl</span></span>|<span data-ttu-id="62336-122">String</span><span class="sxs-lookup"><span data-stu-id="62336-122">String</span></span>| <span data-ttu-id="62336-123">Ссылка на страницу поддержки приложения.</span><span class="sxs-lookup"><span data-stu-id="62336-123">Link to the application's support page.</span></span> <span data-ttu-id="62336-124">Пример: https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="62336-124">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="62336-125">термсофсервицеурл</span><span class="sxs-lookup"><span data-stu-id="62336-125">termsOfServiceUrl</span></span>|<span data-ttu-id="62336-126">String</span><span class="sxs-lookup"><span data-stu-id="62336-126">String</span></span>| <span data-ttu-id="62336-127">Ссылка на условия заявления приложения.</span><span class="sxs-lookup"><span data-stu-id="62336-127">Link to the application's terms of service statement.</span></span> <span data-ttu-id="62336-128">Пример: https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="62336-128">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="62336-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62336-129">JSON representation</span></span>
<span data-ttu-id="62336-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62336-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "logoUrl": "String",
  "marketingUrl": "String",
  "privacyStatementUrl": "String",
  "supportUrl": "String",
  "termsOfServiceUrl": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

