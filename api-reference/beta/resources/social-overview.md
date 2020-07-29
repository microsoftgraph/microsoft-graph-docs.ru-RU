---
title: Использование API Microsoft Graph для интеграции функций социальной и рабочей аналитики в приложении
description: Microsoft Graph обеспечивает доступ к полезным данным о пользователях, их профиле, документах, с которыми они взаимодействуют, их рабочих привычках, а также поддерживает социальные жесты в социальном контексте пользователя.
localization_priority: Priority
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 86a8142882d9a9471ad128ca960ca3840cea7cca
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427475"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-and-workplace-intelligence-in-an-app"></a><span data-ttu-id="29270-103">Использование API Microsoft Graph для интеграции функций социальной и рабочей аналитики в приложении</span><span class="sxs-lookup"><span data-stu-id="29270-103">Use the Microsoft Graph API to integrate people and workplace intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29270-104">Microsoft Graph обеспечивает доступ к полезным данным о пользователях, их профиле, документах, с которыми они взаимодействуют, их рабочих привычках, а также поддерживает социальные жесты в социальном контексте пользователя.</span><span class="sxs-lookup"><span data-stu-id="29270-104">Microsoft Graph enables access to useful data about people, their profile, documents they interact with, and work patterns, and supports gestures in a user's social context.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="29270-105">Сбор и извлечение определенных сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="29270-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="29270-106">Функция: люди</span><span class="sxs-lookup"><span data-stu-id="29270-106">Feature: People</span></span>

<span data-ttu-id="29270-107">Используйте ресурс [person](../resources/person.md) и API службы "Люди" для сбора сведений о пользователе, полученных из его почты, контактов и социальных сетей.</span><span class="sxs-lookup"><span data-stu-id="29270-107">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="29270-108">Результаты упорядочиваются по релевантности на основании множества отношений общения, совместной работы и бизнес-связей.</span><span class="sxs-lookup"><span data-stu-id="29270-108">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="29270-109">Вы можете просматривать, сортировать, отбирать, фильтровать или искать сведения о пользователях, основываясь на заданных условиях.</span><span class="sxs-lookup"><span data-stu-id="29270-109">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="29270-110">Получение списка людей</span><span class="sxs-lookup"><span data-stu-id="29270-110">List people</span></span>](../api/user-list-people.md)

## <a name="help-users-contextualize-others-in-their-organization"></a><span data-ttu-id="29270-111">Помощь пользователям в получении контекстных сведений о других сотрудниках организации</span><span class="sxs-lookup"><span data-stu-id="29270-111">Help users contextualize others in their organization</span></span>

<span data-ttu-id="29270-112">Функция: профиль (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="29270-112">Feature: Profile (preview)</span></span>

<span data-ttu-id="29270-113">Люди, которые хотят получить контекстные сведения о других сотрудниках организации, обычно просматривают профиль или карточку соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="29270-113">People who seek to contextualize others within their organization commonly view a person's profile or profile card.</span></span> 

<span data-ttu-id="29270-114">Ресурс [profile](../resources/profile.md) является богатым источником информации о пользователях в клиенте, который предоставляет удобный механизм хранения и получения информации о людях.</span><span class="sxs-lookup"><span data-stu-id="29270-114">The [profile](../resources/profile.md) resource is a rich source of information about people within a tenant and provides a lightweight mechanism for storing and retrieving information about a person.</span></span> 

## <a name="personalize-people-experiences-within-your-organization"></a><span data-ttu-id="29270-115">Персонализация пользовательского интерфейса в организации</span><span class="sxs-lookup"><span data-stu-id="29270-115">Personalize people experiences within your organization</span></span>

<span data-ttu-id="29270-116">Функция: настройка карточки профиля (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="29270-116">Feature: Profile card customization (preview)</span></span>

<span data-ttu-id="29270-117">Предоставляет администратору возможность настроить сведения, указанные в карточке профиля, которая используется в Microsoft 365 в организации.</span><span class="sxs-lookup"><span data-stu-id="29270-117">Provides the ability for an administrator to customize the information shown on the profile card used across Microsoft 365 within their organization.</span></span>

<span data-ttu-id="29270-118">Ресурс [profileCardProperty](../resources/profileCardProperty.md) представляет атрибут пользователя на карточке профиля Microsoft 365 для организации, который отображается в общем интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="29270-118">The [profileCardProperty](../resources/profileCardProperty.md) resource represents an attribute of a user on the Microsoft 365 profile card for an organization to surface in a shared, people experience.</span></span>

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="29270-119">Помощь пользователям в получении наиболее важных документов для работы</span><span class="sxs-lookup"><span data-stu-id="29270-119">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="29270-120">Функция: аналитика на основе документов</span><span class="sxs-lookup"><span data-stu-id="29270-120">Feature: Document insights</span></span>

<span data-ttu-id="29270-121">Используйте API аналитики для определения наиболее важных документов для пользователя:</span><span class="sxs-lookup"><span data-stu-id="29270-121">Use the insights API to identify the most relevant documents for a user:</span></span>

- <span data-ttu-id="29270-122">Список [популярных документов](../api/insights-list-trending.md) пользователя</span><span class="sxs-lookup"><span data-stu-id="29270-122">List documents [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="29270-123">Список документов, [используемых](../api/insights-list-used.md) пользователем</span><span class="sxs-lookup"><span data-stu-id="29270-123">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="29270-124">Список документов, [к которым пользователю предоставлен доступ или к которым пользователь предоставил доступ](../api/insights-list-shared.md)</span><span class="sxs-lookup"><span data-stu-id="29270-124">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>
- <span data-ttu-id="29270-125">Изучите способы [настройки параметров конфиденциальности для аналитики элементов](/graph/insights-customize-item-insights-privacy.md) в организации.</span><span class="sxs-lookup"><span data-stu-id="29270-125">Explore ways to [customize privacy settings for item insights](/graph/insights-customize-item-insights-privacy.md) in an organization.</span></span>

## <a name="manage--mentions"></a><span data-ttu-id="29270-126">Управление @упоминаниями</span><span class="sxs-lookup"><span data-stu-id="29270-126">Manage @-Mentions</span></span>

<span data-ttu-id="29270-127">Функция: @упоминания (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="29270-127">Feature: @-mentions (preview)</span></span>

<span data-ttu-id="29270-128">Упоминание получателя в сообщении для уведомления и привлечения его внимания является распространенным социальным жестом.</span><span class="sxs-lookup"><span data-stu-id="29270-128">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="29270-129">Ресурс [mention](../resources/mention.md) и API упоминаний предоставляют простой механизм для упоминания получателя в [сообщении](../resources/message.md), получения всех сообщений, в которых пользователь отмечен с помощью @упоминания, или получения всех упоминаний в сообщении.</span><span class="sxs-lookup"><span data-stu-id="29270-129">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="29270-130">Создание упоминаний в новом сообщении</span><span class="sxs-lookup"><span data-stu-id="29270-130">Create mentions in a new message</span></span>

  - [<span data-ttu-id="29270-131">Создание и отправка упоминаний в составе нового сообщения</span><span class="sxs-lookup"><span data-stu-id="29270-131">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="29270-132">Создание упоминания в составе черновика сообщения</span><span class="sxs-lookup"><span data-stu-id="29270-132">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="29270-133">Получение сведений об упоминаниях в сообщении</span><span class="sxs-lookup"><span data-stu-id="29270-133">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="29270-134">Получение всех сообщений в почтовом ящике вошедшего пользователя, в которых упоминается пользователь</span><span class="sxs-lookup"><span data-stu-id="29270-134">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="29270-135">Получение сведений о каждом упоминании в сообщении</span><span class="sxs-lookup"><span data-stu-id="29270-135">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="29270-136">[Удаление упоминания](../api/message-delete.md#request-2) в сообщении</span><span class="sxs-lookup"><span data-stu-id="29270-136">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>


## <a name="help-users-gain-insights-into-their-work-patterns"></a><span data-ttu-id="29270-137">Помощь пользователям в получении аналитики рабочих закономерностей</span><span class="sxs-lookup"><span data-stu-id="29270-137">Help users gain insights into their work patterns</span></span>

<span data-ttu-id="29270-138">Функция: аналитика (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="29270-138">Feature: Analytics (preview)</span></span>

<span data-ttu-id="29270-139">Используйте API аналитики, чтобы получить статистику о действиях и соответствующие параметры для пользователя:</span><span class="sxs-lookup"><span data-stu-id="29270-139">Use the analytics API to get activity statistics and related settings for a user:</span></span>

- <span data-ttu-id="29270-140">[settings](../resources/settings.md). Чтобы API аналитики возвращал результаты для пользователя, в параметрах аналитики текущего пользователя должна отображаться действительная лицензия MyAnalytics, должно быть выбрано использование MyAnalytics и должен применяться облачный почтовый ящик с поддержкой Graph.</span><span class="sxs-lookup"><span data-stu-id="29270-140">[settings](../resources/settings.md): For the analytics API to return results for a user, the current user analytics settings must show a valid MyAnalytics license, be opted in to using MyAnalytics, and have a cloud-hosted mailbox that’s graph-enabled.</span></span>
- <span data-ttu-id="29270-141">[activityStatistics](../resources/activitystatistics.md). Получение данных за последнюю полную неделю (или указанный промежуток времени) о действиях в Microsoft 365, выполненных пользователем, включая количество часов, потраченное на [звонки](callactivitystatistics.md), [чаты (мгновенные сообщения)](chatactivitystatistics.md), [письма](emailactivitystatistics.md) и [собрания](meetingactivitystatistics.md) в течение и вне рабочего времени, а также часы, доступные для [сосредоточенной работы](focusactivitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="29270-141">[activityStatistics](../resources/activitystatistics.md): Gets data for the last complete week (or the specified time range) for the Microsoft 365 activities that a user spent time on, including the number of hours spent on [calls](callactivitystatistics.md), [chats (instant messages)](chatactivitystatistics.md), [email](emailactivitystatistics.md), and [meetings](meetingactivitystatistics.md) during and outside of working hours and the number of hours available for [focused work](focusactivitystatistics.md).</span></span>

## <a name="whats-new"></a><span data-ttu-id="29270-142">Новые возможности</span><span class="sxs-lookup"><span data-stu-id="29270-142">What's new</span></span>
<span data-ttu-id="29270-143">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этих наборов API.</span><span class="sxs-lookup"><span data-stu-id="29270-143">Find out about the [latest new features and updates](/graph/whats-new-overview) for these API sets.</span></span>
