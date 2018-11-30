---
title: Тип ресурса tokenMeetingInfo
description: Тип tokenMeetingInfo.
ms.openlocfilehash: ddaf9a0c36ce4a8a31c56e4db2e065ef186c4053
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076032"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="70f75-103">Тип ресурса tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="70f75-103">tokenMeetingInfo resource type</span></span>

> <span data-ttu-id="70f75-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="70f75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70f75-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70f75-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70f75-106">Тип tokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="70f75-106">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="70f75-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="70f75-107">Properties</span></span>

| <span data-ttu-id="70f75-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="70f75-108">Property</span></span>                     | <span data-ttu-id="70f75-109">Тип</span><span class="sxs-lookup"><span data-stu-id="70f75-109">Type</span></span>    | <span data-ttu-id="70f75-110">Description</span><span class="sxs-lookup"><span data-stu-id="70f75-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="70f75-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="70f75-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="70f75-112">Логический</span><span class="sxs-lookup"><span data-stu-id="70f75-112">Boolean</span></span> | <span data-ttu-id="70f75-113">Указывает, если беседы можно продолжить после покидает узла беседы.</span><span class="sxs-lookup"><span data-stu-id="70f75-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="70f75-114">токен</span><span class="sxs-lookup"><span data-stu-id="70f75-114">token</span></span>                        | <span data-ttu-id="70f75-115">Строка</span><span class="sxs-lookup"><span data-stu-id="70f75-115">String</span></span>  | <span data-ttu-id="70f75-116">Маркер для присоединения к/активации собрания.</span><span class="sxs-lookup"><span data-stu-id="70f75-116">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="70f75-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70f75-117">JSON representation</span></span>

<span data-ttu-id="70f75-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70f75-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="70f75-119">Пример</span><span class="sxs-lookup"><span data-stu-id="70f75-119">Example</span></span>

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
