---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d53709726c55cc3ac9f2051bd499a996b33d9c36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028359"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="65142-103">Тип ресурса aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="65142-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="65142-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65142-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65142-105">Представляет пользователя Azure Active Directory в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="65142-105">Represents an Azure Active Directory user in a [team](team.md).</span></span>
<span data-ttu-id="65142-106">Этот тип наследуется от [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="65142-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="65142-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="65142-107">Properties</span></span>

| <span data-ttu-id="65142-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="65142-108">Property</span></span>   | <span data-ttu-id="65142-109">Тип</span><span class="sxs-lookup"><span data-stu-id="65142-109">Type</span></span> |<span data-ttu-id="65142-110">Описание</span><span class="sxs-lookup"><span data-stu-id="65142-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65142-111">id</span><span class="sxs-lookup"><span data-stu-id="65142-111">id</span></span>|<span data-ttu-id="65142-112">String</span><span class="sxs-lookup"><span data-stu-id="65142-112">String</span></span>| <span data-ttu-id="65142-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65142-113">Read-only.</span></span> <span data-ttu-id="65142-114">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="65142-114">Unique ID of the user.</span></span>|
|<span data-ttu-id="65142-115">displayName</span><span class="sxs-lookup"><span data-stu-id="65142-115">displayName</span></span>| <span data-ttu-id="65142-116">string</span><span class="sxs-lookup"><span data-stu-id="65142-116">string</span></span> | <span data-ttu-id="65142-117">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="65142-117">The display name of the user.</span></span> |
|<span data-ttu-id="65142-118">roles</span><span class="sxs-lookup"><span data-stu-id="65142-118">roles</span></span>| <span data-ttu-id="65142-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65142-119">string collection</span></span> | <span data-ttu-id="65142-120">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="65142-120">The roles for that user.</span></span> |
|<span data-ttu-id="65142-121">userId</span><span class="sxs-lookup"><span data-stu-id="65142-121">userId</span></span>| <span data-ttu-id="65142-122">строка</span><span class="sxs-lookup"><span data-stu-id="65142-122">string</span></span> | <span data-ttu-id="65142-123">GUID пользователя.</span><span class="sxs-lookup"><span data-stu-id="65142-123">The guid of the user.</span></span> |
|<span data-ttu-id="65142-124">email</span><span class="sxs-lookup"><span data-stu-id="65142-124">email</span></span>| <span data-ttu-id="65142-125">строка</span><span class="sxs-lookup"><span data-stu-id="65142-125">string</span></span>  | <span data-ttu-id="65142-126">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="65142-126">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="65142-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65142-127">JSON representation</span></span>

<span data-ttu-id="65142-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65142-128">The following is a JSON representation of the resource.</span></span>

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

