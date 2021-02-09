---
title: Тип ресурса teamworkBot
description: Бот в экосистеме Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3413ee882a7ca387d298b148b37266704558031c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158319"
---
# <a name="teamworkbot-resource-type"></a><span data-ttu-id="7b48c-103">Тип ресурса teamworkBot</span><span class="sxs-lookup"><span data-stu-id="7b48c-103">teamworkBot resource type</span></span>

<span data-ttu-id="7b48c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b48c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b48c-105">Представляет бота в экосистеме Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7b48c-105">Represents a bot in the Microsoft Teams ecosystem.</span></span>

## <a name="methods"></a><span data-ttu-id="7b48c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7b48c-106">Methods</span></span>
|<span data-ttu-id="7b48c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7b48c-107">Method</span></span>|<span data-ttu-id="7b48c-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="7b48c-108">Return type</span></span>|<span data-ttu-id="7b48c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7b48c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7b48c-110">Получить бота</span><span class="sxs-lookup"><span data-stu-id="7b48c-110">Get bot</span></span>](../api/teamworkbot-get.md)|[<span data-ttu-id="7b48c-111">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="7b48c-111">teamworkBot</span></span>](../resources/teamworkbot.md)|<span data-ttu-id="7b48c-112">Чтение свойств и связей объекта [teamworkBot.](../resources/teamworkbot.md)</span><span class="sxs-lookup"><span data-stu-id="7b48c-112">Read the properties and relationships of a [teamworkBot](../resources/teamworkbot.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b48c-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b48c-113">Properties</span></span>
|<span data-ttu-id="7b48c-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b48c-114">Property</span></span>|<span data-ttu-id="7b48c-115">Тип</span><span class="sxs-lookup"><span data-stu-id="7b48c-115">Type</span></span>|<span data-ttu-id="7b48c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="7b48c-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b48c-117">id</span><span class="sxs-lookup"><span data-stu-id="7b48c-117">id</span></span>|<span data-ttu-id="7b48c-118">String</span><span class="sxs-lookup"><span data-stu-id="7b48c-118">String</span></span>|<span data-ttu-id="7b48c-119">ИД бота, связанного с определенным [teamsAppDefinition.](../resources/teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7b48c-119">The id of the bot associated with the specific [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span> <span data-ttu-id="7b48c-120">Обычно это значение является GUID.</span><span class="sxs-lookup"><span data-stu-id="7b48c-120">This value is usually a GUID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b48c-121">Связи</span><span class="sxs-lookup"><span data-stu-id="7b48c-121">Relationships</span></span>
<span data-ttu-id="7b48c-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7b48c-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b48c-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7b48c-123">JSON representation</span></span>
<span data-ttu-id="7b48c-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b48c-124">The following is a JSON representation of the resource.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7b48c-125">См. также</span><span class="sxs-lookup"><span data-stu-id="7b48c-125">See also</span></span>

- <span data-ttu-id="7b48c-126">Чтобы получить боты, установленные в команде, см. пример 2 в [списке приложений в команде.](../api/team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="7b48c-126">To get bots installed in a team, see example 2 in [List apps in team](../api/team-list-installedapps.md).</span></span>
- <span data-ttu-id="7b48c-127">Чтобы получить боты, установленные в чате, см. пример 2 в [списке приложений в чате.](../api/chat-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="7b48c-127">To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md).</span></span>
- <span data-ttu-id="7b48c-128">Чтобы получить боты, установленные в личной области пользователя, см. пример 2 в списке [приложений, установленных для пользователя.](../api/userteamwork-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="7b48c-128">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](../api/userteamwork-list-installedapps.md).</span></span>



