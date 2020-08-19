---
title: Тип ресурса recipient
description: 'Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе. '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: daf48391c0dd26ded407659ff9159703aed31566
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806823"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="adcf4-103">Тип ресурса recipient</span><span class="sxs-lookup"><span data-stu-id="adcf4-103">recipient resource type</span></span>

<span data-ttu-id="adcf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adcf4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="adcf4-105">Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе.</span><span class="sxs-lookup"><span data-stu-id="adcf4-105">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="adcf4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="adcf4-106">Properties</span></span>
| <span data-ttu-id="adcf4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="adcf4-107">Property</span></span>     | <span data-ttu-id="adcf4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="adcf4-108">Type</span></span>   |<span data-ttu-id="adcf4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="adcf4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adcf4-110">emailAddress</span><span class="sxs-lookup"><span data-stu-id="adcf4-110">emailAddress</span></span>|[<span data-ttu-id="adcf4-111">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="adcf4-111">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="adcf4-112">Электронный адрес получателя.</span><span class="sxs-lookup"><span data-stu-id="adcf4-112">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="adcf4-113">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="adcf4-113">JSON representation</span></span>

<span data-ttu-id="adcf4-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adcf4-114">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
