---
title: Тип ресурса customAction
description: Представляет любые настраиваемые действия, которые может предоставить метка, если настроен администратором.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1d9c88715cba6fc8faede1419b3c8809c3ec3f54
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941808"
---
# <a name="customaction-resource-type"></a><span data-ttu-id="3cfb7-103">Тип ресурса customAction</span><span class="sxs-lookup"><span data-stu-id="3cfb7-103">customAction resource type</span></span>

<span data-ttu-id="3cfb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cfb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cfb7-105">Представляет любые настраиваемые действия, которые может предоставить метка, если настроен администратором.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-105">Represents any custom actions that a label may provide, if configured by the administrator.</span></span> <span data-ttu-id="3cfb7-106">Настраиваемые действия можно определить как часть [informationProtectionLabel](informationProtectionLabel.md) с помощью модуля PowerShell Центра безопасности и соответствия требованиям Office 365.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-106">Custom actions might be defined as part of an [informationProtectionLabel](informationProtectionLabel.md) via Office 365 Security and Compliance Center's PowerShell module.</span></span> <span data-ttu-id="3cfb7-107">Действия должны быть понятны потребляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-107">The actions must be understood by the consuming application.</span></span>

## <a name="properties"></a><span data-ttu-id="3cfb7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3cfb7-108">Properties</span></span>

| <span data-ttu-id="3cfb7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3cfb7-109">Property</span></span>   | <span data-ttu-id="3cfb7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3cfb7-110">Type</span></span>                                       | <span data-ttu-id="3cfb7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3cfb7-111">Description</span></span>                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="3cfb7-112">name</span><span class="sxs-lookup"><span data-stu-id="3cfb7-112">name</span></span>       | <span data-ttu-id="3cfb7-113">String</span><span class="sxs-lookup"><span data-stu-id="3cfb7-113">String</span></span>                                     | <span data-ttu-id="3cfb7-114">Имя настраиваемого действия.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-114">Name of the custom action.</span></span>                           |
| <span data-ttu-id="3cfb7-115">properties</span><span class="sxs-lookup"><span data-stu-id="3cfb7-115">properties</span></span> | <span data-ttu-id="3cfb7-116">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3cfb7-116">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="3cfb7-117">Свойства в формате пары ключевых значений действия.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-117">Properties, in key value pair format, of the action.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3cfb7-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3cfb7-118">JSON representation</span></span>

<span data-ttu-id="3cfb7-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-119">The following is a JSON representation of the resource.</span></span>

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

