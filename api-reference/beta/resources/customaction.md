---
title: Тип ресурса customAction
description: Представляет все настраиваемые действия, которые могут предоставляться метке, если она настроена администратором.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bbb3fc99ce474752fd2382d5777afeb1c56f632e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938872"
---
# <a name="customaction-resource-type"></a><span data-ttu-id="baaac-103">Тип ресурса customAction</span><span class="sxs-lookup"><span data-stu-id="baaac-103">customAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baaac-104">Представляет все настраиваемые действия, которые могут предоставляться метке, если она настроена администратором.</span><span class="sxs-lookup"><span data-stu-id="baaac-104">Represents any custom actions that a label may provide, if configured by the administrator.</span></span> <span data-ttu-id="baaac-105">Настраиваемые действия могут быть определены как часть [информатионпротектионлабел](informationProtectionLabel.md) с помощью модуля PowerShell центра безопасности и соответствия требованиям Office 365.</span><span class="sxs-lookup"><span data-stu-id="baaac-105">Custom actions might be defined as part of an [informationProtectionLabel](informationProtectionLabel.md) via Office 365 Security and Compliance Center's PowerShell module.</span></span> <span data-ttu-id="baaac-106">Приложение должно понимать действия, которые использует приложение.</span><span class="sxs-lookup"><span data-stu-id="baaac-106">The actions must be understood by the consuming application.</span></span>

## <a name="properties"></a><span data-ttu-id="baaac-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="baaac-107">Properties</span></span>

| <span data-ttu-id="baaac-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="baaac-108">Property</span></span>   | <span data-ttu-id="baaac-109">Тип</span><span class="sxs-lookup"><span data-stu-id="baaac-109">Type</span></span>                                       | <span data-ttu-id="baaac-110">Описание</span><span class="sxs-lookup"><span data-stu-id="baaac-110">Description</span></span>                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="baaac-111">name</span><span class="sxs-lookup"><span data-stu-id="baaac-111">name</span></span>       | <span data-ttu-id="baaac-112">String</span><span class="sxs-lookup"><span data-stu-id="baaac-112">String</span></span>                                     | <span data-ttu-id="baaac-113">Имя дополнительного действия.</span><span class="sxs-lookup"><span data-stu-id="baaac-113">Name of the custom action.</span></span>                           |
| <span data-ttu-id="baaac-114">properties</span><span class="sxs-lookup"><span data-stu-id="baaac-114">properties</span></span> | <span data-ttu-id="baaac-115">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="baaac-115">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="baaac-116">Свойства, в формате "комбинация значений ключей" действия.</span><span class="sxs-lookup"><span data-stu-id="baaac-116">Properties, in key value pair format, of the action.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="baaac-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="baaac-117">JSON representation</span></span>

<span data-ttu-id="baaac-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="baaac-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "name": "String",
  "properties": [{"@odata.type": "microsoft.graph.keyValuePair"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->