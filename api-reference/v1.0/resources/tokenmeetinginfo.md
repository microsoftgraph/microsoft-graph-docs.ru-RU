---
title: Тип ресурса Токенмитингинфо
description: Тип Токенмитингинфо.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 05cc4c21fe3a8ea0d4b27b6c27b737ec6fe317d2
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912974"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="5b230-103">Тип ресурса Токенмитингинфо</span><span class="sxs-lookup"><span data-stu-id="5b230-103">tokenMeetingInfo resource type</span></span>

<span data-ttu-id="5b230-104">Это сведения о маркере, с помощью которого вы можете присоединиться к существующему собранию.</span><span class="sxs-lookup"><span data-stu-id="5b230-104">This is the token information that allows you to join an existing meeting.</span></span> <span data-ttu-id="5b230-105">Это значение получается в составе уведомления о входящем вызове.</span><span class="sxs-lookup"><span data-stu-id="5b230-105">This is obtained as part of the incoming call notification.</span></span> 

<span data-ttu-id="5b230-106">В случае отключения вызова эта информация поможет повторно присоединиться к этому вызову.</span><span class="sxs-lookup"><span data-stu-id="5b230-106">In the event that a call is disconnected, this information can help you rejoin that call.</span></span>

## <a name="properties"></a><span data-ttu-id="5b230-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b230-107">Properties</span></span>

| <span data-ttu-id="5b230-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b230-108">Property</span></span>                     | <span data-ttu-id="5b230-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5b230-109">Type</span></span>    | <span data-ttu-id="5b230-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5b230-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="5b230-111">token</span><span class="sxs-lookup"><span data-stu-id="5b230-111">token</span></span>                        | <span data-ttu-id="5b230-112">Строка</span><span class="sxs-lookup"><span data-stu-id="5b230-112">String</span></span>  | <span data-ttu-id="5b230-113">Маркер, используемый для присоединения к вызову.</span><span class="sxs-lookup"><span data-stu-id="5b230-113">The token used to join the call.</span></span>                                                 |

## <a name="json-representation"></a><span data-ttu-id="5b230-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b230-114">JSON representation</span></span>

<span data-ttu-id="5b230-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b230-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
    "token": "String"
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
