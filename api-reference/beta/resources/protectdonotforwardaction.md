---
title: Тип ресурса Протектдонотфорвардактион
description: Информирует приложение о необходимости защиты от пересылки.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: db7605fb421878f258420f79c1cd06055624e53d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521364"
---
# <a name="protectdonotforwardaction-resource-type"></a><span data-ttu-id="e2c11-103">Тип ресурса Протектдонотфорвардактион</span><span class="sxs-lookup"><span data-stu-id="e2c11-103">protectDoNotForwardAction resource type</span></span>

<span data-ttu-id="e2c11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2c11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2c11-105">Информирует приложение о необходимости защиты от пересылки.</span><span class="sxs-lookup"><span data-stu-id="e2c11-105">Informs the application to apply Do Not Forward protection.</span></span> <span data-ttu-id="e2c11-106">**протектиондонотфорвардактион** может быть возвращено [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md) или [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) , если результирующая метка настроена для применения [защиты от пересылки](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span><span class="sxs-lookup"><span data-stu-id="e2c11-106">**protectionDoNotForwardAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply [Do Not Forward protection](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span></span> <span data-ttu-id="e2c11-107">Приложение, использующее приложение, должно использовать клиентскую библиотеку для применения защиты с помощью Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="e2c11-107">The consuming application must use a client library to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="e2c11-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2c11-108">Properties</span></span>

<span data-ttu-id="e2c11-109">Нет</span><span class="sxs-lookup"><span data-stu-id="e2c11-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2c11-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2c11-110">JSON representation</span></span>

<span data-ttu-id="e2c11-111">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2c11-111">The following is a JSON representation of the resource.</span></span>

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
