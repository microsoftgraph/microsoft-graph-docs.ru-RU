---
title: Тип ресурса teamworkBot
description: Бот в экосистеме Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8c21e7ab3b88c2659bf055e39b931cbc6e9d2f39
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844678"
---
# <a name="teamworkbot-resource-type"></a><span data-ttu-id="74ce6-103">Тип ресурса teamworkBot</span><span class="sxs-lookup"><span data-stu-id="74ce6-103">teamworkBot resource type</span></span>

<span data-ttu-id="74ce6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74ce6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74ce6-105">Представляет бота в экосистеме Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="74ce6-105">Represents a bot in the Microsoft Teams ecosystem.</span></span>

## <a name="methods"></a><span data-ttu-id="74ce6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="74ce6-106">Methods</span></span>
|<span data-ttu-id="74ce6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="74ce6-107">Method</span></span>|<span data-ttu-id="74ce6-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="74ce6-108">Return type</span></span>|<span data-ttu-id="74ce6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="74ce6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="74ce6-110">Получить бота</span><span class="sxs-lookup"><span data-stu-id="74ce6-110">Get bot</span></span>](../api/teamworkbot-get.md)|[<span data-ttu-id="74ce6-111">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="74ce6-111">teamworkBot</span></span>](../resources/teamworkbot.md)|<span data-ttu-id="74ce6-112">Чтение свойств и связей объекта [teamworkBot.](../resources/teamworkbot.md)</span><span class="sxs-lookup"><span data-stu-id="74ce6-112">Read the properties and relationships of a [teamworkBot](../resources/teamworkbot.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="74ce6-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="74ce6-113">Properties</span></span>
|<span data-ttu-id="74ce6-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="74ce6-114">Property</span></span>|<span data-ttu-id="74ce6-115">Тип</span><span class="sxs-lookup"><span data-stu-id="74ce6-115">Type</span></span>|<span data-ttu-id="74ce6-116">Описание</span><span class="sxs-lookup"><span data-stu-id="74ce6-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74ce6-117">id</span><span class="sxs-lookup"><span data-stu-id="74ce6-117">id</span></span>|<span data-ttu-id="74ce6-118">String</span><span class="sxs-lookup"><span data-stu-id="74ce6-118">String</span></span>|<span data-ttu-id="74ce6-119">ИД бота, связанного с определенным [teamsAppDefinition.](../resources/teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="74ce6-119">The id of the bot associated with the specific [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span> <span data-ttu-id="74ce6-120">Обычно это значение является GUID.</span><span class="sxs-lookup"><span data-stu-id="74ce6-120">This value is usually a GUID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74ce6-121">Связи</span><span class="sxs-lookup"><span data-stu-id="74ce6-121">Relationships</span></span>
<span data-ttu-id="74ce6-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="74ce6-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74ce6-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="74ce6-123">JSON representation</span></span>
<span data-ttu-id="74ce6-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74ce6-124">The following is a JSON representation of the resource.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="74ce6-125">См. также</span><span class="sxs-lookup"><span data-stu-id="74ce6-125">See also</span></span>

- <span data-ttu-id="74ce6-126">Чтобы получить ботов, установленных в команде, см. пример 2 в [списке приложений в команде.](../api/team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="74ce6-126">To get bots installed in a team, see example 2 in [List apps in team](../api/team-list-installedapps.md).</span></span>
- <span data-ttu-id="74ce6-127">Чтобы получить боты, установленные в чате, см. пример 2 в [списке приложений в чате.](../api/chat-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="74ce6-127">To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md).</span></span>
- <span data-ttu-id="74ce6-128">Чтобы получить боты, установленные в личной области пользователя, см. пример 2 в списке [приложений, установленных для пользователя.](../api/userteamwork-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="74ce6-128">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](../api/userteamwork-list-installedapps.md).</span></span>



