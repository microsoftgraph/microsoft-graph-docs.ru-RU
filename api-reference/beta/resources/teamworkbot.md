---
title: Тип ресурса teamworkBot
description: Бот в экосистеме Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 383c646fdb30d082daa73e37fd227238db195b6b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706498"
---
# <a name="teamworkbot-resource-type"></a><span data-ttu-id="aa4bc-103">Тип ресурса teamworkBot</span><span class="sxs-lookup"><span data-stu-id="aa4bc-103">teamworkBot resource type</span></span>

<span data-ttu-id="aa4bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa4bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa4bc-105">Представляет бота в экосистеме Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="aa4bc-105">Represents a bot in the Microsoft Teams ecosystem.</span></span>

## <a name="methods"></a><span data-ttu-id="aa4bc-106">Методы</span><span class="sxs-lookup"><span data-stu-id="aa4bc-106">Methods</span></span>
|<span data-ttu-id="aa4bc-107">Метод</span><span class="sxs-lookup"><span data-stu-id="aa4bc-107">Method</span></span>|<span data-ttu-id="aa4bc-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="aa4bc-108">Return type</span></span>|<span data-ttu-id="aa4bc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aa4bc-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa4bc-110">Получить бота</span><span class="sxs-lookup"><span data-stu-id="aa4bc-110">Get bot</span></span>](../api/teamworkbot-get.md)|[<span data-ttu-id="aa4bc-111">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="aa4bc-111">teamworkBot</span></span>](../resources/teamworkbot.md)|<span data-ttu-id="aa4bc-112">Чтение свойств и связей объекта [teamworkBot.](../resources/teamworkbot.md)</span><span class="sxs-lookup"><span data-stu-id="aa4bc-112">Read the properties and relationships of a [teamworkBot](../resources/teamworkbot.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa4bc-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa4bc-113">Properties</span></span>
|<span data-ttu-id="aa4bc-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa4bc-114">Property</span></span>|<span data-ttu-id="aa4bc-115">Тип</span><span class="sxs-lookup"><span data-stu-id="aa4bc-115">Type</span></span>|<span data-ttu-id="aa4bc-116">Описание</span><span class="sxs-lookup"><span data-stu-id="aa4bc-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa4bc-117">id</span><span class="sxs-lookup"><span data-stu-id="aa4bc-117">id</span></span>|<span data-ttu-id="aa4bc-118">String</span><span class="sxs-lookup"><span data-stu-id="aa4bc-118">String</span></span>|<span data-ttu-id="aa4bc-119">ИД бота, связанного с определенным [teamsAppDefinition.](../resources/teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="aa4bc-119">The id of the bot associated with the specific [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span> <span data-ttu-id="aa4bc-120">Обычно это значение является GUID.</span><span class="sxs-lookup"><span data-stu-id="aa4bc-120">This value is usually a GUID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa4bc-121">Связи</span><span class="sxs-lookup"><span data-stu-id="aa4bc-121">Relationships</span></span>
<span data-ttu-id="aa4bc-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aa4bc-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa4bc-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aa4bc-123">JSON representation</span></span>
<span data-ttu-id="aa4bc-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa4bc-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkBot",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "String (identifier)"
}
```

## <a name="see-also"></a><span data-ttu-id="aa4bc-125">См. также</span><span class="sxs-lookup"><span data-stu-id="aa4bc-125">See also</span></span>

- <span data-ttu-id="aa4bc-126">Чтобы получить ботов, установленных в команде, см. пример 2 в [списке приложений в команде.](../api/team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="aa4bc-126">To get bots installed in a team, see example 2 in [List apps in team](../api/team-list-installedapps.md).</span></span>
- <span data-ttu-id="aa4bc-127">Чтобы получить боты, установленные в чате, см. пример 2 в [списке приложений в чате.](../api/chat-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="aa4bc-127">To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md).</span></span>
- <span data-ttu-id="aa4bc-128">Чтобы получить боты, установленные в личной области пользователя, см. пример 2 в списке [приложений, установленных для пользователя.](../api/userteamwork-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="aa4bc-128">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](../api/userteamwork-list-installedapps.md).</span></span>



