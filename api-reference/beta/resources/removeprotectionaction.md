---
title: Тип ресурса Ремовепротектионактион
description: Представляет действие для удаления защиты из файла или информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b3ed559460947e903e3085ab48edb421045bc3c6
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939280"
---
# <a name="removeprotectionaction-resource-type"></a><span data-ttu-id="490ea-103">Тип ресурса Ремовепротектионактион</span><span class="sxs-lookup"><span data-stu-id="490ea-103">removeProtectionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="490ea-104">Представляет действие для удаления защиты из файла или информации.</span><span class="sxs-lookup"><span data-stu-id="490ea-104">Represents an action to remove protection from the file or information.</span></span> <span data-ttu-id="490ea-105">API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовепротектионактион** , если необходимо удалить защиту в результате обновления или удаления метки.</span><span class="sxs-lookup"><span data-stu-id="490ea-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeProtectionAction** if protection is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="490ea-106">Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, который содержит заданный ранее заголовок контента.</span><span class="sxs-lookup"><span data-stu-id="490ea-106">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span> <span data-ttu-id="490ea-107">Защита должна быть удалена с помощью клиентской библиотеки, например Microsoft Information Protection SDK, только в том случае, если вызывающий пользователь имеет достаточные права на удаление защиты.</span><span class="sxs-lookup"><span data-stu-id="490ea-107">Protection should be removed via a client library, such as the Microsoft Information Protection SDK, only if the calling user has sufficient rights to remove protection.</span></span>

## <a name="properties"></a><span data-ttu-id="490ea-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="490ea-108">Properties</span></span>

<span data-ttu-id="490ea-109">Нет</span><span class="sxs-lookup"><span data-stu-id="490ea-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="490ea-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="490ea-110">JSON representation</span></span>

<span data-ttu-id="490ea-111">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="490ea-111">The following is a JSON representation of the resource.</span></span>

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