---
title: Тип ресурса Протектбитемплатеактион
description: Информирует приложение о том, что шаблон защиты Azure Information Protection должен быть применен.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a7a557dfd72dac9161ae29436f5fc96eb55075d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939076"
---
# <a name="protectbytemplateaction-resource-type"></a><span data-ttu-id="84f63-103">Тип ресурса Протектбитемплатеактион</span><span class="sxs-lookup"><span data-stu-id="84f63-103">protectByTemplateAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84f63-104">Информирует приложение о том, что шаблон защиты Azure Information Protection должен быть применен.</span><span class="sxs-lookup"><span data-stu-id="84f63-104">Informs the application that an Azure Information Protection protection template should be applied.</span></span> <span data-ttu-id="84f63-105">**протектионбитемплатеактион** может быть возвращено [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md) или [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) , если полученная метка настроена на применение защиты.</span><span class="sxs-lookup"><span data-stu-id="84f63-105">**protectionByTemplateAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply protection.</span></span> <span data-ttu-id="84f63-106">Приложение-приложение должно прочитать templateId из результата, а затем использовать клиентскую библиотеку, например Microsoft Information Protection SDK, для применения защиты с помощью Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="84f63-106">The consuming application must read the templateId from the result and then use a client library, such as the Microsoft Information Protection SDK, to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="84f63-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="84f63-107">Properties</span></span>

| <span data-ttu-id="84f63-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="84f63-108">Property</span></span>   | <span data-ttu-id="84f63-109">Тип</span><span class="sxs-lookup"><span data-stu-id="84f63-109">Type</span></span>   | <span data-ttu-id="84f63-110">Описание</span><span class="sxs-lookup"><span data-stu-id="84f63-110">Description</span></span>                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="84f63-111">templateId</span><span class="sxs-lookup"><span data-stu-id="84f63-111">templateId</span></span> | <span data-ttu-id="84f63-112">Строка</span><span class="sxs-lookup"><span data-stu-id="84f63-112">String</span></span> | <span data-ttu-id="84f63-113">GUID шаблона Azure Information Protection для применения к данным.</span><span class="sxs-lookup"><span data-stu-id="84f63-113">The GUID of the Azure Information Protection template to apply to the information.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="84f63-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84f63-114">JSON representation</span></span>

<span data-ttu-id="84f63-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84f63-115">The following is a JSON representation of the resource.</span></span>

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