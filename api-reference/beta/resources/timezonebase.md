---
title: Тип ресурса timeZoneBase
description: Основное представление часового пояса.
ms.openlocfilehash: 00e09b064a083aa72316838c213f9c84e1139a19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081478"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="26a4c-103">Тип ресурса timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="26a4c-103">timeZoneBase resource type</span></span>

> <span data-ttu-id="26a4c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="26a4c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26a4c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a4c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26a4c-106">Основное представление часового пояса.</span><span class="sxs-lookup"><span data-stu-id="26a4c-106">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="26a4c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="26a4c-107">Properties</span></span>
| <span data-ttu-id="26a4c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="26a4c-108">Property</span></span>     | <span data-ttu-id="26a4c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="26a4c-109">Type</span></span>   |<span data-ttu-id="26a4c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="26a4c-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26a4c-111">name</span><span class="sxs-lookup"><span data-stu-id="26a4c-111">name</span></span> | <span data-ttu-id="26a4c-112">строка</span><span class="sxs-lookup"><span data-stu-id="26a4c-112">string</span></span> | <span data-ttu-id="26a4c-113">Имя часового пояса</span><span class="sxs-lookup"><span data-stu-id="26a4c-113">The name of a time zone.</span></span> <span data-ttu-id="26a4c-114">(стандартного, например "Гавайско-Алеутское время (зима)" или особого, например "Особый часовой пояс").</span><span class="sxs-lookup"><span data-stu-id="26a4c-114">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="26a4c-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26a4c-115">JSON representation</span></span>

<span data-ttu-id="26a4c-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26a4c-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->