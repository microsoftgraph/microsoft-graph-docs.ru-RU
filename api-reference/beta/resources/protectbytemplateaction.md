---
title: Тип ресурса Протектбитемплатеактион
description: Информирует приложение о том, что шаблон защиты Azure Information Protection должен быть применен.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 19103cd07404677b680606a6fd0ec9d4caa43600
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993162"
---
# <a name="protectbytemplateaction-resource-type"></a><span data-ttu-id="49a4a-103">Тип ресурса Протектбитемплатеактион</span><span class="sxs-lookup"><span data-stu-id="49a4a-103">protectByTemplateAction resource type</span></span>

<span data-ttu-id="49a4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49a4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49a4a-105">Информирует приложение о том, что шаблон защиты Azure Information Protection должен быть применен.</span><span class="sxs-lookup"><span data-stu-id="49a4a-105">Informs the application that an Azure Information Protection protection template should be applied.</span></span> <span data-ttu-id="49a4a-106">**протектионбитемплатеактион** может быть возвращено [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md) или [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) , если полученная метка настроена на применение защиты.</span><span class="sxs-lookup"><span data-stu-id="49a4a-106">**protectionByTemplateAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply protection.</span></span> <span data-ttu-id="49a4a-107">Приложение-приложение должно прочитать templateId из результата, а затем использовать клиентскую библиотеку, например Microsoft Information Protection SDK, для применения защиты с помощью Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="49a4a-107">The consuming application must read the templateId from the result and then use a client library, such as the Microsoft Information Protection SDK, to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="49a4a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="49a4a-108">Properties</span></span>

| <span data-ttu-id="49a4a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="49a4a-109">Property</span></span>   | <span data-ttu-id="49a4a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="49a4a-110">Type</span></span>   | <span data-ttu-id="49a4a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="49a4a-111">Description</span></span>                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="49a4a-112">templateId</span><span class="sxs-lookup"><span data-stu-id="49a4a-112">templateId</span></span> | <span data-ttu-id="49a4a-113">String</span><span class="sxs-lookup"><span data-stu-id="49a4a-113">String</span></span> | <span data-ttu-id="49a4a-114">GUID шаблона Azure Information Protection для применения к данным.</span><span class="sxs-lookup"><span data-stu-id="49a4a-114">The GUID of the Azure Information Protection template to apply to the information.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="49a4a-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49a4a-115">JSON representation</span></span>

<span data-ttu-id="49a4a-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49a4a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectByTemplateAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "templateId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "protectByTemplateAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

