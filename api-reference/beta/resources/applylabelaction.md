---
title: Тип ресурса Апплилабелактион
description: Представляет набор действий, которые следует предпринять для применения или обновления метки.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2ea3d99ddd22056f9a3413f047a20387bf22a934
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050229"
---
# <a name="applylabelaction-resource-type"></a><span data-ttu-id="9f05b-103">Тип ресурса Апплилабелактион</span><span class="sxs-lookup"><span data-stu-id="9f05b-103">applyLabelAction resource type</span></span>

<span data-ttu-id="9f05b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f05b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f05b-105">Представляет набор действий, которые следует предпринять для применения или обновления метки.</span><span class="sxs-lookup"><span data-stu-id="9f05b-105">Represents a set of actions that should be taken to apply or update a label.</span></span> <span data-ttu-id="9f05b-106">**апплилабелактион** возвращается, когда результат операции оценки метки состоит в том, что метка должна быть применена.</span><span class="sxs-lookup"><span data-stu-id="9f05b-106">**applyLabelAction** is returned when the result of a label evaluation operation is that a label should be applied.</span></span> <span data-ttu-id="9f05b-107">`actions`Свойство содержит коллекцию [информатионпротектионактион](informationProtectionaction.md) , в которой описывается полный набор действий для *применения* метки, включая удаление старых метаданных, маркировки содержимого и защиту.</span><span class="sxs-lookup"><span data-stu-id="9f05b-107">The `actions` property contains an [informationProtectionAction](informationProtectionaction.md) collection that described the full set of actions to *apply* the label, including removal of old metadata, content marking, and protection.</span></span>

## <a name="properties"></a><span data-ttu-id="9f05b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f05b-108">Properties</span></span>

| <span data-ttu-id="9f05b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f05b-109">Property</span></span>                    | <span data-ttu-id="9f05b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9f05b-110">Type</span></span>                                                                     | <span data-ttu-id="9f05b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9f05b-111">Description</span></span>                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="9f05b-112">актионсаурце</span><span class="sxs-lookup"><span data-stu-id="9f05b-112">actionSource</span></span>                | <span data-ttu-id="9f05b-113">String</span><span class="sxs-lookup"><span data-stu-id="9f05b-113">String</span></span>                                                                   | <span data-ttu-id="9f05b-114">Возможные значения: `manual`, `automatic`, `recommended`, `default`.</span><span class="sxs-lookup"><span data-stu-id="9f05b-114">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span>                                                                                                                             |
| <span data-ttu-id="9f05b-115">actions</span><span class="sxs-lookup"><span data-stu-id="9f05b-115">actions</span></span>                     | <span data-ttu-id="9f05b-116">Коллекция [информатионпротектионактион](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="9f05b-116">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="9f05b-117">Коллекция определенных действий, которые будут выполняться приложением использования для добавления метки в документ.</span><span class="sxs-lookup"><span data-stu-id="9f05b-117">The collection of specific actions that should be taken by the consuming application to label the document.</span></span> <span data-ttu-id="9f05b-118">Полный список представлен в  [информатионпротектионактион](informationprotectionaction.md) .</span><span class="sxs-lookup"><span data-stu-id="9f05b-118">See  [informationProtectionAction](informationprotectionaction.md) for the full list.</span></span> |
| <span data-ttu-id="9f05b-119">label</span><span class="sxs-lookup"><span data-stu-id="9f05b-119">label</span></span>                       | [<span data-ttu-id="9f05b-120">лабелдетаилс</span><span class="sxs-lookup"><span data-stu-id="9f05b-120">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="9f05b-121">Объект, описывающий сведения о применяемой метке.</span><span class="sxs-lookup"><span data-stu-id="9f05b-121">Object that describes the details of the label to apply.</span></span>                                                                                                                                          |
| <span data-ttu-id="9f05b-122">респонсиблесенситиветипеидс</span><span class="sxs-lookup"><span data-stu-id="9f05b-122">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="9f05b-123">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="9f05b-123">Guid collection</span></span>                                                          | <span data-ttu-id="9f05b-124">Если метка была результатом автоматической классификации, предоставьте список идентификаторов GUID типа конфиденциальной информации, которые привели к возвращенной метке.</span><span class="sxs-lookup"><span data-stu-id="9f05b-124">If the label was the result of an automatic classification, supply the list of sensitive info type GUIDs that resulted in the returned label.</span></span>                                         
## <a name="json-representation"></a><span data-ttu-id="9f05b-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f05b-125">JSON representation</span></span>

<span data-ttu-id="9f05b-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f05b-126">The following is a JSON representation of the resource.</span></span>

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

