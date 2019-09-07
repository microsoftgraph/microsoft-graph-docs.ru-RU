---
title: Тип ресурса Каллмедиастате
description: Представляет состояние мультимедиа для вызова.
author: VinodRavichandran
ms.prod: microsoft-teams
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 6b092598c50663ec9e7803a13332798d05fe095b
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36793035"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="8eb5b-103">Тип ресурса АудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="8eb5b-103">audioConferencing resource type</span></span>

> <span data-ttu-id="8eb5b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8eb5b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eb5b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eb5b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8eb5b-106">Представляет состояние [звонка для вызова](call.md).</span><span class="sxs-lookup"><span data-stu-id="8eb5b-106">Represents the media state for a call [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8eb5b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8eb5b-107">Properties</span></span>

| <span data-ttu-id="8eb5b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8eb5b-108">Property</span></span>            | <span data-ttu-id="8eb5b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8eb5b-109">Type</span></span>    | <span data-ttu-id="8eb5b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb5b-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="8eb5b-111">audio</span><span class="sxs-lookup"><span data-stu-id="8eb5b-111">audio</span></span>           | <span data-ttu-id="8eb5b-112">String.</span><span class="sxs-lookup"><span data-stu-id="8eb5b-112">String</span></span>  | <span data-ttu-id="8eb5b-113">Состояние звукового носителя.</span><span class="sxs-lookup"><span data-stu-id="8eb5b-113">The audio media state.</span></span> <span data-ttu-id="8eb5b-114">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="8eb5b-114">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8eb5b-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8eb5b-115">JSON representation</span></span>

<span data-ttu-id="8eb5b-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8eb5b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callMediaState"
}-->
```json
{
  "audio": "active | inactive",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callMediaState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
