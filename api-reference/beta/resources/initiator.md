---
title: Тип ресурса инициатора
description: Указывает, кто инициировал событие подготовки.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2846c247d4a0d196d4c620f447b40d47cd486c81
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349454"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="21db7-103">Тип ресурса инициатора</span><span class="sxs-lookup"><span data-stu-id="21db7-103">initiator resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21db7-104">Указывает, кто инициировал событие подготовки.</span><span class="sxs-lookup"><span data-stu-id="21db7-104">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="21db7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="21db7-105">Properties</span></span>

| <span data-ttu-id="21db7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="21db7-106">Property</span></span>     | <span data-ttu-id="21db7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="21db7-107">Type</span></span>        | <span data-ttu-id="21db7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="21db7-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21db7-109">displayName</span><span class="sxs-lookup"><span data-stu-id="21db7-109">displayName</span></span>|<span data-ttu-id="21db7-110">Строка</span><span class="sxs-lookup"><span data-stu-id="21db7-110">String</span></span>|<span data-ttu-id="21db7-111">Имя пользователя или службы, которые инициировали событие подготовки.</span><span class="sxs-lookup"><span data-stu-id="21db7-111">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="21db7-112">id</span><span class="sxs-lookup"><span data-stu-id="21db7-112">id</span></span>|<span data-ttu-id="21db7-113">String</span><span class="sxs-lookup"><span data-stu-id="21db7-113">String</span></span>|<span data-ttu-id="21db7-114">Уникальный идентификатор пользователя или службы, которые инициировали событие подготовки.</span><span class="sxs-lookup"><span data-stu-id="21db7-114">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="21db7-115">Инитиатортипе</span><span class="sxs-lookup"><span data-stu-id="21db7-115">initiatorType</span></span>|<span data-ttu-id="21db7-116">String</span><span class="sxs-lookup"><span data-stu-id="21db7-116">String</span></span>| <span data-ttu-id="21db7-117">Тип инициатора.</span><span class="sxs-lookup"><span data-stu-id="21db7-117">Type of initiator.</span></span> <span data-ttu-id="21db7-118">Возможные значения: `user`, `app`, `system`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="21db7-118">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21db7-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21db7-119">JSON representation</span></span>

<span data-ttu-id="21db7-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21db7-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
