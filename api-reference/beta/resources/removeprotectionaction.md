---
title: Тип ресурса Ремовепротектионактион
description: Представляет действие для удаления защиты из файла или информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63a539fe4366703aaeb7e6b16735bb0302951dd7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521147"
---
# <a name="removeprotectionaction-resource-type"></a><span data-ttu-id="ddbe6-103">Тип ресурса Ремовепротектионактион</span><span class="sxs-lookup"><span data-stu-id="ddbe6-103">removeProtectionAction resource type</span></span>

<span data-ttu-id="ddbe6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ddbe6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddbe6-105">Представляет действие для удаления защиты из файла или информации.</span><span class="sxs-lookup"><span data-stu-id="ddbe6-105">Represents an action to remove protection from the file or information.</span></span> <span data-ttu-id="ddbe6-106">API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовепротектионактион** , если необходимо удалить защиту в результате обновления или удаления метки.</span><span class="sxs-lookup"><span data-stu-id="ddbe6-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeProtectionAction** if protection is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="ddbe6-107">Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, который содержит заданный ранее заголовок контента.</span><span class="sxs-lookup"><span data-stu-id="ddbe6-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span> <span data-ttu-id="ddbe6-108">Защита должна быть удалена с помощью клиентской библиотеки, например Microsoft Information Protection SDK, только в том случае, если вызывающий пользователь имеет достаточные права на удаление защиты.</span><span class="sxs-lookup"><span data-stu-id="ddbe6-108">Protection should be removed via a client library, such as the Microsoft Information Protection SDK, only if the calling user has sufficient rights to remove protection.</span></span>

## <a name="properties"></a><span data-ttu-id="ddbe6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ddbe6-109">Properties</span></span>

<span data-ttu-id="ddbe6-110">Нет</span><span class="sxs-lookup"><span data-stu-id="ddbe6-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddbe6-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ddbe6-111">JSON representation</span></span>

<span data-ttu-id="ddbe6-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddbe6-112">The following is a JSON representation of the resource.</span></span>

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