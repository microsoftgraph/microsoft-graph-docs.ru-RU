---
title: Тип ресурса recipient
description: 'Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе. '
localization_priority: Normal
ms.openlocfilehash: 4b326e7c85d8390ea6356860255103a466194f92
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343923"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="5ad77-103">Тип ресурса recipient</span><span class="sxs-lookup"><span data-stu-id="5ad77-103">recipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ad77-104">Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе.</span><span class="sxs-lookup"><span data-stu-id="5ad77-104">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="5ad77-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ad77-105">Properties</span></span>
| <span data-ttu-id="5ad77-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ad77-106">Property</span></span>     | <span data-ttu-id="5ad77-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5ad77-107">Type</span></span>   |<span data-ttu-id="5ad77-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5ad77-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ad77-109">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5ad77-109">emailAddress</span></span>|[<span data-ttu-id="5ad77-110">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="5ad77-110">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="5ad77-111">Электронный адрес получателя.</span><span class="sxs-lookup"><span data-stu-id="5ad77-111">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ad77-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ad77-112">JSON representation</span></span>

<span data-ttu-id="5ad77-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ad77-113">Here is a JSON representation of the resource</span></span>

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
