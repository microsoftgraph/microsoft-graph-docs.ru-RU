---
title: Тип ресурса Токенмитингинфо
description: Тип Токенмитингинфо.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 138a003dfff142b0ea84d3a2b97a43681075d311
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015997"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="24c75-103">Тип ресурса Токенмитингинфо</span><span class="sxs-lookup"><span data-stu-id="24c75-103">tokenMeetingInfo resource type</span></span>

<span data-ttu-id="24c75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24c75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24c75-105">Это сведения о маркере, с помощью которого вы можете присоединиться к существующему собранию.</span><span class="sxs-lookup"><span data-stu-id="24c75-105">This is the token information that allows you to join an existing meeting.</span></span> <span data-ttu-id="24c75-106">Это значение получается в составе уведомления о входящем вызове.</span><span class="sxs-lookup"><span data-stu-id="24c75-106">This is obtained as part of the incoming call notification.</span></span> 

<span data-ttu-id="24c75-107">В случае отключения вызова эта информация поможет повторно присоединиться к этому вызову.</span><span class="sxs-lookup"><span data-stu-id="24c75-107">In the event that a call is disconnected, this information can help you rejoin that call.</span></span>

## <a name="properties"></a><span data-ttu-id="24c75-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="24c75-108">Properties</span></span>

| <span data-ttu-id="24c75-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="24c75-109">Property</span></span>                     | <span data-ttu-id="24c75-110">Тип</span><span class="sxs-lookup"><span data-stu-id="24c75-110">Type</span></span>    | <span data-ttu-id="24c75-111">Описание</span><span class="sxs-lookup"><span data-stu-id="24c75-111">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="24c75-112">token</span><span class="sxs-lookup"><span data-stu-id="24c75-112">token</span></span>                        | <span data-ttu-id="24c75-113">Строка</span><span class="sxs-lookup"><span data-stu-id="24c75-113">String</span></span>  | <span data-ttu-id="24c75-114">Маркер, используемый для присоединения к вызову.</span><span class="sxs-lookup"><span data-stu-id="24c75-114">The token used to join the call.</span></span>                                                 |

## <a name="json-representation"></a><span data-ttu-id="24c75-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24c75-115">JSON representation</span></span>

<span data-ttu-id="24c75-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24c75-116">The following is a JSON representation of the resource.</span></span>

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


