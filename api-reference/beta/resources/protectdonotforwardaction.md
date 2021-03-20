---
title: тип ресурсов protectDoNotForwardAction
description: Информирует приложение о применении защиты Do Not Forward.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: a68771ea278ba8a904c032a86732b2b190eeeb43
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941773"
---
# <a name="protectdonotforwardaction-resource-type"></a><span data-ttu-id="84839-103">тип ресурсов protectDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="84839-103">protectDoNotForwardAction resource type</span></span>

<span data-ttu-id="84839-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84839-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84839-105">Информирует приложение о применении защиты Do Not Forward.</span><span class="sxs-lookup"><span data-stu-id="84839-105">Informs the application to apply Do Not Forward protection.</span></span> <span data-ttu-id="84839-106">**protectionDoNotForwardAction** может быть возвращена с помощью [оценкиApplication](../api/informationprotectionlabel-evaluateapplication.md) или [evaluateClassificationResults,](../api/informationprotectionlabel-evaluateclassificationresults.md) если результированная метка настроена для применения защиты [Do Not Forward.](/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails)</span><span class="sxs-lookup"><span data-stu-id="84839-106">**protectionDoNotForwardAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply [Do Not Forward protection](/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span></span> <span data-ttu-id="84839-107">Потребляемому приложению необходимо использовать клиентскую библиотеку для применения защиты с помощью Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="84839-107">The consuming application must use a client library to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="84839-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="84839-108">Properties</span></span>

<span data-ttu-id="84839-109">Нет</span><span class="sxs-lookup"><span data-stu-id="84839-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84839-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84839-110">JSON representation</span></span>

<span data-ttu-id="84839-111">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84839-111">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectDoNotForwardAction",
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
  "description": "protectDoNotForwardAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->