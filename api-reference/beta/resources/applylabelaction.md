---
title: Тип ресурса Апплилабелактион
description: Представляет набор действий, которые следует предпринять для применения или обновления метки.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fc7911b3a225f226edc74dc9b194a2522b7c4251
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939147"
---
# <a name="applylabelaction-resource-type"></a><span data-ttu-id="184ad-103">Тип ресурса Апплилабелактион</span><span class="sxs-lookup"><span data-stu-id="184ad-103">applyLabelAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="184ad-104">Представляет набор действий, которые следует предпринять для применения или обновления метки.</span><span class="sxs-lookup"><span data-stu-id="184ad-104">Represents a set of actions that should be taken to apply or update a label.</span></span> <span data-ttu-id="184ad-105">**апплилабелактион** возвращается, когда результат операции оценки метки состоит в том, что метка должна быть применена.</span><span class="sxs-lookup"><span data-stu-id="184ad-105">**applyLabelAction** is returned when the result of a label evaluation operation is that a label should be applied.</span></span> <span data-ttu-id="184ad-106">Свойство содержит коллекцию [информатионпротектионактион](informationProtectionaction.md) , в которой описывается полный набор действий для применения метки, включая удаление старых метаданных, маркировки содержимого и защиту. \*\* `actions`</span><span class="sxs-lookup"><span data-stu-id="184ad-106">The `actions` property contains an [informationProtectionAction](informationProtectionaction.md) collection that described the full set of actions to *apply* the label, including removal of old metadata, content marking, and protection.</span></span>

## <a name="properties"></a><span data-ttu-id="184ad-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="184ad-107">Properties</span></span>

| <span data-ttu-id="184ad-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="184ad-108">Property</span></span>                    | <span data-ttu-id="184ad-109">Тип</span><span class="sxs-lookup"><span data-stu-id="184ad-109">Type</span></span>                                                                     | <span data-ttu-id="184ad-110">Описание</span><span class="sxs-lookup"><span data-stu-id="184ad-110">Description</span></span>                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="184ad-111">актионсаурце</span><span class="sxs-lookup"><span data-stu-id="184ad-111">actionSource</span></span>                | <span data-ttu-id="184ad-112">String</span><span class="sxs-lookup"><span data-stu-id="184ad-112">String</span></span>                                                                   | <span data-ttu-id="184ad-113">Возможные значения: `manual`, `automatic`, `recommended`, `default`.</span><span class="sxs-lookup"><span data-stu-id="184ad-113">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span>                                                                                                                             |
| <span data-ttu-id="184ad-114">actions</span><span class="sxs-lookup"><span data-stu-id="184ad-114">actions</span></span>                     | <span data-ttu-id="184ad-115">Коллекция [информатионпротектионактион](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="184ad-115">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="184ad-116">Коллекция определенных действий, которые будут выполняться приложением использования для добавления метки в документ.</span><span class="sxs-lookup"><span data-stu-id="184ad-116">The collection of specific actions that should be taken by the consuming application to label the document.</span></span> <span data-ttu-id="184ad-117">Полный список представлен в [информатионпротектионактион](informationprotectionaction.md) .</span><span class="sxs-lookup"><span data-stu-id="184ad-117">See  [informationProtectionAction](informationprotectionaction.md) for the full list.</span></span> |
| <span data-ttu-id="184ad-118">label</span><span class="sxs-lookup"><span data-stu-id="184ad-118">label</span></span>                       | [<span data-ttu-id="184ad-119">лабелдетаилс</span><span class="sxs-lookup"><span data-stu-id="184ad-119">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="184ad-120">Объект, описывающий сведения о применяемой метке.</span><span class="sxs-lookup"><span data-stu-id="184ad-120">Object that describes the details of the label to apply.</span></span>                                                                                                                                          |
| <span data-ttu-id="184ad-121">респонсиблесенситиветипеидс</span><span class="sxs-lookup"><span data-stu-id="184ad-121">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="184ad-122">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="184ad-122">Guid collection</span></span>                                                          | <span data-ttu-id="184ad-123">Если метка была результатом автоматической классификации, предоставьте список идентификаторов GUID типа конфиденциальной информации, которые привели к возвращенной метке.</span><span class="sxs-lookup"><span data-stu-id="184ad-123">If the label was the result of an automatic classification, supply the list of sensitive info type GUIDs that resulted in the returned label.</span></span>                                         
## <a name="json-representation"></a><span data-ttu-id="184ad-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="184ad-124">JSON representation</span></span>

<span data-ttu-id="184ad-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="184ad-125">The following is a JSON representation of the resource.</span></span>

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