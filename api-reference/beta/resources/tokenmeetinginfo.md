---
title: Тип ресурса tokenMeetingInfo
description: Тип tokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0d68b60cdfc1470bb1c1c3846c34dfc76c5c5a1b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919269"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="1f3f2-103">Тип ресурса tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="1f3f2-103">tokenMeetingInfo resource type</span></span>

> <span data-ttu-id="1f3f2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1f3f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f3f2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f3f2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f3f2-106">Тип tokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="1f3f2-106">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="1f3f2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f3f2-107">Properties</span></span>

| <span data-ttu-id="1f3f2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f3f2-108">Property</span></span>                     | <span data-ttu-id="1f3f2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1f3f2-109">Type</span></span>    | <span data-ttu-id="1f3f2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1f3f2-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="1f3f2-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="1f3f2-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="1f3f2-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f3f2-112">Boolean</span></span> | <span data-ttu-id="1f3f2-113">Указывает, если беседы можно продолжить после покидает узла беседы.</span><span class="sxs-lookup"><span data-stu-id="1f3f2-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="1f3f2-114">токен</span><span class="sxs-lookup"><span data-stu-id="1f3f2-114">token</span></span>                        | <span data-ttu-id="1f3f2-115">Строка</span><span class="sxs-lookup"><span data-stu-id="1f3f2-115">String</span></span>  | <span data-ttu-id="1f3f2-116">Маркер для присоединения к/активации собрания.</span><span class="sxs-lookup"><span data-stu-id="1f3f2-116">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="1f3f2-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f3f2-117">JSON representation</span></span>

<span data-ttu-id="1f3f2-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f3f2-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="1f3f2-119">Пример</span><span class="sxs-lookup"><span data-stu-id="1f3f2-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
