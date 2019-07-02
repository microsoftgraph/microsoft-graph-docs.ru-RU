---
title: 'Используйте API Microsoft Graph для интеграции функций социальной и рабочей аналитики '
description: Microsoft Graph поддерживает социальные жесты в социальном контексте пользователя и предоставляет доступ к полезным сведениям о пользователях и к социальным данным.
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: 0118902f42984a541c750f34db945bc0e7ede5f2
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35417677"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-and-workplace-intelligence-in-an-app"></a><span data-ttu-id="4348a-103">Используйте API Microsoft Graph для интеграции функций социальной и рабочей аналитики </span><span class="sxs-lookup"><span data-stu-id="4348a-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4348a-104">Microsoft Graph поддерживает социальные жесты в социальном контексте пользователя и предоставляет доступ к полезным сведениям о пользователях и социальным данным.</span><span class="sxs-lookup"><span data-stu-id="4348a-104">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="4348a-105">Сбор и извлечение определенных сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="4348a-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="4348a-106">Используйте ресурс [person](../resources/person.md) и API службы "Люди" для сбора сведений о пользователе, полученных из его почты, контактов и социальных сетей.</span><span class="sxs-lookup"><span data-stu-id="4348a-106">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="4348a-107">Результаты упорядочиваются по релевантности на основании множества отношений общения, совместной работы и бизнес-связей.</span><span class="sxs-lookup"><span data-stu-id="4348a-107">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="4348a-108">Вы можете просматривать, сортировать, отбирать, фильтровать или искать сведения о пользователях, основываясь на заданных условиях.</span><span class="sxs-lookup"><span data-stu-id="4348a-108">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="4348a-109">Получение списка людей</span><span class="sxs-lookup"><span data-stu-id="4348a-109">List people</span></span>](../api/user-list-people.md)

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="4348a-110">Помогите пользователям получить наиболее важные документы для работы</span><span class="sxs-lookup"><span data-stu-id="4348a-110">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="4348a-111">Используйте API аналитики для определения наиболее важных документов для пользователя:</span><span class="sxs-lookup"><span data-stu-id="4348a-111">Use the insights API to identify the most relevant documents for a user:</span></span> 

- <span data-ttu-id="4348a-112">Список [популярных документов](../api/insights-list-trending.md) пользователя</span><span class="sxs-lookup"><span data-stu-id="4348a-112">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="4348a-113">Список документов, [используемых](../api/insights-list-used.md) пользователем</span><span class="sxs-lookup"><span data-stu-id="4348a-113">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="4348a-114">Список документов, [к которым пользователю предоставлен доступ или к которым пользователь предоставил доступ](../api/insights-list-shared.md)</span><span class="sxs-lookup"><span data-stu-id="4348a-114">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>

## <a name="manage--mentions"></a><span data-ttu-id="4348a-115">Управление @упоминаниями</span><span class="sxs-lookup"><span data-stu-id="4348a-115">Manage @-Mentions</span></span>

<span data-ttu-id="4348a-116">Упоминание получателя в сообщении для уведомления и привлечения его внимания является распространенным социальным жестом.</span><span class="sxs-lookup"><span data-stu-id="4348a-116">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="4348a-117">Ресурс [mention](../resources/mention.md) и API упоминаний предоставляют простой механизм для упоминания получателя в [сообщении](../resources/message.md), получения всех сообщений, в которых пользователь отмечен с помощью @упоминания, или получения всех упоминаний в сообщении.</span><span class="sxs-lookup"><span data-stu-id="4348a-117">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="4348a-118">Создание упоминаний в новом сообщении</span><span class="sxs-lookup"><span data-stu-id="4348a-118">Create mentions in a new message</span></span>

  - [<span data-ttu-id="4348a-119">Создание и отправка упоминаний в составе нового сообщения</span><span class="sxs-lookup"><span data-stu-id="4348a-119">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="4348a-120">Создание упоминания в составе черновика сообщения</span><span class="sxs-lookup"><span data-stu-id="4348a-120">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="4348a-121">Получение сведений об упоминаниях в сообщении</span><span class="sxs-lookup"><span data-stu-id="4348a-121">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="4348a-122">Получение всех сообщений в почтовом ящике вошедшего пользователя, в которых упоминается пользователь</span><span class="sxs-lookup"><span data-stu-id="4348a-122">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="4348a-123">Получение сведений о каждом упоминании в сообщении</span><span class="sxs-lookup"><span data-stu-id="4348a-123">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="4348a-124">[Удаление упоминания](../api/message-delete.md#request-2) в сообщении</span><span class="sxs-lookup"><span data-stu-id="4348a-124">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

