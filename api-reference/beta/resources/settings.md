---
title: Тип ресурса settings
description: Текущие необходимые параметры для пользователя для использования API аналитики.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a7d534aecf6e7ffa427ea175ae06e2b1820435b2
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450816"
---
# <a name="settings-resource-type"></a><span data-ttu-id="e8c48-103">Тип ресурса settings</span><span class="sxs-lookup"><span data-stu-id="e8c48-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8c48-104">Представляет текущие обязательные параметры для пользователя с помощью API аналитики.</span><span class="sxs-lookup"><span data-stu-id="e8c48-104">Represents the current required settings for a user to use the analytics API.</span></span>

<span data-ttu-id="e8c48-105">Чтобы API аналитики возвращал результаты для пользователей, они должны иметь размещенный в облаке почтовый ящик, включенный для Microsoft Graph, имеющий действительную лицензию MyAnalytics и быть участником использования MyAnalytics.</span><span class="sxs-lookup"><span data-stu-id="e8c48-105">For the analytics API to return results for users, they must have a cloud-hosted mailbox that’s enabled for Microsoft Graph, have a valid MyAnalytics license, and be opted in to using MyAnalytics.</span></span>

## <a name="methods"></a><span data-ttu-id="e8c48-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e8c48-106">Methods</span></span>

| <span data-ttu-id="e8c48-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e8c48-107">Method</span></span>       | <span data-ttu-id="e8c48-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e8c48-108">Return Type</span></span> | <span data-ttu-id="e8c48-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e8c48-109">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="e8c48-110">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="e8c48-110">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="e8c48-111">settings</span><span class="sxs-lookup"><span data-stu-id="e8c48-111">settings</span></span>](settings.md) | <span data-ttu-id="e8c48-112">Получение следующих параметров свойства для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8c48-112">Get the following property settings for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8c48-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8c48-113">Properties</span></span>

| <span data-ttu-id="e8c48-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8c48-114">Property</span></span>     | <span data-ttu-id="e8c48-115">Тип</span><span class="sxs-lookup"><span data-stu-id="e8c48-115">Type</span></span>        | <span data-ttu-id="e8c48-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e8c48-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e8c48-117">хасграфмаилбокс</span><span class="sxs-lookup"><span data-stu-id="e8c48-117">hasGraphMailbox</span></span>|<span data-ttu-id="e8c48-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8c48-118">Boolean</span></span>|<span data-ttu-id="e8c48-119">Указывает, размещается ли основной почтовый ящик пользователя в облаке и включено ли для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e8c48-119">Specifies if the user's primary mailbox is hosted in the cloud and is enabled for Microsoft Graph.</span></span>|
|<span data-ttu-id="e8c48-120">хаслиценсе</span><span class="sxs-lookup"><span data-stu-id="e8c48-120">hasLicense</span></span>|<span data-ttu-id="e8c48-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8c48-121">Boolean</span></span>|<span data-ttu-id="e8c48-122">Указывает, назначена ли лицензия MyAnalytics для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8c48-122">Specifies if the user has a MyAnalytics license assigned.</span></span>|
|<span data-ttu-id="e8c48-123">хасоптедаут</span><span class="sxs-lookup"><span data-stu-id="e8c48-123">hasOptedOut</span></span>|<span data-ttu-id="e8c48-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8c48-124">Boolean</span></span>|<span data-ttu-id="e8c48-125">Указывает, выбрал ли пользователь из MyAnalytics.</span><span class="sxs-lookup"><span data-stu-id="e8c48-125">Specifies if the user opted out of MyAnalytics.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8c48-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8c48-126">JSON representation</span></span>

<span data-ttu-id="e8c48-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8c48-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settings",
  "baseType": null
}-->

```json
{
  "hasGraphMailbox": true,
  "hasLicense": true,
  "hasOptedOut": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->