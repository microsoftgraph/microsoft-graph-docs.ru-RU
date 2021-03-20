---
title: тип ресурса downgradeJustification
description: Представляет пользовательские сведения о том, почему было выполнено понижение.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: bc7336469f93de9e6d2b07fe73df9dce2eafd47f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941801"
---
# <a name="downgradejustification-resource-type"></a><span data-ttu-id="97a1b-103">тип ресурса downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="97a1b-103">downgradeJustification resource type</span></span>

<span data-ttu-id="97a1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97a1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97a1b-105">Представляет пользовательские сведения о том, почему было выполнено понижение.</span><span class="sxs-lookup"><span data-stu-id="97a1b-105">Represents user input on why downgrade was performed.</span></span> <span data-ttu-id="97a1b-106">Обоснование понижения может потребоваться на основе конфигурации политики меток в Центре безопасности и соответствия требованиям Office.</span><span class="sxs-lookup"><span data-stu-id="97a1b-106">Downgrade justification might be required based on label policy configuration in Office Security and Compliance Center.</span></span>

## <a name="properties"></a><span data-ttu-id="97a1b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="97a1b-107">Properties</span></span>

| <span data-ttu-id="97a1b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="97a1b-108">Property</span></span>             | <span data-ttu-id="97a1b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="97a1b-109">Type</span></span>    | <span data-ttu-id="97a1b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="97a1b-110">Description</span></span>                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="97a1b-111">isDowngradeJustified</span><span class="sxs-lookup"><span data-stu-id="97a1b-111">isDowngradeJustified</span></span> | <span data-ttu-id="97a1b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="97a1b-112">Boolean</span></span> | <span data-ttu-id="97a1b-113">Указывает, является ли понижение или не оправдано.</span><span class="sxs-lookup"><span data-stu-id="97a1b-113">Indicates whether the downgrade is or is not justified.</span></span>                                              |
| <span data-ttu-id="97a1b-114">justificationMessage</span><span class="sxs-lookup"><span data-stu-id="97a1b-114">justificationMessage</span></span> | <span data-ttu-id="97a1b-115">Строка</span><span class="sxs-lookup"><span data-stu-id="97a1b-115">String</span></span>  | <span data-ttu-id="97a1b-116">Сообщение, которое указывает, почему понижение является оправданным.</span><span class="sxs-lookup"><span data-stu-id="97a1b-116">Message that indicates why a downgrade is justified.</span></span> <span data-ttu-id="97a1b-117">Сообщение будет отображаться в административных журналах.</span><span class="sxs-lookup"><span data-stu-id="97a1b-117">The message will appear in administrative logs.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="97a1b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97a1b-118">JSON representation</span></span>

<span data-ttu-id="97a1b-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97a1b-119">The following is a JSON representation of the resource.</span></span>

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

