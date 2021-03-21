---
title: recommendLabelAction resource type
description: Представляет метку, которую следует рекомендовать пользователю для приложения к файлу на основе типов конфиденциальной информации.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 10d3ac687605ab648cdd3d68d6a3721c8fba2e30
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962576"
---
# <a name="recommendlabelaction-resource-type"></a><span data-ttu-id="07e93-103">recommendLabelAction resource type</span><span class="sxs-lookup"><span data-stu-id="07e93-103">recommendLabelAction resource type</span></span>

<span data-ttu-id="07e93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07e93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07e93-105">Представляет метку, которую следует рекомендовать пользователю для приложения к файлу на основе обнаруженных типов конфиденциальной информации.</span><span class="sxs-lookup"><span data-stu-id="07e93-105">Represents a label that should be recommended to the user for application to the file based on discovered sensitive information types.</span></span> <span data-ttu-id="07e93-106">В [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) может быть возвращена **рекомендацияLabelAction,** если политика  маркировки Microsoft Information Protection настроена на рекомендации и метку, а не на принудительное выполнение метки.</span><span class="sxs-lookup"><span data-stu-id="07e93-106">The [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) may return a **recommendLabelAction** if the Microsoft Information Protection labeling policy is set to **recommend** and label rather than enforce a label.</span></span> <span data-ttu-id="07e93-107">Пользователь или прикладный пользователь может игнорировать или принимать эту рекомендацию.</span><span class="sxs-lookup"><span data-stu-id="07e93-107">The user or appliation may choose to ignore or accept the recommendation.</span></span> 

## <a name="properties"></a><span data-ttu-id="07e93-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="07e93-108">Properties</span></span>

| <span data-ttu-id="07e93-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="07e93-109">Property</span></span>                    | <span data-ttu-id="07e93-110">Тип</span><span class="sxs-lookup"><span data-stu-id="07e93-110">Type</span></span>                                                                     | <span data-ttu-id="07e93-111">Описание</span><span class="sxs-lookup"><span data-stu-id="07e93-111">Description</span></span>                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| <span data-ttu-id="07e93-112">actionSource</span><span class="sxs-lookup"><span data-stu-id="07e93-112">actionSource</span></span>                | <span data-ttu-id="07e93-113">String</span><span class="sxs-lookup"><span data-stu-id="07e93-113">String</span></span>                                                                   | <span data-ttu-id="07e93-114">Возможные значения: `manual`, `automatic`, `recommended`, `default`.</span><span class="sxs-lookup"><span data-stu-id="07e93-114">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span> |
| <span data-ttu-id="07e93-115">actions</span><span class="sxs-lookup"><span data-stu-id="07e93-115">actions</span></span>                     | <span data-ttu-id="07e93-116">[коллекция informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="07e93-116">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="07e93-117">Действия, которые необходимо принять, если метка принята пользователем.</span><span class="sxs-lookup"><span data-stu-id="07e93-117">Actions to take if the label is accepted by the user.</span></span>                                                                       |
| <span data-ttu-id="07e93-118">label</span><span class="sxs-lookup"><span data-stu-id="07e93-118">label</span></span>                       | [<span data-ttu-id="07e93-119">labelDetails</span><span class="sxs-lookup"><span data-stu-id="07e93-119">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="07e93-120">Метка, которая рекомендуется.</span><span class="sxs-lookup"><span data-stu-id="07e93-120">The label that is being recommended.</span></span>                                                                      |
| <span data-ttu-id="07e93-121">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="07e93-121">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="07e93-122">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="07e93-122">Guid collection</span></span>                                                          | <span data-ttu-id="07e93-123">GUID типа конфиденциальной информации, из-за чего была дана рекомендация.</span><span class="sxs-lookup"><span data-stu-id="07e93-123">The sensitive information type GUIDs that caused the recommendation to be given.</span></span>                                                                      |

## <a name="json-representation"></a><span data-ttu-id="07e93-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07e93-124">JSON representation</span></span>

<span data-ttu-id="07e93-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07e93-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recommendLabelAction",
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
  "description": "recommendLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


