---
title: Тип ресурса customAction
description: Представляет все настраиваемые действия, которые могут предоставляться метке, если она настроена администратором.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e2a660659f8c0f3a2c6dc571e743884c54365a20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507326"
---
# <a name="customaction-resource-type"></a><span data-ttu-id="6e628-103">Тип ресурса customAction</span><span class="sxs-lookup"><span data-stu-id="6e628-103">customAction resource type</span></span>

<span data-ttu-id="6e628-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e628-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e628-105">Представляет все настраиваемые действия, которые могут предоставляться метке, если она настроена администратором.</span><span class="sxs-lookup"><span data-stu-id="6e628-105">Represents any custom actions that a label may provide, if configured by the administrator.</span></span> <span data-ttu-id="6e628-106">Настраиваемые действия могут быть определены как часть [информатионпротектионлабел](informationProtectionLabel.md) с помощью модуля PowerShell центра безопасности и соответствия требованиям Office 365.</span><span class="sxs-lookup"><span data-stu-id="6e628-106">Custom actions might be defined as part of an [informationProtectionLabel](informationProtectionLabel.md) via Office 365 Security and Compliance Center's PowerShell module.</span></span> <span data-ttu-id="6e628-107">Приложение должно понимать действия, которые использует приложение.</span><span class="sxs-lookup"><span data-stu-id="6e628-107">The actions must be understood by the consuming application.</span></span>

## <a name="properties"></a><span data-ttu-id="6e628-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e628-108">Properties</span></span>

| <span data-ttu-id="6e628-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e628-109">Property</span></span>   | <span data-ttu-id="6e628-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6e628-110">Type</span></span>                                       | <span data-ttu-id="6e628-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6e628-111">Description</span></span>                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="6e628-112">name</span><span class="sxs-lookup"><span data-stu-id="6e628-112">name</span></span>       | <span data-ttu-id="6e628-113">String</span><span class="sxs-lookup"><span data-stu-id="6e628-113">String</span></span>                                     | <span data-ttu-id="6e628-114">Имя дополнительного действия.</span><span class="sxs-lookup"><span data-stu-id="6e628-114">Name of the custom action.</span></span>                           |
| <span data-ttu-id="6e628-115">properties</span><span class="sxs-lookup"><span data-stu-id="6e628-115">properties</span></span> | <span data-ttu-id="6e628-116">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6e628-116">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="6e628-117">Свойства, в формате "комбинация значений ключей" действия.</span><span class="sxs-lookup"><span data-stu-id="6e628-117">Properties, in key value pair format, of the action.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6e628-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e628-118">JSON representation</span></span>

<span data-ttu-id="6e628-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e628-119">The following is a JSON representation of the resource.</span></span>

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