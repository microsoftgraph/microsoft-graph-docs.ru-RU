---
title: Тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d17ce96d1f714845d07bee3505a28d5a4e7e3978
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130248"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="1c04a-103">Тип ресурса informationalUrl</span><span class="sxs-lookup"><span data-stu-id="1c04a-103">informationalUrl resource type</span></span>

<span data-ttu-id="1c04a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c04a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c04a-105">Основные сведения о профиле приложения.</span><span class="sxs-lookup"><span data-stu-id="1c04a-105">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="1c04a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c04a-106">Properties</span></span>

| <span data-ttu-id="1c04a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c04a-107">Property</span></span> | <span data-ttu-id="1c04a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1c04a-108">Type</span></span> | <span data-ttu-id="1c04a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1c04a-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1c04a-110">logoUrl</span><span class="sxs-lookup"><span data-stu-id="1c04a-110">logoUrl</span></span>|<span data-ttu-id="1c04a-111">Строка</span><span class="sxs-lookup"><span data-stu-id="1c04a-111">String</span></span>|<span data-ttu-id="1c04a-112">URL-адрес CDN для логотипа приложения, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c04a-112">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="1c04a-113">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="1c04a-113">marketingUrl</span></span>|<span data-ttu-id="1c04a-114">Строка</span><span class="sxs-lookup"><span data-stu-id="1c04a-114">String</span></span>| <span data-ttu-id="1c04a-115">Ссылка на страницу маркетинга приложения.</span><span class="sxs-lookup"><span data-stu-id="1c04a-115">Link to the application's marketing page.</span></span> <span data-ttu-id="1c04a-116">Пример: https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="1c04a-116">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="1c04a-117">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="1c04a-117">privacyStatementUrl</span></span>|<span data-ttu-id="1c04a-118">Строка</span><span class="sxs-lookup"><span data-stu-id="1c04a-118">String</span></span>| <span data-ttu-id="1c04a-119">Ссылка на заявление о конфиденциальности приложения.</span><span class="sxs-lookup"><span data-stu-id="1c04a-119">Link to the application's privacy statement.</span></span> <span data-ttu-id="1c04a-120">Пример: https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="1c04a-120">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="1c04a-121">supportUrl</span><span class="sxs-lookup"><span data-stu-id="1c04a-121">supportUrl</span></span>|<span data-ttu-id="1c04a-122">Строка</span><span class="sxs-lookup"><span data-stu-id="1c04a-122">String</span></span>| <span data-ttu-id="1c04a-123">Ссылка на страницу поддержки приложения.</span><span class="sxs-lookup"><span data-stu-id="1c04a-123">Link to the application's support page.</span></span> <span data-ttu-id="1c04a-124">Пример: https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="1c04a-124">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="1c04a-125">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="1c04a-125">termsOfServiceUrl</span></span>|<span data-ttu-id="1c04a-126">Строка</span><span class="sxs-lookup"><span data-stu-id="1c04a-126">String</span></span>| <span data-ttu-id="1c04a-127">Ссылка на заявление об условиях обслуживания приложения.</span><span class="sxs-lookup"><span data-stu-id="1c04a-127">Link to the application's terms of service statement.</span></span> <span data-ttu-id="1c04a-128">Пример: https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="1c04a-128">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1c04a-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1c04a-129">JSON representation</span></span>
<span data-ttu-id="1c04a-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c04a-130">Here is a JSON representation of the resource.</span></span>

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


