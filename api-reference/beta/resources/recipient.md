---
title: Тип ресурса recipient
description: 'Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e5117517bd9a2d25d5a29de57ab4a5d3c963ca89
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521252"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="912ba-103">Тип ресурса recipient</span><span class="sxs-lookup"><span data-stu-id="912ba-103">recipient resource type</span></span>

<span data-ttu-id="912ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="912ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="912ba-105">Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе.</span><span class="sxs-lookup"><span data-stu-id="912ba-105">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="912ba-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="912ba-106">Properties</span></span>
| <span data-ttu-id="912ba-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="912ba-107">Property</span></span>     | <span data-ttu-id="912ba-108">Тип</span><span class="sxs-lookup"><span data-stu-id="912ba-108">Type</span></span>   |<span data-ttu-id="912ba-109">Описание</span><span class="sxs-lookup"><span data-stu-id="912ba-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="912ba-110">emailAddress</span><span class="sxs-lookup"><span data-stu-id="912ba-110">emailAddress</span></span>|[<span data-ttu-id="912ba-111">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="912ba-111">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="912ba-112">Электронный адрес получателя.</span><span class="sxs-lookup"><span data-stu-id="912ba-112">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="912ba-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="912ba-113">JSON representation</span></span>

<span data-ttu-id="912ba-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="912ba-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
