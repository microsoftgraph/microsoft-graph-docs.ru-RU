---
title: Тип ресурса Довнградежустификатион
description: Представляет ввод пользователя по причине выполнения возврата к предыдущей версии.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7c0e34d70bd91ecd896eba4329d775a95d696bed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979653"
---
# <a name="downgradejustification-resource-type"></a><span data-ttu-id="53941-103">Тип ресурса Довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="53941-103">downgradeJustification resource type</span></span>

<span data-ttu-id="53941-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53941-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53941-105">Представляет ввод пользователя по причине выполнения возврата к предыдущей версии.</span><span class="sxs-lookup"><span data-stu-id="53941-105">Represents user input on why downgrade was performed.</span></span> <span data-ttu-id="53941-106">Выравнивание на более ранней версии может потребоваться на основе конфигурации политики меток в центре безопасности и соответствия требованиям Office.</span><span class="sxs-lookup"><span data-stu-id="53941-106">Downgrade justification might be required based on label policy configuration in Office Security and Compliance Center.</span></span>

## <a name="properties"></a><span data-ttu-id="53941-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="53941-107">Properties</span></span>

| <span data-ttu-id="53941-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="53941-108">Property</span></span>             | <span data-ttu-id="53941-109">Тип</span><span class="sxs-lookup"><span data-stu-id="53941-109">Type</span></span>    | <span data-ttu-id="53941-110">Описание</span><span class="sxs-lookup"><span data-stu-id="53941-110">Description</span></span>                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="53941-111">исдовнградежустифиед</span><span class="sxs-lookup"><span data-stu-id="53941-111">isDowngradeJustified</span></span> | <span data-ttu-id="53941-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="53941-112">Boolean</span></span> | <span data-ttu-id="53941-113">Указывает, является ли переход на предыдущее или не выровненный.</span><span class="sxs-lookup"><span data-stu-id="53941-113">Indicates whether the downgrade is or is not justified.</span></span>                                              |
| <span data-ttu-id="53941-114">жустификатионмессаже</span><span class="sxs-lookup"><span data-stu-id="53941-114">justificationMessage</span></span> | <span data-ttu-id="53941-115">String</span><span class="sxs-lookup"><span data-stu-id="53941-115">String</span></span>  | <span data-ttu-id="53941-116">Сообщение, указывающее, почему выравниваются более ранние версии.</span><span class="sxs-lookup"><span data-stu-id="53941-116">Message that indicates why a downgrade is justified.</span></span> <span data-ttu-id="53941-117">Сообщение будет отображаться в разделе Журналы администрирования.</span><span class="sxs-lookup"><span data-stu-id="53941-117">The message will appear in administrative logs.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="53941-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53941-118">JSON representation</span></span>

<span data-ttu-id="53941-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53941-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.downgradeJustification",
  "baseType": null
}-->

```json
{
  "isDowngradeJustified": true,
  "justificationMessage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "downgradeJustification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

