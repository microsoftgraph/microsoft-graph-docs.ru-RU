---
title: Тип ресурса callRoute
description: Тип callRoute.
author: VinodRavichandran
ms.openlocfilehash: 9538fb8f27f60e869c19edc7bd19d7f6b29e8fff
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380158"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="10427-103">Тип ресурса callRoute</span><span class="sxs-lookup"><span data-stu-id="10427-103">callRoute resource type</span></span>

> <span data-ttu-id="10427-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="10427-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10427-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10427-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="10427-106">Тип callRoute.</span><span class="sxs-lookup"><span data-stu-id="10427-106">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="10427-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="10427-107">Properties</span></span>

| <span data-ttu-id="10427-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="10427-108">Property</span></span>            | <span data-ttu-id="10427-109">Тип</span><span class="sxs-lookup"><span data-stu-id="10427-109">Type</span></span>                          | <span data-ttu-id="10427-110">Описание</span><span class="sxs-lookup"><span data-stu-id="10427-110">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="10427-111">Окончательный</span><span class="sxs-lookup"><span data-stu-id="10427-111">final</span></span>               | [<span data-ttu-id="10427-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="10427-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="10427-113">Идентификатор, который был разрешен к в вызове.</span><span class="sxs-lookup"><span data-stu-id="10427-113">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="10427-114">Исходный текст</span><span class="sxs-lookup"><span data-stu-id="10427-114">original</span></span>            | [<span data-ttu-id="10427-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="10427-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="10427-116">Идентификатор, который изначально использовался в вызове.</span><span class="sxs-lookup"><span data-stu-id="10427-116">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="10427-117">routingType</span><span class="sxs-lookup"><span data-stu-id="10427-117">routingType</span></span>         | <span data-ttu-id="10427-118">String</span><span class="sxs-lookup"><span data-stu-id="10427-118">String</span></span>                        | <span data-ttu-id="10427-119">Возможные значения: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="10427-119">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="10427-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10427-120">JSON representation</span></span>

<span data-ttu-id="10427-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10427-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
