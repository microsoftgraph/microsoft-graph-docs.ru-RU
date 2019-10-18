---
title: Использование API Microsoft Graph для интеграции функций социальной и рабочей аналитики в приложении
description: Microsoft Graph обеспечивает доступ к полезным социальным и рабочим данным для пользователей, а также поддерживает социальные жесты в социальном контексте пользователя.
localization_priority: Priority
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 74beb2a66f103342f6dbc5e5977200751a309c08
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450671"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-and-workplace-intelligence-in-an-app"></a><span data-ttu-id="65756-103">Использование API Microsoft Graph для интеграции функций социальной и рабочей аналитики в приложении</span><span class="sxs-lookup"><span data-stu-id="65756-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65756-104">Microsoft Graph обеспечивает доступ к социальным и рабочим данным для пользователей, а также поддерживает жесты в социальном контексте пользователя.</span><span class="sxs-lookup"><span data-stu-id="65756-104">Microsoft Graph enables access to social and workplace data for people, and supports gestures in a user's social context.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="65756-105">Сбор и извлечение определенных сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="65756-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="65756-106">Используйте ресурс [person](../resources/person.md) и API службы "Люди" для сбора сведений о пользователе, полученных из его почты, контактов и социальных сетей.</span><span class="sxs-lookup"><span data-stu-id="65756-106">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="65756-107">Результаты упорядочиваются по релевантности на основании множества отношений общения, совместной работы и бизнес-связей.</span><span class="sxs-lookup"><span data-stu-id="65756-107">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="65756-108">Вы можете просматривать, сортировать, отбирать, фильтровать или искать сведения о пользователях, основываясь на заданных условиях.</span><span class="sxs-lookup"><span data-stu-id="65756-108">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="65756-109">Получение списка людей</span><span class="sxs-lookup"><span data-stu-id="65756-109">List people</span></span>](../api/user-list-people.md)

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="65756-110">Помогите пользователям получить наиболее важные документы для работы</span><span class="sxs-lookup"><span data-stu-id="65756-110">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="65756-111">Используйте API аналитики для определения наиболее важных документов для пользователя:</span><span class="sxs-lookup"><span data-stu-id="65756-111">Use the insights API to identify the most relevant documents for a user:</span></span>

- <span data-ttu-id="65756-112">Список [популярных документов](../api/insights-list-trending.md) пользователя</span><span class="sxs-lookup"><span data-stu-id="65756-112">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="65756-113">Список документов, [используемых](../api/insights-list-used.md) пользователем</span><span class="sxs-lookup"><span data-stu-id="65756-113">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="65756-114">Список документов, [к которым пользователю предоставлен доступ или к которым пользователь предоставил доступ](../api/insights-list-shared.md)</span><span class="sxs-lookup"><span data-stu-id="65756-114">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>

## <a name="help-users-gain-insights-into-their-work-patterns"></a><span data-ttu-id="65756-115">Помощь пользователям в получении аналитики рабочих закономерностей</span><span class="sxs-lookup"><span data-stu-id="65756-115">Help users gain insights into their work patterns</span></span>

<span data-ttu-id="65756-116">Используйте API аналитики, чтобы получить статистику о действиях и соответствующие параметры для пользователя:</span><span class="sxs-lookup"><span data-stu-id="65756-116">Use the analytics API to get activity statistics and related settings for a user:</span></span>

- <span data-ttu-id="65756-117">[settings](../resources/settings.md). Чтобы API аналитики возвращал результаты для пользователя, в параметрах аналитики текущего пользователя должна отображаться действительная лицензия MyAnalytics, должно быть выбрано использование MyAnalytics и должен применяться облачный почтовый ящик с поддержкой Graph.</span><span class="sxs-lookup"><span data-stu-id="65756-117">[settings](../resources/settings.md): For the analytics API to return results for a user, the current user analytics settings must show a valid MyAnalytics license, be opted in to using MyAnalytics, and have a cloud-hosted mailbox that’s graph-enabled.</span></span>
- <span data-ttu-id="65756-118">[activityStatistics](../resources/activitystatistics.md). Получение данных за последнюю полную неделю (или указанный промежуток времени) для действий в Office 365, выполнявшихся пользователем, включая количество часов, потраченное на [звонки](callactivitystatistics.md), [чаты (мгновенные сообщения)](chatactivitystatistics.md), [письма](emailactivitystatistics.md) и [собрания](meetingactivitystatistics.md) в течение и вне рабочего времени, а также часы, доступные для [сосредоточенной работы](focusactivitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="65756-118">[activityStatistics](../resources/activitystatistics.md): Gets data for the last complete week (or the specified time range) for the Office 365 activities that a user spent time on, including the number of hours spent on [calls](callactivitystatistics.md), [chats (instant messages)](chatactivitystatistics.md), [email](emailactivitystatistics.md), and [meetings](meetingactivitystatistics.md) during and outside of working hours and the number of hours available for [focused work](focusactivitystatistics.md).</span></span>

## <a name="manage--mentions"></a><span data-ttu-id="65756-119">Управление @упоминаниями</span><span class="sxs-lookup"><span data-stu-id="65756-119">Manage @-Mentions</span></span>

<span data-ttu-id="65756-120">Упоминание получателя в сообщении для уведомления и привлечения его внимания является распространенным социальным жестом.</span><span class="sxs-lookup"><span data-stu-id="65756-120">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="65756-121">Ресурс [mention](../resources/mention.md) и API упоминаний предоставляют простой механизм для упоминания получателя в [сообщении](../resources/message.md), получения всех сообщений, в которых пользователь отмечен с помощью @упоминания, или получения всех упоминаний в сообщении.</span><span class="sxs-lookup"><span data-stu-id="65756-121">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="65756-122">Создание упоминаний в новом сообщении</span><span class="sxs-lookup"><span data-stu-id="65756-122">Create mentions in a new message</span></span>

  - [<span data-ttu-id="65756-123">Создание и отправка упоминаний в составе нового сообщения</span><span class="sxs-lookup"><span data-stu-id="65756-123">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="65756-124">Создание упоминания в составе черновика сообщения</span><span class="sxs-lookup"><span data-stu-id="65756-124">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="65756-125">Получение сведений об упоминаниях в сообщении</span><span class="sxs-lookup"><span data-stu-id="65756-125">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="65756-126">Получение всех сообщений в почтовом ящике вошедшего пользователя, в которых упоминается пользователь</span><span class="sxs-lookup"><span data-stu-id="65756-126">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="65756-127">Получение сведений о каждом упоминании в сообщении</span><span class="sxs-lookup"><span data-stu-id="65756-127">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="65756-128">[Удаление упоминания](../api/message-delete.md#request-2) в сообщении</span><span class="sxs-lookup"><span data-stu-id="65756-128">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>
