---
title: Использование Microsoft Graph API для интеграции социальных аналитики в приложении
description: Microsoft Graph поддерживает социальных жесты в социальных контекста пользователя и предоставляет доступ к полезным пользователей и социального контента.
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: 3ccc574a966c5a0dc81f62fe4fa0a595fb25a982
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944882"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a><span data-ttu-id="f406f-103">Использование Microsoft Graph API для интеграции социальных аналитики в приложении</span><span class="sxs-lookup"><span data-stu-id="f406f-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

> <span data-ttu-id="f406f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f406f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f406f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f406f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f406f-106">Microsoft Graph поддерживает социальных жесты в социальных контекста пользователя и предоставляет доступ к полезным пользователей и социального контента.</span><span class="sxs-lookup"><span data-stu-id="f406f-106">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="f406f-107">Статистические и извлеките конкретные сведения о пользователях</span><span class="sxs-lookup"><span data-stu-id="f406f-107">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="f406f-108">Использование ресурсов [человека](../resources/person.md) и API людей и статистические данные о сотруднике из почты, контакты и социальными сетями.</span><span class="sxs-lookup"><span data-stu-id="f406f-108">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="f406f-109">Результаты сортируются по релевантности, их на основе нескольких связи, совместной работы и деловыми отношениями.</span><span class="sxs-lookup"><span data-stu-id="f406f-109">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="f406f-110">Этот API позволяет Обзор сортировки, выбор, фильтра и поиска для пользователей на основе критериев.</span><span class="sxs-lookup"><span data-stu-id="f406f-110">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="f406f-111">List people</span><span class="sxs-lookup"><span data-stu-id="f406f-111">List people</span></span>](../api/user-list-people.md)

## <a name="manage--mentions"></a><span data-ttu-id="f406f-112">Управление частотой упоминания</span><span class="sxs-lookup"><span data-stu-id="f406f-112">Manage @-Mentions</span></span>

<span data-ttu-id="f406f-113">Вызов получателя для уведомления и получение внимания получателя в сообщение — это общие социальных жестам.</span><span class="sxs-lookup"><span data-stu-id="f406f-113">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="f406f-114">Ресурс [упомянуть](../resources/mention.md) и API упоминания предоставление механизма простых выноска получателя в [сообщение](../resources/message.md), получение всех сообщений, в которых пользователь получает уведомление с помощью @ Упоминание или получение каждого упоминаются в сообщение.</span><span class="sxs-lookup"><span data-stu-id="f406f-114">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="f406f-115">Создание упоминания в новые сообщения</span><span class="sxs-lookup"><span data-stu-id="f406f-115">Create mentions in a new message</span></span>

  - [<span data-ttu-id="f406f-116">Создание и отправка упоминания как часть нового сообщения</span><span class="sxs-lookup"><span data-stu-id="f406f-116">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="f406f-117">Создание упоминания как часть черновика сообщения</span><span class="sxs-lookup"><span data-stu-id="f406f-117">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="f406f-118">Получение сведений о упоминания в сообщение</span><span class="sxs-lookup"><span data-stu-id="f406f-118">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="f406f-119">Получение всех сообщений в почтовый ящик пользователя выполнил вход, упомянуть пользователя</span><span class="sxs-lookup"><span data-stu-id="f406f-119">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="f406f-120">Подробные сведения о каждом упоминаются в сообщение</span><span class="sxs-lookup"><span data-stu-id="f406f-120">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="f406f-121">[Удаление упоминаются](../api/message-delete.md#request-2) в сообщение</span><span class="sxs-lookup"><span data-stu-id="f406f-121">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

## <a name="access-social-data-around-and-about-a-user"></a><span data-ttu-id="f406f-122">Access социального контента решения, а также о пользователя</span><span class="sxs-lookup"><span data-stu-id="f406f-122">Access social data around and about a user</span></span>

<span data-ttu-id="f406f-123">Графическое представление Office инкапсулирует связи между разными организациями в Office 365.</span><span class="sxs-lookup"><span data-stu-id="f406f-123">Office Graph encapsulates the relationships between different entities in Office 365.</span></span> <span data-ttu-id="f406f-124">Использование Office график для получения наблюдения из социальных сетей в отдельных пользователей в Office 365.</span><span class="sxs-lookup"><span data-stu-id="f406f-124">Use Office Graph to get social insights into individual users across Office 365.</span></span>

- <span data-ttu-id="f406f-125">Список элементов [тенденции вокруг](../api/insights-list-trending.md) пользователя</span><span class="sxs-lookup"><span data-stu-id="f406f-125">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="f406f-126">Список пользователей, которые были [Работа с](../api/user-list-people.md) пользователем</span><span class="sxs-lookup"><span data-stu-id="f406f-126">List users who have been [working with](../api/user-list-people.md) a user</span></span>
