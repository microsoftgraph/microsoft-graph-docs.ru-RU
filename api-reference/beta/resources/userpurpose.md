---
title: Тип ресурса Усерпурпосе
description: Представляет получателя или тип почтового ящика пользователя в Exchange Online.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 83abf3bd19434867bbd162b6260ed5f4445d8ffd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057845"
---
# <a name="userpurpose-resource-type"></a><span data-ttu-id="7b919-103">Тип ресурса Усерпурпосе</span><span class="sxs-lookup"><span data-stu-id="7b919-103">userPurpose resource type</span></span>

<span data-ttu-id="7b919-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b919-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b919-105">Назначение почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7b919-105">The purpose of the mailbox.</span></span> <span data-ttu-id="7b919-106">Используется для различения почтового ящика одного пользователя из общего почтового ящика и почтового ящика оборудования в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="7b919-106">Used to differentiate a mailbox for a single user from a shared mailbox and equipment mailbox in Exchange Online.</span></span>


## <a name="properties"></a><span data-ttu-id="7b919-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b919-107">Properties</span></span>
|<span data-ttu-id="7b919-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b919-108">Property</span></span>|<span data-ttu-id="7b919-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7b919-109">Type</span></span>|<span data-ttu-id="7b919-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7b919-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b919-111">значение</span><span class="sxs-lookup"><span data-stu-id="7b919-111">value</span></span>|[<span data-ttu-id="7b919-112">маилбоксреЦипиенттипе</span><span class="sxs-lookup"><span data-stu-id="7b919-112">mailboxRecipientType</span></span>](#mailboxrecipienttype-values)|<span data-ttu-id="7b919-113">Представляет получателя или тип почтового ящика пользователя в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="7b919-113">Represents the user's recipient or mailbox type in Exchange Online.</span></span> <span data-ttu-id="7b919-114">Возможные значения: `unknown` ,, `user` , `linked` , `shared` `room` , `equipment` и `others` .</span><span class="sxs-lookup"><span data-stu-id="7b919-114">Possible values are: `unknown`, `user`, `linked`, `shared`, `room`, `equipment`, and `others`.</span></span> <span data-ttu-id="7b919-115">Более подробную информацию можно найти в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="7b919-115">See the next section for more information.</span></span>|

### <a name="mailboxrecipienttype-values"></a><span data-ttu-id="7b919-116">значения МаилбоксреЦипиенттипе</span><span class="sxs-lookup"><span data-stu-id="7b919-116">mailboxRecipientType values</span></span>
|<span data-ttu-id="7b919-117">Member</span><span class="sxs-lookup"><span data-stu-id="7b919-117">Member</span></span>|<span data-ttu-id="7b919-118">Описание</span><span class="sxs-lookup"><span data-stu-id="7b919-118">Description</span></span>|
|:---------------|:--------|
|<span data-ttu-id="7b919-119">unknown</span><span class="sxs-lookup"><span data-stu-id="7b919-119">unknown</span></span>|<span data-ttu-id="7b919-120">Сведения о почтовом ящике не найдены.</span><span class="sxs-lookup"><span data-stu-id="7b919-120">No information found about the mailbox.</span></span>|
|<span data-ttu-id="7b919-121">user</span><span class="sxs-lookup"><span data-stu-id="7b919-121">user</span></span>|<span data-ttu-id="7b919-122">Учетная запись пользователя с почтовым ящиком в локальном лесе.</span><span class="sxs-lookup"><span data-stu-id="7b919-122">A user account with a mailbox in the local forest.</span></span>|
|<span data-ttu-id="7b919-123">вязывает</span><span class="sxs-lookup"><span data-stu-id="7b919-123">linked</span></span>|<span data-ttu-id="7b919-124">Почтовый ящик, связанный с учетной записью пользователя в другом лесе.</span><span class="sxs-lookup"><span data-stu-id="7b919-124">A mailbox linked to a user account in another forest.</span></span>|
|<span data-ttu-id="7b919-125">общие</span><span class="sxs-lookup"><span data-stu-id="7b919-125">shared</span></span>|<span data-ttu-id="7b919-126">Почтовые ящики, используемые двумя или более учетными записями пользователей.</span><span class="sxs-lookup"><span data-stu-id="7b919-126">A mailbox shared by two or more user accounts.</span></span>|
|<span data-ttu-id="7b919-127">отеле</span><span class="sxs-lookup"><span data-stu-id="7b919-127">room</span></span>|<span data-ttu-id="7b919-128">Почтовый ящик, представляющий комнату переговоров.</span><span class="sxs-lookup"><span data-stu-id="7b919-128">A mailbox representing a conference room.</span></span>|
|<span data-ttu-id="7b919-129">перифери</span><span class="sxs-lookup"><span data-stu-id="7b919-129">equipment</span></span>|<span data-ttu-id="7b919-130">Почтовый ящик, представляющий компонент оборудования.</span><span class="sxs-lookup"><span data-stu-id="7b919-130">A mailbox representing a piece of equipment.</span></span>|
|<span data-ttu-id="7b919-131">владельцев</span><span class="sxs-lookup"><span data-stu-id="7b919-131">others</span></span>|<span data-ttu-id="7b919-132">Найден почтовый ящик, но цель пользователя отличается от указанных выше.</span><span class="sxs-lookup"><span data-stu-id="7b919-132">Mailbox found but user purpose is different from the ones specified above.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b919-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7b919-133">JSON representation</span></span>

<span data-ttu-id="7b919-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b919-134">Here is a JSON representation of the resource.</span></span>

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


