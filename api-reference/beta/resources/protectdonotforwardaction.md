---
title: Тип ресурса Протектдонотфорвардактион
description: Информирует приложение о необходимости защиты от пересылки.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1d9687460a549438db1c9076bef2184b0b1ee5d3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939189"
---
# <a name="protectdonotforwardaction-resource-type"></a><span data-ttu-id="c262b-103">Тип ресурса Протектдонотфорвардактион</span><span class="sxs-lookup"><span data-stu-id="c262b-103">protectDoNotForwardAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c262b-104">Информирует приложение о необходимости защиты от пересылки.</span><span class="sxs-lookup"><span data-stu-id="c262b-104">Informs the application to apply Do Not Forward protection.</span></span> <span data-ttu-id="c262b-105">**протектиондонотфорвардактион** может быть возвращено [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md) или [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) , если результирующая метка настроена для применения [защиты от пересылки](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span><span class="sxs-lookup"><span data-stu-id="c262b-105">**protectionDoNotForwardAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply [Do Not Forward protection](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span></span> <span data-ttu-id="c262b-106">Приложение, использующее приложение, должно использовать клиентскую библиотеку для применения защиты с помощью Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="c262b-106">The consuming application must use a client library to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="c262b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c262b-107">Properties</span></span>

<span data-ttu-id="c262b-108">Нет</span><span class="sxs-lookup"><span data-stu-id="c262b-108">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c262b-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c262b-109">JSON representation</span></span>

<span data-ttu-id="c262b-110">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c262b-110">The following is a JSON representation of the resource.</span></span>

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
