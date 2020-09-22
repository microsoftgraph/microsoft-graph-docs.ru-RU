---
title: Тип ресурса Нетворклокатиондетаил
description: Предоставляет имя и тип сети, из которой пользователь выполнил вход.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 210201613a2f93c99472b42c5ea3ef231a10125d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026609"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="c59ef-103">Тип ресурса Нетворклокатиондетаил</span><span class="sxs-lookup"><span data-stu-id="c59ef-103">networkLocationDetail resource type</span></span>

<span data-ttu-id="c59ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c59ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c59ef-105">Предоставляет имя и тип сети, из которой пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="c59ef-105">Provides the name and type of network from which the user signed in.</span></span>

## <a name="properties"></a><span data-ttu-id="c59ef-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c59ef-106">Properties</span></span>

| <span data-ttu-id="c59ef-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c59ef-107">Property</span></span>     | <span data-ttu-id="c59ef-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c59ef-108">Type</span></span>        | <span data-ttu-id="c59ef-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c59ef-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c59ef-110">нетворкнамес</span><span class="sxs-lookup"><span data-stu-id="c59ef-110">networkNames</span></span>|<span data-ttu-id="c59ef-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c59ef-111">String collection</span></span>|<span data-ttu-id="c59ef-112">Предоставляет имя сети, используемой при входе.</span><span class="sxs-lookup"><span data-stu-id="c59ef-112">Provides the name of the network used when signing in.</span></span>|
|<span data-ttu-id="c59ef-113">нетворктипе</span><span class="sxs-lookup"><span data-stu-id="c59ef-113">networkType</span></span>|<span data-ttu-id="c59ef-114">нетворктипе</span><span class="sxs-lookup"><span data-stu-id="c59ef-114">networkType</span></span>| <span data-ttu-id="c59ef-115">Предоставляет тип сети, используемой при входе.</span><span class="sxs-lookup"><span data-stu-id="c59ef-115">Provides the type of network used when signing in.</span></span> <span data-ttu-id="c59ef-116">Возможные значения: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c59ef-116">Possible values are: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c59ef-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c59ef-117">JSON representation</span></span>

<span data-ttu-id="c59ef-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c59ef-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail",
  "baseType": null
}-->

```json
{
  "networkNames": ["String"],
  "networkType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

