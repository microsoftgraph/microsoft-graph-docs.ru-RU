---
title: Тип ресурса chatMessageMention
description: 'Представляет упоминаются в сущности chatMessage. Упоминание может быть пользователь, группа, программа-робот или канала. '
ms.openlocfilehash: 5f1e427b0ed2b8ffcfbc86417beb4719dc6fb2a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075099"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="f776e-104">Тип ресурса chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="f776e-104">chatMessageMention resource type</span></span>

> <span data-ttu-id="f776e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f776e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f776e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f776e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f776e-107">Представляет упоминаются в сущности [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="f776e-107">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="f776e-108">Упоминание может быть пользователь, группа, программа-робот или канала.</span><span class="sxs-lookup"><span data-stu-id="f776e-108">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="f776e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f776e-109">Properties</span></span>
| <span data-ttu-id="f776e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f776e-110">Property</span></span>     | <span data-ttu-id="f776e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f776e-111">Type</span></span>   |<span data-ttu-id="f776e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f776e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f776e-113">id</span><span class="sxs-lookup"><span data-stu-id="f776e-113">id</span></span>|<span data-ttu-id="f776e-114">строка</span><span class="sxs-lookup"><span data-stu-id="f776e-114">string</span></span>|<span data-ttu-id="f776e-115">Идентификатор сущности упоминаемые</span><span class="sxs-lookup"><span data-stu-id="f776e-115">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="f776e-116">mentionText</span><span class="sxs-lookup"><span data-stu-id="f776e-116">mentionText</span></span>|<span data-ttu-id="f776e-117">string</span><span class="sxs-lookup"><span data-stu-id="f776e-117">string</span></span>|<span data-ttu-id="f776e-118">Строка, используемая для представления упоминание Ex: отображаемое имя пользователя, имя группы и т.д.</span><span class="sxs-lookup"><span data-stu-id="f776e-118">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="f776e-119">упомянутые</span><span class="sxs-lookup"><span data-stu-id="f776e-119">mentioned</span></span>|[<span data-ttu-id="f776e-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="f776e-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="f776e-121">Пользователь, который был упомянут</span><span class="sxs-lookup"><span data-stu-id="f776e-121">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f776e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f776e-122">JSON representation</span></span>

<span data-ttu-id="f776e-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f776e-123">The following is a JSON representation of the resource.</span></span>

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
