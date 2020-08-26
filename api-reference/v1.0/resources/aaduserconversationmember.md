---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9714605cabbc25d3eeae7a68b2bc8f09d6131836
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873456"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="350a0-103">Тип ресурса aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="350a0-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="350a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="350a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="350a0-105">Представляет пользователя Azure Active Directory в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="350a0-105">Represents an Azure Active Directory user in a [team](team.md).</span></span>
<span data-ttu-id="350a0-106">Этот тип наследуется от [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="350a0-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="350a0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="350a0-107">Properties</span></span>

| <span data-ttu-id="350a0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="350a0-108">Property</span></span>   | <span data-ttu-id="350a0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="350a0-109">Type</span></span> |<span data-ttu-id="350a0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="350a0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="350a0-111">id</span><span class="sxs-lookup"><span data-stu-id="350a0-111">id</span></span>|<span data-ttu-id="350a0-112">String</span><span class="sxs-lookup"><span data-stu-id="350a0-112">String</span></span>| <span data-ttu-id="350a0-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="350a0-113">Read-only.</span></span> <span data-ttu-id="350a0-114">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="350a0-114">Unique ID of the user.</span></span>|
|<span data-ttu-id="350a0-115">displayName</span><span class="sxs-lookup"><span data-stu-id="350a0-115">displayName</span></span>| <span data-ttu-id="350a0-116">string</span><span class="sxs-lookup"><span data-stu-id="350a0-116">string</span></span> | <span data-ttu-id="350a0-117">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="350a0-117">The display name of the user.</span></span> |
|<span data-ttu-id="350a0-118">roles</span><span class="sxs-lookup"><span data-stu-id="350a0-118">roles</span></span>| <span data-ttu-id="350a0-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="350a0-119">string collection</span></span> | <span data-ttu-id="350a0-120">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="350a0-120">The roles for that user.</span></span> |
|<span data-ttu-id="350a0-121">userId</span><span class="sxs-lookup"><span data-stu-id="350a0-121">userId</span></span>| <span data-ttu-id="350a0-122">строка</span><span class="sxs-lookup"><span data-stu-id="350a0-122">string</span></span> | <span data-ttu-id="350a0-123">GUID пользователя.</span><span class="sxs-lookup"><span data-stu-id="350a0-123">The guid of the user.</span></span> |
|<span data-ttu-id="350a0-124">email</span><span class="sxs-lookup"><span data-stu-id="350a0-124">email</span></span>| <span data-ttu-id="350a0-125">строка</span><span class="sxs-lookup"><span data-stu-id="350a0-125">string</span></span>  | <span data-ttu-id="350a0-126">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="350a0-126">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="350a0-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="350a0-127">JSON representation</span></span>

<span data-ttu-id="350a0-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="350a0-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
