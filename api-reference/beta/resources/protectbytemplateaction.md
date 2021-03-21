---
title: тип ресурса protectByTemplateAction
description: Информирует приложение о том, что должен применяться шаблон защиты от информационных данных Azure.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6524774af3faa496b141e37ec270f8a73770ee63
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956829"
---
# <a name="protectbytemplateaction-resource-type"></a><span data-ttu-id="86951-103">тип ресурса protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="86951-103">protectByTemplateAction resource type</span></span>

<span data-ttu-id="86951-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86951-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86951-105">Информирует приложение о том, что должен применяться шаблон защиты от информационных данных Azure.</span><span class="sxs-lookup"><span data-stu-id="86951-105">Informs the application that an Azure Information Protection protection template should be applied.</span></span> <span data-ttu-id="86951-106">**ProtectionByTemplateAction** может быть возвращена с помощью [оценкиApplication](../api/informationprotectionlabel-evaluateapplication.md) или [evaluateClassificationResults,](../api/informationprotectionlabel-evaluateclassificationresults.md) если в результате метка настроена на применение защиты.</span><span class="sxs-lookup"><span data-stu-id="86951-106">**protectionByTemplateAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply protection.</span></span> <span data-ttu-id="86951-107">Потребляющие приложения должны считыть шаблонId из результата, а затем использовать клиентскую библиотеку, например SDK Microsoft Information Protection, для применения защиты с помощью Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="86951-107">The consuming application must read the templateId from the result and then use a client library, such as the Microsoft Information Protection SDK, to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="86951-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="86951-108">Properties</span></span>

| <span data-ttu-id="86951-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="86951-109">Property</span></span>   | <span data-ttu-id="86951-110">Тип</span><span class="sxs-lookup"><span data-stu-id="86951-110">Type</span></span>   | <span data-ttu-id="86951-111">Описание</span><span class="sxs-lookup"><span data-stu-id="86951-111">Description</span></span>                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="86951-112">templateId</span><span class="sxs-lookup"><span data-stu-id="86951-112">templateId</span></span> | <span data-ttu-id="86951-113">Строка</span><span class="sxs-lookup"><span data-stu-id="86951-113">String</span></span> | <span data-ttu-id="86951-114">GUID шаблона Azure Information Protection для применения к данным.</span><span class="sxs-lookup"><span data-stu-id="86951-114">The GUID of the Azure Information Protection template to apply to the information.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="86951-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86951-115">JSON representation</span></span>

<span data-ttu-id="86951-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86951-116">The following is a JSON representation of the resource.</span></span>

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

