---
title: Тип ресурса tokenMeetingInfo
description: Тип tokenMeetingInfo.
author: VinodRavichandran
ms.openlocfilehash: 6fa66fef6f401db848a9ed3e92c5a1003a5294b6
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380550"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="bb135-103">Тип ресурса tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="bb135-103">tokenMeetingInfo resource type</span></span>

> <span data-ttu-id="bb135-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bb135-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb135-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb135-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb135-106">Тип tokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="bb135-106">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="bb135-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb135-107">Properties</span></span>

| <span data-ttu-id="bb135-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb135-108">Property</span></span>                     | <span data-ttu-id="bb135-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bb135-109">Type</span></span>    | <span data-ttu-id="bb135-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb135-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="bb135-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="bb135-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="bb135-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb135-112">Boolean</span></span> | <span data-ttu-id="bb135-113">Указывает, если беседы можно продолжить после покидает узла беседы.</span><span class="sxs-lookup"><span data-stu-id="bb135-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="bb135-114">токен</span><span class="sxs-lookup"><span data-stu-id="bb135-114">token</span></span>                        | <span data-ttu-id="bb135-115">Строка</span><span class="sxs-lookup"><span data-stu-id="bb135-115">String</span></span>  | <span data-ttu-id="bb135-116">Маркер для присоединения к/активации собрания.</span><span class="sxs-lookup"><span data-stu-id="bb135-116">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="bb135-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb135-117">JSON representation</span></span>

<span data-ttu-id="bb135-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb135-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="bb135-119">Пример</span><span class="sxs-lookup"><span data-stu-id="bb135-119">Example</span></span>

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
