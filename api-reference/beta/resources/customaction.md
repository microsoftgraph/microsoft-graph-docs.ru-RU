---
title: Тип ресурса customAction
description: Представляет все настраиваемые действия, которые могут предоставляться метке, если она настроена администратором.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c71454a6647604d4155fc80c72ec48d22d85d03
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050012"
---
# <a name="customaction-resource-type"></a><span data-ttu-id="0d44b-103">Тип ресурса customAction</span><span class="sxs-lookup"><span data-stu-id="0d44b-103">customAction resource type</span></span>

<span data-ttu-id="0d44b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d44b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d44b-105">Представляет все настраиваемые действия, которые могут предоставляться метке, если она настроена администратором.</span><span class="sxs-lookup"><span data-stu-id="0d44b-105">Represents any custom actions that a label may provide, if configured by the administrator.</span></span> <span data-ttu-id="0d44b-106">Настраиваемые действия могут быть определены как часть [информатионпротектионлабел](informationProtectionLabel.md) с помощью модуля PowerShell центра безопасности и соответствия требованиям Office 365.</span><span class="sxs-lookup"><span data-stu-id="0d44b-106">Custom actions might be defined as part of an [informationProtectionLabel](informationProtectionLabel.md) via Office 365 Security and Compliance Center's PowerShell module.</span></span> <span data-ttu-id="0d44b-107">Приложение должно понимать действия, которые использует приложение.</span><span class="sxs-lookup"><span data-stu-id="0d44b-107">The actions must be understood by the consuming application.</span></span>

## <a name="properties"></a><span data-ttu-id="0d44b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d44b-108">Properties</span></span>

| <span data-ttu-id="0d44b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d44b-109">Property</span></span>   | <span data-ttu-id="0d44b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0d44b-110">Type</span></span>                                       | <span data-ttu-id="0d44b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d44b-111">Description</span></span>                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="0d44b-112">name</span><span class="sxs-lookup"><span data-stu-id="0d44b-112">name</span></span>       | <span data-ttu-id="0d44b-113">String</span><span class="sxs-lookup"><span data-stu-id="0d44b-113">String</span></span>                                     | <span data-ttu-id="0d44b-114">Имя дополнительного действия.</span><span class="sxs-lookup"><span data-stu-id="0d44b-114">Name of the custom action.</span></span>                           |
| <span data-ttu-id="0d44b-115">properties</span><span class="sxs-lookup"><span data-stu-id="0d44b-115">properties</span></span> | <span data-ttu-id="0d44b-116">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0d44b-116">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="0d44b-117">Свойства, в формате "комбинация значений ключей" действия.</span><span class="sxs-lookup"><span data-stu-id="0d44b-117">Properties, in key value pair format, of the action.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0d44b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d44b-118">JSON representation</span></span>

<span data-ttu-id="0d44b-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d44b-119">The following is a JSON representation of the resource.</span></span>

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

