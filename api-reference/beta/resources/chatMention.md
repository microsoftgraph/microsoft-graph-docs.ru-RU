---
title: Тип ресурса chatMessageMention
description: 'Представляет упоминаются в сущности chatMessage. Упоминание может быть пользователь, группа, программа-робот или канала. '
localization_priority: Normal
ms.openlocfilehash: 7b24d2af6f61f3da69480557e1c5b5f32c009c25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876141"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="9a9f5-104">Тип ресурса chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="9a9f5-104">chatMessageMention resource type</span></span>

> <span data-ttu-id="9a9f5-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9a9f5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a9f5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a9f5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a9f5-107">Представляет упоминаются в сущности [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="9a9f5-107">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="9a9f5-108">Упоминание может быть пользователь, группа, программа-робот или канала.</span><span class="sxs-lookup"><span data-stu-id="9a9f5-108">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="9a9f5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a9f5-109">Properties</span></span>
| <span data-ttu-id="9a9f5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a9f5-110">Property</span></span>     | <span data-ttu-id="9a9f5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9a9f5-111">Type</span></span>   |<span data-ttu-id="9a9f5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9a9f5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a9f5-113">id</span><span class="sxs-lookup"><span data-stu-id="9a9f5-113">id</span></span>|<span data-ttu-id="9a9f5-114">строка</span><span class="sxs-lookup"><span data-stu-id="9a9f5-114">string</span></span>|<span data-ttu-id="9a9f5-115">Идентификатор сущности упоминаемые</span><span class="sxs-lookup"><span data-stu-id="9a9f5-115">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="9a9f5-116">mentionText</span><span class="sxs-lookup"><span data-stu-id="9a9f5-116">mentionText</span></span>|<span data-ttu-id="9a9f5-117">string</span><span class="sxs-lookup"><span data-stu-id="9a9f5-117">string</span></span>|<span data-ttu-id="9a9f5-118">Строка, используемая для представления упоминание Ex: отображаемое имя пользователя, имя группы и т.д.</span><span class="sxs-lookup"><span data-stu-id="9a9f5-118">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="9a9f5-119">упомянутые</span><span class="sxs-lookup"><span data-stu-id="9a9f5-119">mentioned</span></span>|[<span data-ttu-id="9a9f5-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="9a9f5-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="9a9f5-121">Пользователь, который был упомянут</span><span class="sxs-lookup"><span data-stu-id="9a9f5-121">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a9f5-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a9f5-122">JSON representation</span></span>

<span data-ttu-id="9a9f5-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a9f5-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
