---
title: Тип ресурса Чанжетраккедентити
description: Представляет сущность для отслеживания изменений, внесенных в любой поддерживаемый ресурс смен
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a167f6409ba972b66f23a3608047b4e72c036846
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951981"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="8a4cd-103">Тип ресурса Чанжетраккедентити</span><span class="sxs-lookup"><span data-stu-id="8a4cd-103">changeTrackedEntity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a4cd-104">Представляет сущность для отслеживания изменений, внесенных в любое поддерживаемое [Расписание](schedule.md) и связанный ресурс.</span><span class="sxs-lookup"><span data-stu-id="8a4cd-104">Represents an entity to track changes made to any supported [schedule](schedule.md) and associated resource.</span></span>

## <a name="properties"></a><span data-ttu-id="8a4cd-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a4cd-105">Properties</span></span>

| <span data-ttu-id="8a4cd-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a4cd-106">Property</span></span>     | <span data-ttu-id="8a4cd-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8a4cd-107">Type</span></span>        | <span data-ttu-id="8a4cd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8a4cd-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a4cd-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a4cd-109">createdDateTime</span></span>|<span data-ttu-id="8a4cd-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a4cd-110">DateTimeOffset</span></span>|<span data-ttu-id="8a4cd-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8a4cd-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8a4cd-113">id</span><span class="sxs-lookup"><span data-stu-id="8a4cd-113">id</span></span>|<span data-ttu-id="8a4cd-114">String</span><span class="sxs-lookup"><span data-stu-id="8a4cd-114">String</span></span>| <span data-ttu-id="8a4cd-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a4cd-115">Read-only.</span></span>|
|<span data-ttu-id="8a4cd-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8a4cd-116">lastModifiedBy</span></span>|[<span data-ttu-id="8a4cd-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="8a4cd-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="8a4cd-118">Идентификатор пользователя, который последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="8a4cd-118">Identity of the person who last modified the entity.</span></span>|
|<span data-ttu-id="8a4cd-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a4cd-119">lastModifiedDateTime</span></span>|<span data-ttu-id="8a4cd-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a4cd-120">DateTimeOffset</span></span>|<span data-ttu-id="8a4cd-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8a4cd-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a4cd-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="8a4cd-123">Relationships</span></span>

<span data-ttu-id="8a4cd-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8a4cd-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a4cd-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8a4cd-125">JSON representation</span></span>

<span data-ttu-id="8a4cd-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a4cd-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeTrackedEntity",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "changeTrackedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
