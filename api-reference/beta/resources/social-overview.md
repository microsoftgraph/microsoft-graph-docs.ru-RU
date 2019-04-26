---
title: Интегрирование социальной аналитики в приложение с помощью Microsoft Graph API
description: Microsoft Graph поддерживает социальные жесты в социальном контексте пользователя и предоставляет доступ к полезным сведениям о пользователях и социальным данным.
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: 45482d2e47c97b6c09302ab60ff9c031cef1e92a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345718"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a><span data-ttu-id="45a61-103">Интегрирование социальной аналитики в приложение с помощью Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="45a61-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45a61-104">Microsoft Graph поддерживает социальные жесты в социальном контексте пользователя и предоставляет доступ к полезным сведениям о пользователях и социальным данным.</span><span class="sxs-lookup"><span data-stu-id="45a61-104">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="45a61-105">Сбор и извлечение определенных сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="45a61-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="45a61-106">Используйте ресурс [person](../resources/person.md) и API службы "Люди" для сбора сведений о пользователе, полученных из его почты, контактов и социальных сетей.</span><span class="sxs-lookup"><span data-stu-id="45a61-106">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="45a61-107">Результаты упорядочиваются по релевантности на основании множества отношений общения, совместной работы и бизнес-связей.</span><span class="sxs-lookup"><span data-stu-id="45a61-107">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="45a61-108">Вы можете просматривать, сортировать, отбирать, фильтровать или искать сведения о пользователях, основываясь на заданных условиях.</span><span class="sxs-lookup"><span data-stu-id="45a61-108">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="45a61-109">Получение списка людей</span><span class="sxs-lookup"><span data-stu-id="45a61-109">List people</span></span>](../api/user-list-people.md)

## <a name="manage--mentions"></a><span data-ttu-id="45a61-110">Управление @упоминаниями</span><span class="sxs-lookup"><span data-stu-id="45a61-110">Manage @-Mentions</span></span>

<span data-ttu-id="45a61-111">Упоминание получателя в сообщении для уведомления и привлечения его внимания является распространенным социальным жестом.</span><span class="sxs-lookup"><span data-stu-id="45a61-111">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="45a61-112">Ресурс [mention](../resources/mention.md) и API упоминаний предоставляют простой механизм для упоминания получателя в [сообщении](../resources/message.md), получения всех сообщений, в которых пользователь отмечен с помощью @упоминания, или получения всех упоминаний в сообщении.</span><span class="sxs-lookup"><span data-stu-id="45a61-112">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="45a61-113">Создание упоминаний в новом сообщении</span><span class="sxs-lookup"><span data-stu-id="45a61-113">Create mentions in a new message</span></span>

  - [<span data-ttu-id="45a61-114">Создание и отправка упоминаний в составе нового сообщения</span><span class="sxs-lookup"><span data-stu-id="45a61-114">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="45a61-115">Создание упоминания в составе черновика сообщения</span><span class="sxs-lookup"><span data-stu-id="45a61-115">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="45a61-116">Получение сведений об упоминаниях в сообщении</span><span class="sxs-lookup"><span data-stu-id="45a61-116">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="45a61-117">Получение всех сообщений в почтовом ящике вошедшего пользователя, в которых упоминается пользователь</span><span class="sxs-lookup"><span data-stu-id="45a61-117">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="45a61-118">Получение сведений о каждом упоминании в сообщении</span><span class="sxs-lookup"><span data-stu-id="45a61-118">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="45a61-119">[Удаление упоминания](../api/message-delete.md#request-2) в сообщении</span><span class="sxs-lookup"><span data-stu-id="45a61-119">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

## <a name="access-social-data-around-and-about-a-user"></a><span data-ttu-id="45a61-120">Доступ к социальным данным о пользователе</span><span class="sxs-lookup"><span data-stu-id="45a61-120">Access social data around and about a user</span></span>

<span data-ttu-id="45a61-121">Office Graph собирает отношения между различными объектами в Office 365.</span><span class="sxs-lookup"><span data-stu-id="45a61-121">Office Graph encapsulates the relationships between different entities in Office 365.</span></span> <span data-ttu-id="45a61-122">С помощью Office Graph можно получать социальную аналитику по отдельным пользователям в Office 365.</span><span class="sxs-lookup"><span data-stu-id="45a61-122">Use Office Graph to get social insights into individual users across Office 365.</span></span>

- <span data-ttu-id="45a61-123">Перечисление [популярных](../api/insights-list-trending.md) элементов, связанных с пользователем</span><span class="sxs-lookup"><span data-stu-id="45a61-123">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="45a61-124">Перечисление пользователей, [работавших](../api/user-list-people.md) с пользователем</span><span class="sxs-lookup"><span data-stu-id="45a61-124">List users who have been [working with](../api/user-list-people.md) a user</span></span>
