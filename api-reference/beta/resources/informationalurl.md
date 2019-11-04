---
title: Тип ресурса informationalUrl
description: Основные сведения о профиле приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c8cf7bcc40480042b4cd43230ca0245bd690fd7b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938844"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="9f204-103">Тип ресурса informationalUrl</span><span class="sxs-lookup"><span data-stu-id="9f204-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f204-104">Основные сведения о профиле приложения.</span><span class="sxs-lookup"><span data-stu-id="9f204-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="9f204-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f204-105">Properties</span></span>

| <span data-ttu-id="9f204-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f204-106">Property</span></span> | <span data-ttu-id="9f204-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9f204-107">Type</span></span> | <span data-ttu-id="9f204-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9f204-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9f204-109">logoUrl</span><span class="sxs-lookup"><span data-stu-id="9f204-109">logoUrl</span></span>|<span data-ttu-id="9f204-110">Строка</span><span class="sxs-lookup"><span data-stu-id="9f204-110">String</span></span>|<span data-ttu-id="9f204-111">URL-адрес сети CDN для логотипа приложения и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9f204-111">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="9f204-112">маркетингурл</span><span class="sxs-lookup"><span data-stu-id="9f204-112">marketingUrl</span></span>|<span data-ttu-id="9f204-113">Строка</span><span class="sxs-lookup"><span data-stu-id="9f204-113">String</span></span>| <span data-ttu-id="9f204-114">Ссылка на маркетинговую страницу приложения.</span><span class="sxs-lookup"><span data-stu-id="9f204-114">Link to the application's marketing page.</span></span> <span data-ttu-id="9f204-115">Пример: https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="9f204-115">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="9f204-116">привацистатементурл</span><span class="sxs-lookup"><span data-stu-id="9f204-116">privacyStatementUrl</span></span>|<span data-ttu-id="9f204-117">Строка</span><span class="sxs-lookup"><span data-stu-id="9f204-117">String</span></span>| <span data-ttu-id="9f204-118">Ссылка на заявление о конфиденциальности приложения.</span><span class="sxs-lookup"><span data-stu-id="9f204-118">Link to the application's privacy statement.</span></span> <span data-ttu-id="9f204-119">Пример: https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="9f204-119">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="9f204-120">supportUrl</span><span class="sxs-lookup"><span data-stu-id="9f204-120">supportUrl</span></span>|<span data-ttu-id="9f204-121">Строка</span><span class="sxs-lookup"><span data-stu-id="9f204-121">String</span></span>| <span data-ttu-id="9f204-122">Ссылка на страницу поддержки приложения.</span><span class="sxs-lookup"><span data-stu-id="9f204-122">Link to the application's support page.</span></span> <span data-ttu-id="9f204-123">Пример: https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="9f204-123">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="9f204-124">термсофсервицеурл</span><span class="sxs-lookup"><span data-stu-id="9f204-124">termsOfServiceUrl</span></span>|<span data-ttu-id="9f204-125">Строка</span><span class="sxs-lookup"><span data-stu-id="9f204-125">String</span></span>| <span data-ttu-id="9f204-126">Ссылка на условия заявления приложения.</span><span class="sxs-lookup"><span data-stu-id="9f204-126">Link to the application's terms of service statement.</span></span> <span data-ttu-id="9f204-127">Пример: https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="9f204-127">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f204-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f204-128">JSON representation</span></span>
<span data-ttu-id="9f204-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f204-129">Here is a JSON representation of the resource.</span></span>

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
