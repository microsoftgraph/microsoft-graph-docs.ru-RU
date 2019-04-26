---
title: Тип ресурса Токенмитингинфо
description: Тип Токенмитингинфо.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 38a5aae17cf4364a1cfd58680c2e7b9437cf0e40
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345510"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="2fde0-103">Тип ресурса Токенмитингинфо</span><span class="sxs-lookup"><span data-stu-id="2fde0-103">tokenMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fde0-104">Тип Токенмитингинфо.</span><span class="sxs-lookup"><span data-stu-id="2fde0-104">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="2fde0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2fde0-105">Properties</span></span>

| <span data-ttu-id="2fde0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fde0-106">Property</span></span>                     | <span data-ttu-id="2fde0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2fde0-107">Type</span></span>    | <span data-ttu-id="2fde0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2fde0-108">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="2fde0-109">Алловконверсатионвисаусост</span><span class="sxs-lookup"><span data-stu-id="2fde0-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="2fde0-110">Логический</span><span class="sxs-lookup"><span data-stu-id="2fde0-110">Boolean</span></span> | <span data-ttu-id="2fde0-111">Указывает, может ли беседа продолжиться после закрытия узла беседы.</span><span class="sxs-lookup"><span data-stu-id="2fde0-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="2fde0-112">токен</span><span class="sxs-lookup"><span data-stu-id="2fde0-112">token</span></span>                        | <span data-ttu-id="2fde0-113">Строка</span><span class="sxs-lookup"><span data-stu-id="2fde0-113">String</span></span>  | <span data-ttu-id="2fde0-114">Токен для присоединения и активации собрания.</span><span class="sxs-lookup"><span data-stu-id="2fde0-114">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="2fde0-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2fde0-115">JSON representation</span></span>

<span data-ttu-id="2fde0-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fde0-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType": "microsoft.graph.meetingInfo",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="2fde0-117">Пример</span><span class="sxs-lookup"><span data-stu-id="2fde0-117">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
