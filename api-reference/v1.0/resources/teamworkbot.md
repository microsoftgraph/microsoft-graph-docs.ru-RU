---
title: тип ресурса teamworkBot
description: Бот в экосистеме Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99bdde9a4ff26945dd5aa040f2741fdf50c1273b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476440"
---
# <a name="teamworkbot-resource-type"></a><span data-ttu-id="ec28b-103">тип ресурса teamworkBot</span><span class="sxs-lookup"><span data-stu-id="ec28b-103">teamworkBot resource type</span></span>

<span data-ttu-id="ec28b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec28b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec28b-105">Представляет бот в экосистеме Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ec28b-105">Represents a bot in the Microsoft Teams ecosystem.</span></span>

## <a name="methods"></a><span data-ttu-id="ec28b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ec28b-106">Methods</span></span>
|<span data-ttu-id="ec28b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ec28b-107">Method</span></span>|<span data-ttu-id="ec28b-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="ec28b-108">Return type</span></span>|<span data-ttu-id="ec28b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ec28b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ec28b-110">Получить бот</span><span class="sxs-lookup"><span data-stu-id="ec28b-110">Get bot</span></span>](../api/teamworkbot-get.md)|[<span data-ttu-id="ec28b-111">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="ec28b-111">teamworkBot</span></span>](../resources/teamworkbot.md)|<span data-ttu-id="ec28b-112">Ознакомьтесь с свойствами и отношениями объекта [teamworkBot.](../resources/teamworkbot.md)</span><span class="sxs-lookup"><span data-stu-id="ec28b-112">Read the properties and relationships of a [teamworkBot](../resources/teamworkbot.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ec28b-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec28b-113">Properties</span></span>
|<span data-ttu-id="ec28b-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec28b-114">Property</span></span>|<span data-ttu-id="ec28b-115">Тип</span><span class="sxs-lookup"><span data-stu-id="ec28b-115">Type</span></span>|<span data-ttu-id="ec28b-116">Описание</span><span class="sxs-lookup"><span data-stu-id="ec28b-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec28b-117">id</span><span class="sxs-lookup"><span data-stu-id="ec28b-117">id</span></span>|<span data-ttu-id="ec28b-118">String</span><span class="sxs-lookup"><span data-stu-id="ec28b-118">String</span></span>|<span data-ttu-id="ec28b-119">ID бота, связанного с [определенными группамиAppDefinition.](../resources/teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ec28b-119">The ID of the bot associated with the specific [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span> <span data-ttu-id="ec28b-120">Это значение обычно является GUID.</span><span class="sxs-lookup"><span data-stu-id="ec28b-120">This value is usually a GUID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec28b-121">Связи</span><span class="sxs-lookup"><span data-stu-id="ec28b-121">Relationships</span></span>
<span data-ttu-id="ec28b-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ec28b-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec28b-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ec28b-123">JSON representation</span></span>
<span data-ttu-id="ec28b-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec28b-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkBot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "String (identifier)"
}
```

## <a name="see-also"></a><span data-ttu-id="ec28b-125">См. также</span><span class="sxs-lookup"><span data-stu-id="ec28b-125">See also</span></span>

- <span data-ttu-id="ec28b-126">Чтобы получить боты, установленные в команде, см. пример 2 в [списке приложений в команде.](../api/team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="ec28b-126">To get bots installed in a team, see example 2 in [List apps in team](../api/team-list-installedapps.md).</span></span> <!-- - To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md). -->
- <span data-ttu-id="ec28b-127">Чтобы получить боты, установленные в личной области пользователя, см. пример 2 в [приложениях List, установленных для пользователя.](../api/userteamwork-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="ec28b-127">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](../api/userteamwork-list-installedapps.md).</span></span>



