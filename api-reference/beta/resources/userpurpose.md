---
title: Тип ресурса Усерпурпосе
description: Представляет получателя или тип почтового ящика пользователя в Exchange Online.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: b4ed5db9dfa87b2829d78371339c166c3bb74265
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846378"
---
# <a name="userpurpose-resource-type"></a><span data-ttu-id="2b26a-103">Тип ресурса Усерпурпосе</span><span class="sxs-lookup"><span data-stu-id="2b26a-103">userPurpose resource type</span></span>

<span data-ttu-id="2b26a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b26a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b26a-105">Назначение почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2b26a-105">The purpose of the mailbox.</span></span> <span data-ttu-id="2b26a-106">Используется для различения почтового ящика одного пользователя из общего почтового ящика и почтового ящика оборудования в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="2b26a-106">Used to differentiate a mailbox for a single user from a shared mailbox and equipment mailbox in Exchange Online.</span></span>


## <a name="properties"></a><span data-ttu-id="2b26a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b26a-107">Properties</span></span>
|<span data-ttu-id="2b26a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b26a-108">Property</span></span>|<span data-ttu-id="2b26a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2b26a-109">Type</span></span>|<span data-ttu-id="2b26a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2b26a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b26a-111">значение</span><span class="sxs-lookup"><span data-stu-id="2b26a-111">value</span></span>|[<span data-ttu-id="2b26a-112">маилбоксреЦипиенттипе</span><span class="sxs-lookup"><span data-stu-id="2b26a-112">mailboxRecipientType</span></span>](#mailboxrecipienttype-values)|<span data-ttu-id="2b26a-113">Представляет получателя или тип почтового ящика пользователя в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="2b26a-113">Represents the user's recipient or mailbox type in Exchange Online.</span></span> <span data-ttu-id="2b26a-114">Возможные значения: `unknown` ,, `user` , `linked` , `shared` `room` , `equipment` и `others` .</span><span class="sxs-lookup"><span data-stu-id="2b26a-114">Possible values are: `unknown`, `user`, `linked`, `shared`, `room`, `equipment`, and `others`.</span></span> <span data-ttu-id="2b26a-115">Более подробную информацию можно найти в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="2b26a-115">See the next section for more information.</span></span>|

### <a name="mailboxrecipienttype-values"></a><span data-ttu-id="2b26a-116">значения МаилбоксреЦипиенттипе</span><span class="sxs-lookup"><span data-stu-id="2b26a-116">mailboxRecipientType values</span></span>
|<span data-ttu-id="2b26a-117">Member</span><span class="sxs-lookup"><span data-stu-id="2b26a-117">Member</span></span>|<span data-ttu-id="2b26a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="2b26a-118">Description</span></span>|
|:---------------|:--------|
|<span data-ttu-id="2b26a-119">unknown</span><span class="sxs-lookup"><span data-stu-id="2b26a-119">unknown</span></span>|<span data-ttu-id="2b26a-120">Сведения о почтовом ящике не найдены.</span><span class="sxs-lookup"><span data-stu-id="2b26a-120">No information found about the mailbox.</span></span>|
|<span data-ttu-id="2b26a-121">пользователь;</span><span class="sxs-lookup"><span data-stu-id="2b26a-121">user</span></span>|<span data-ttu-id="2b26a-122">Учетная запись пользователя с почтовым ящиком в локальном лесе.</span><span class="sxs-lookup"><span data-stu-id="2b26a-122">A user account with a mailbox in the local forest.</span></span>|
|<span data-ttu-id="2b26a-123">вязывает</span><span class="sxs-lookup"><span data-stu-id="2b26a-123">linked</span></span>|<span data-ttu-id="2b26a-124">Почтовый ящик, связанный с учетной записью пользователя в другом лесе.</span><span class="sxs-lookup"><span data-stu-id="2b26a-124">A mailbox linked to a user account in another forest.</span></span>|
|<span data-ttu-id="2b26a-125">общие</span><span class="sxs-lookup"><span data-stu-id="2b26a-125">shared</span></span>|<span data-ttu-id="2b26a-126">Почтовые ящики, используемые двумя или более учетными записями пользователей.</span><span class="sxs-lookup"><span data-stu-id="2b26a-126">A mailbox shared by two or more user accounts.</span></span>|
|<span data-ttu-id="2b26a-127">отеле</span><span class="sxs-lookup"><span data-stu-id="2b26a-127">room</span></span>|<span data-ttu-id="2b26a-128">Почтовый ящик, представляющий комнату переговоров.</span><span class="sxs-lookup"><span data-stu-id="2b26a-128">A mailbox representing a conference room.</span></span>|
|<span data-ttu-id="2b26a-129">перифери</span><span class="sxs-lookup"><span data-stu-id="2b26a-129">equipment</span></span>|<span data-ttu-id="2b26a-130">Почтовый ящик, представляющий компонент оборудования.</span><span class="sxs-lookup"><span data-stu-id="2b26a-130">A mailbox representing a piece of equipment.</span></span>|
|<span data-ttu-id="2b26a-131">владельцев</span><span class="sxs-lookup"><span data-stu-id="2b26a-131">others</span></span>|<span data-ttu-id="2b26a-132">Найден почтовый ящик, но цель пользователя отличается от указанных выше.</span><span class="sxs-lookup"><span data-stu-id="2b26a-132">Mailbox found but user purpose is different from the ones specified above.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b26a-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b26a-133">JSON representation</span></span>

<span data-ttu-id="2b26a-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b26a-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userPurpose"
}-->

```json
{
    "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userPurpose resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
