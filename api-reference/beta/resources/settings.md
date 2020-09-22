---
title: Тип ресурса settings
description: Текущие необходимые параметры для пользователя для использования API аналитики.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 822ac02be4f3dc5d507aa5d9dbbb2fa22b194b64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033547"
---
# <a name="settings-resource-type"></a><span data-ttu-id="42e46-103">Тип ресурса settings</span><span class="sxs-lookup"><span data-stu-id="42e46-103">settings resource type</span></span>

<span data-ttu-id="42e46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42e46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42e46-105">Представляет текущие обязательные параметры для пользователя с помощью API аналитики.</span><span class="sxs-lookup"><span data-stu-id="42e46-105">Represents the current required settings for a user to use the analytics API.</span></span>

<span data-ttu-id="42e46-106">Чтобы API аналитики возвращал результаты для пользователей, они должны иметь размещенный в облаке почтовый ящик, включенный для Microsoft Graph, имеющий действительную лицензию MyAnalytics и быть участником использования MyAnalytics.</span><span class="sxs-lookup"><span data-stu-id="42e46-106">For the analytics API to return results for users, they must have a cloud-hosted mailbox that’s enabled for Microsoft Graph, have a valid MyAnalytics license, and be opted in to using MyAnalytics.</span></span>

## <a name="methods"></a><span data-ttu-id="42e46-107">Методы</span><span class="sxs-lookup"><span data-stu-id="42e46-107">Methods</span></span>

| <span data-ttu-id="42e46-108">Метод</span><span class="sxs-lookup"><span data-stu-id="42e46-108">Method</span></span>       | <span data-ttu-id="42e46-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="42e46-109">Return Type</span></span> | <span data-ttu-id="42e46-110">Описание</span><span class="sxs-lookup"><span data-stu-id="42e46-110">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="42e46-111">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="42e46-111">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="42e46-112">settings</span><span class="sxs-lookup"><span data-stu-id="42e46-112">settings</span></span>](settings.md) | <span data-ttu-id="42e46-113">Получение следующих параметров свойства для пользователя.</span><span class="sxs-lookup"><span data-stu-id="42e46-113">Get the following property settings for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="42e46-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="42e46-114">Properties</span></span>

| <span data-ttu-id="42e46-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="42e46-115">Property</span></span>     | <span data-ttu-id="42e46-116">Тип</span><span class="sxs-lookup"><span data-stu-id="42e46-116">Type</span></span>        | <span data-ttu-id="42e46-117">Описание</span><span class="sxs-lookup"><span data-stu-id="42e46-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42e46-118">хасграфмаилбокс</span><span class="sxs-lookup"><span data-stu-id="42e46-118">hasGraphMailbox</span></span>|<span data-ttu-id="42e46-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="42e46-119">Boolean</span></span>|<span data-ttu-id="42e46-120">Указывает, размещается ли основной почтовый ящик пользователя в облаке и включено ли для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="42e46-120">Specifies if the user's primary mailbox is hosted in the cloud and is enabled for Microsoft Graph.</span></span>|
|<span data-ttu-id="42e46-121">хаслиценсе</span><span class="sxs-lookup"><span data-stu-id="42e46-121">hasLicense</span></span>|<span data-ttu-id="42e46-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="42e46-122">Boolean</span></span>|<span data-ttu-id="42e46-123">Указывает, назначена ли лицензия MyAnalytics для пользователя.</span><span class="sxs-lookup"><span data-stu-id="42e46-123">Specifies if the user has a MyAnalytics license assigned.</span></span>|
|<span data-ttu-id="42e46-124">хасоптедаут</span><span class="sxs-lookup"><span data-stu-id="42e46-124">hasOptedOut</span></span>|<span data-ttu-id="42e46-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="42e46-125">Boolean</span></span>|<span data-ttu-id="42e46-126">Указывает, выбрал ли пользователь из MyAnalytics.</span><span class="sxs-lookup"><span data-stu-id="42e46-126">Specifies if the user opted out of MyAnalytics.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42e46-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42e46-127">JSON representation</span></span>

<span data-ttu-id="42e46-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42e46-128">The following is a JSON representation of the resource.</span></span>

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

