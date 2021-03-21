---
title: removeProtectionAction resource type
description: Представляет действие по удалению защиты из файла или сведений.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2b315c9d2641524d8a134f0e0b9704c51419ada4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962037"
---
# <a name="removeprotectionaction-resource-type"></a><span data-ttu-id="efdf9-103">removeProtectionAction resource type</span><span class="sxs-lookup"><span data-stu-id="efdf9-103">removeProtectionAction resource type</span></span>

<span data-ttu-id="efdf9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efdf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efdf9-105">Представляет действие по удалению защиты из файла или сведений.</span><span class="sxs-lookup"><span data-stu-id="efdf9-105">Represents an action to remove protection from the file or information.</span></span> <span data-ttu-id="efdf9-106">[ОценкаApplication,](../api/informationprotectionlabel-evaluateapplication.md) [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)или оценка APIRemoval могут вернуть **removeProtectionAction,** если защита будет удалена в результате обновления или удаления метки. [](../api/informationprotectionlabel-evaluateremoval.md)</span><span class="sxs-lookup"><span data-stu-id="efdf9-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeProtectionAction** if protection is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="efdf9-107">Действие предписывает потребляемому приложению удалить определенный элемент пользовательского интерфейса, содержащий ранее применимый заголовок контента.</span><span class="sxs-lookup"><span data-stu-id="efdf9-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span> <span data-ttu-id="efdf9-108">Защита должна быть удалена с помощью клиентской библиотеки, например SDK Microsoft Information Protection, только если у вызываемого пользователя достаточно прав для удаления защиты.</span><span class="sxs-lookup"><span data-stu-id="efdf9-108">Protection should be removed via a client library, such as the Microsoft Information Protection SDK, only if the calling user has sufficient rights to remove protection.</span></span>

## <a name="properties"></a><span data-ttu-id="efdf9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="efdf9-109">Properties</span></span>

<span data-ttu-id="efdf9-110">Нет</span><span class="sxs-lookup"><span data-stu-id="efdf9-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efdf9-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efdf9-111">JSON representation</span></span>

<span data-ttu-id="efdf9-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efdf9-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeProtectionAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "removeProtectionAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

