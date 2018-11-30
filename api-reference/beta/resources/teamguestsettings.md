---
title: Тип ресурса teamGuestSettings
description: Параметры для настройки ли гости могут создать, обновить или удалить каналы рабочих групп.
ms.openlocfilehash: 744e19165121d101a720a86bec0242fc31137768
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078483"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="5e87f-103">Тип ресурса teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="5e87f-103">teamGuestSettings resource type</span></span>

> <span data-ttu-id="5e87f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e87f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e87f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e87f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e87f-106">Параметры для настройки ли гости могут создать, обновить или удалить каналы в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="5e87f-106">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5e87f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e87f-107">Properties</span></span>
| <span data-ttu-id="5e87f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e87f-108">Property</span></span>     | <span data-ttu-id="5e87f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5e87f-109">Type</span></span>   |<span data-ttu-id="5e87f-110">Description</span><span class="sxs-lookup"><span data-stu-id="5e87f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e87f-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="5e87f-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="5e87f-112">Логический</span><span class="sxs-lookup"><span data-stu-id="5e87f-112">Boolean</span></span>|<span data-ttu-id="5e87f-113">Если параметр имеет значение true, Гости можно добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="5e87f-113">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="5e87f-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="5e87f-114">allowDeleteChannels</span></span>|<span data-ttu-id="5e87f-115">Логический</span><span class="sxs-lookup"><span data-stu-id="5e87f-115">Boolean</span></span>|<span data-ttu-id="5e87f-116">Если параметр имеет значение true, гости могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="5e87f-116">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e87f-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e87f-117">JSON representation</span></span>

<span data-ttu-id="5e87f-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e87f-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
