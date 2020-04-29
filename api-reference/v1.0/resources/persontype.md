---
title: тип ресурса personType
description: Представляет тип пользователя.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 9b6dc5153fb12f44abad57d1977024675aa0bd45
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447194"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="b8dda-103">тип ресурса personType</span><span class="sxs-lookup"><span data-stu-id="b8dda-103">personType resource type</span></span>

<span data-ttu-id="b8dda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8dda-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8dda-105">Представляет тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8dda-105">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b8dda-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8dda-106">JSON representation</span></span>

<span data-ttu-id="b8dda-107">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8dda-107">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b8dda-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8dda-108">Properties</span></span>
| <span data-ttu-id="b8dda-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8dda-109">Property</span></span>     | <span data-ttu-id="b8dda-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b8dda-110">Type</span></span>   |<span data-ttu-id="b8dda-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b8dda-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8dda-112">класс</span><span class="sxs-lookup"><span data-stu-id="b8dda-112">class</span></span>|<span data-ttu-id="b8dda-113">String</span><span class="sxs-lookup"><span data-stu-id="b8dda-113">String</span></span>|<span data-ttu-id="b8dda-114">Тип источника данных, например Person.</span><span class="sxs-lookup"><span data-stu-id="b8dda-114">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="b8dda-115">subclass</span><span class="sxs-lookup"><span data-stu-id="b8dda-115">subclass</span></span>|<span data-ttu-id="b8dda-116">String</span><span class="sxs-lookup"><span data-stu-id="b8dda-116">String</span></span>|<span data-ttu-id="b8dda-117">Дополнительный тип источника данных, например OrganizationUser.</span><span class="sxs-lookup"><span data-stu-id="b8dda-117">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
