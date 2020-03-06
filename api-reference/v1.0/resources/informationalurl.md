---
title: Тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ebf2a79931936e8f45f93cba46b1fefdbf0163b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532881"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="7e626-103">Тип ресурса informationalUrl</span><span class="sxs-lookup"><span data-stu-id="7e626-103">informationalUrl resource type</span></span>

<span data-ttu-id="7e626-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e626-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e626-105">Основные сведения о профиле приложения.</span><span class="sxs-lookup"><span data-stu-id="7e626-105">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="7e626-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e626-106">Properties</span></span>

| <span data-ttu-id="7e626-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e626-107">Property</span></span> | <span data-ttu-id="7e626-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7e626-108">Type</span></span> | <span data-ttu-id="7e626-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7e626-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7e626-110">logoUrl</span><span class="sxs-lookup"><span data-stu-id="7e626-110">logoUrl</span></span>|<span data-ttu-id="7e626-111">Строка</span><span class="sxs-lookup"><span data-stu-id="7e626-111">String</span></span>|<span data-ttu-id="7e626-112">URL-адрес сети CDN для логотипа приложения и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7e626-112">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="7e626-113">маркетингурл</span><span class="sxs-lookup"><span data-stu-id="7e626-113">marketingUrl</span></span>|<span data-ttu-id="7e626-114">Строка</span><span class="sxs-lookup"><span data-stu-id="7e626-114">String</span></span>| <span data-ttu-id="7e626-115">Ссылка на маркетинговую страницу приложения.</span><span class="sxs-lookup"><span data-stu-id="7e626-115">Link to the application's marketing page.</span></span> <span data-ttu-id="7e626-116">Пример: https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="7e626-116">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="7e626-117">привацистатементурл</span><span class="sxs-lookup"><span data-stu-id="7e626-117">privacyStatementUrl</span></span>|<span data-ttu-id="7e626-118">Строка</span><span class="sxs-lookup"><span data-stu-id="7e626-118">String</span></span>| <span data-ttu-id="7e626-119">Ссылка на заявление о конфиденциальности приложения.</span><span class="sxs-lookup"><span data-stu-id="7e626-119">Link to the application's privacy statement.</span></span> <span data-ttu-id="7e626-120">Пример: https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="7e626-120">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="7e626-121">supportUrl</span><span class="sxs-lookup"><span data-stu-id="7e626-121">supportUrl</span></span>|<span data-ttu-id="7e626-122">Строка</span><span class="sxs-lookup"><span data-stu-id="7e626-122">String</span></span>| <span data-ttu-id="7e626-123">Ссылка на страницу поддержки приложения.</span><span class="sxs-lookup"><span data-stu-id="7e626-123">Link to the application's support page.</span></span> <span data-ttu-id="7e626-124">Пример: https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="7e626-124">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="7e626-125">термсофсервицеурл</span><span class="sxs-lookup"><span data-stu-id="7e626-125">termsOfServiceUrl</span></span>|<span data-ttu-id="7e626-126">Строка</span><span class="sxs-lookup"><span data-stu-id="7e626-126">String</span></span>| <span data-ttu-id="7e626-127">Ссылка на условия заявления приложения.</span><span class="sxs-lookup"><span data-stu-id="7e626-127">Link to the application's terms of service statement.</span></span> <span data-ttu-id="7e626-128">Пример: https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="7e626-128">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7e626-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e626-129">JSON representation</span></span>
<span data-ttu-id="7e626-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e626-130">Here is a JSON representation of the resource.</span></span>

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
