---
title: тип ресурса applyLabelAction
description: Представляет набор действий, которые необходимо принять для применения или обновления метки.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e53a2796c7cd4f0b8c0a415ca4bc38ffefeb609e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945744"
---
# <a name="applylabelaction-resource-type"></a><span data-ttu-id="e75db-103">тип ресурса applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="e75db-103">applyLabelAction resource type</span></span>

<span data-ttu-id="e75db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e75db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e75db-105">Представляет набор действий, которые необходимо принять для применения или обновления метки.</span><span class="sxs-lookup"><span data-stu-id="e75db-105">Represents a set of actions that should be taken to apply or update a label.</span></span> <span data-ttu-id="e75db-106">**applyLabelAction** возвращается, когда результатом операции оценки меток является применение метки.</span><span class="sxs-lookup"><span data-stu-id="e75db-106">**applyLabelAction** is returned when the result of a label evaluation operation is that a label should be applied.</span></span> <span data-ttu-id="e75db-107">Свойство `actions` содержит [коллекцию informationProtectionAction,](informationProtectionaction.md) в которую описан  полный набор действий для применения метки, включая удаление старых метаданных, маркировку контента и защиту.</span><span class="sxs-lookup"><span data-stu-id="e75db-107">The `actions` property contains an [informationProtectionAction](informationProtectionaction.md) collection that described the full set of actions to *apply* the label, including removal of old metadata, content marking, and protection.</span></span>

## <a name="properties"></a><span data-ttu-id="e75db-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e75db-108">Properties</span></span>

| <span data-ttu-id="e75db-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e75db-109">Property</span></span>                    | <span data-ttu-id="e75db-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e75db-110">Type</span></span>                                                                     | <span data-ttu-id="e75db-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e75db-111">Description</span></span>                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="e75db-112">actionSource</span><span class="sxs-lookup"><span data-stu-id="e75db-112">actionSource</span></span>                | <span data-ttu-id="e75db-113">String</span><span class="sxs-lookup"><span data-stu-id="e75db-113">String</span></span>                                                                   | <span data-ttu-id="e75db-114">Возможные значения: `manual`, `automatic`, `recommended`, `default`.</span><span class="sxs-lookup"><span data-stu-id="e75db-114">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span>                                                                                                                             |
| <span data-ttu-id="e75db-115">actions</span><span class="sxs-lookup"><span data-stu-id="e75db-115">actions</span></span>                     | <span data-ttu-id="e75db-116">[коллекция informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="e75db-116">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="e75db-117">Коллекция определенных действий, которые должно приниматься потреблять приложение для метки документа.</span><span class="sxs-lookup"><span data-stu-id="e75db-117">The collection of specific actions that should be taken by the consuming application to label the document.</span></span> <span data-ttu-id="e75db-118">Полный список см. в списке [informationProtectionAction.](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="e75db-118">See  [informationProtectionAction](informationprotectionaction.md) for the full list.</span></span> |
| <span data-ttu-id="e75db-119">label</span><span class="sxs-lookup"><span data-stu-id="e75db-119">label</span></span>                       | [<span data-ttu-id="e75db-120">labelDetails</span><span class="sxs-lookup"><span data-stu-id="e75db-120">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="e75db-121">Объект, описывая детали метки для применения.</span><span class="sxs-lookup"><span data-stu-id="e75db-121">Object that describes the details of the label to apply.</span></span>                                                                                                                                          |
| <span data-ttu-id="e75db-122">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="e75db-122">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="e75db-123">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="e75db-123">Guid collection</span></span>                                                          | <span data-ttu-id="e75db-124">Если метка была результатом автоматической классификации, введите список GUID-интерфейсов типа конфиденциальной информации, которые привели к возврату метки.</span><span class="sxs-lookup"><span data-stu-id="e75db-124">If the label was the result of an automatic classification, supply the list of sensitive info type GUIDs that resulted in the returned label.</span></span>                                         
## <a name="json-representation"></a><span data-ttu-id="e75db-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e75db-125">JSON representation</span></span>

<span data-ttu-id="e75db-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e75db-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applyLabelAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "actionSource": "String",
  "actions": [{"@odata.type": "microsoft.graph.informationProtectionAction"}],
  "label": {"@odata.type": "microsoft.graph.labelDetails"},
  "responsibleSensitiveTypeIds": ["Guid"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applyLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

