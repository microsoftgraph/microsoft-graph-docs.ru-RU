---
title: Тип ресурса Йомиперсоннаме
description: Тип ресурса Йомиперсоннаме
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0a598c4b5e999b03aeb7201c6eae3a230d3160a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518975"
---
# <a name="yomipersonname-resource-type"></a><span data-ttu-id="4ffd3-103">Тип ресурса Йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="4ffd3-103">yomiPersonName resource type</span></span>

<span data-ttu-id="4ffd3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ffd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ffd3-105">Предоставляет пользователю способ хранения сведений о том, как произношение имени для несобственных динамиков языка, в котором представлен ресурс [PersonName](personname.md) .</span><span class="sxs-lookup"><span data-stu-id="4ffd3-105">Provides a mechanism for a user to store information about how to pronounce a name for non-native speakers of the language that the [personName](personname.md) resource is represented in.</span></span>

## <a name="properties"></a><span data-ttu-id="4ffd3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ffd3-106">Properties</span></span>

| <span data-ttu-id="4ffd3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ffd3-107">Property</span></span>     | <span data-ttu-id="4ffd3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4ffd3-108">Type</span></span>        | <span data-ttu-id="4ffd3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4ffd3-109">Description</span></span>                                             |
|:-------------|:------------|:--------------------------------------------------------|
|<span data-ttu-id="4ffd3-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4ffd3-110">displayName</span></span>   |<span data-ttu-id="4ffd3-111">String</span><span class="sxs-lookup"><span data-stu-id="4ffd3-111">String</span></span>       | <span data-ttu-id="4ffd3-112">Составные руководства по произношению имени и фамилии.</span><span class="sxs-lookup"><span data-stu-id="4ffd3-112">Composite of first and last name pronunciation guides.</span></span>  |
|<span data-ttu-id="4ffd3-113">первыми</span><span class="sxs-lookup"><span data-stu-id="4ffd3-113">first</span></span>         |<span data-ttu-id="4ffd3-114">String</span><span class="sxs-lookup"><span data-stu-id="4ffd3-114">String</span></span>       | <span data-ttu-id="4ffd3-115">Произношение руководства для первого имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ffd3-115">Pronunciation guide for the first name of the user.</span></span>     |
|<span data-ttu-id="4ffd3-116">Фамили</span><span class="sxs-lookup"><span data-stu-id="4ffd3-116">last</span></span>          |<span data-ttu-id="4ffd3-117">String</span><span class="sxs-lookup"><span data-stu-id="4ffd3-117">String</span></span>       | <span data-ttu-id="4ffd3-118">Произношение руководства для последнего имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ffd3-118">Pronunciation guide for the last name of the user.</span></span>      |
|<span data-ttu-id="4ffd3-119">маиден</span><span class="sxs-lookup"><span data-stu-id="4ffd3-119">maiden</span></span>        |<span data-ttu-id="4ffd3-120">String</span><span class="sxs-lookup"><span data-stu-id="4ffd3-120">String</span></span>       | <span data-ttu-id="4ffd3-121">Произношение руководства для маиден имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ffd3-121">Pronunciation guide for the maiden name of the user.</span></span>    |
|<span data-ttu-id="4ffd3-122">назван</span><span class="sxs-lookup"><span data-stu-id="4ffd3-122">middle</span></span>        |<span data-ttu-id="4ffd3-123">String</span><span class="sxs-lookup"><span data-stu-id="4ffd3-123">String</span></span>       | <span data-ttu-id="4ffd3-124">Произношение руководства по среднему имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ffd3-124">Pronunciation guide for the middle name of the user.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="4ffd3-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ffd3-125">JSON representation</span></span>

<span data-ttu-id="4ffd3-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ffd3-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.yomiPersonName",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "yomiPersonName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
