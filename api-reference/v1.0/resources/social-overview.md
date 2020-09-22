---
title: Интегрирование аналитики о людях в приложение с помощью Microsoft Graph API
description: Microsoft Graph позволяет получить доступ к полезным сведениям о людях и документах, с которыми они взаимодействуют.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 154762d1658503a25ffe2ec39bdf602f4a9d2b8d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970546"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-intelligence-in-an-app"></a><span data-ttu-id="fa45d-103">Интегрирование аналитики о людях в приложение с помощью Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="fa45d-103">Use the Microsoft Graph API to integrate people intelligence in an app</span></span>

<span data-ttu-id="fa45d-104">Microsoft Graph позволяет получить доступ к полезным сведениям о людях и документах, с которыми они взаимодействуют.</span><span class="sxs-lookup"><span data-stu-id="fa45d-104">Microsoft Graph enables access to useful data about people and documents they interact with.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="fa45d-105">Сбор и извлечение определенных сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="fa45d-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="fa45d-106">Функция: люди</span><span class="sxs-lookup"><span data-stu-id="fa45d-106">Feature: People</span></span>

<span data-ttu-id="fa45d-107">Можно использовать ресурс [person](../resources/person.md) и API службы "Люди" для сбора сведений о пользователе, полученных из его почты, контактов и социальных сетей.</span><span class="sxs-lookup"><span data-stu-id="fa45d-107">You can use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="fa45d-108">Результаты упорядочиваются по релевантности на основании множества шаблонов общения и совместной работы, а также его бизнес-связями.</span><span class="sxs-lookup"><span data-stu-id="fa45d-108">The results are ordered by their relevance based on multiple communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="fa45d-109">Вы можете просматривать, сортировать, отбирать, фильтровать или искать сведения о пользователях, основываясь на заданных условиях.</span><span class="sxs-lookup"><span data-stu-id="fa45d-109">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

<span data-ttu-id="fa45d-110">Со сценариями и примерами можно ознакомиться в статье [Получение сведений о релевантных людях](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="fa45d-110">For scenarios and examples, see [Get information about relevant people](/graph/people-example).</span></span>

<span data-ttu-id="fa45d-111">Чтобы использовать API, ознакомьтесь со следующими материалами:</span><span class="sxs-lookup"><span data-stu-id="fa45d-111">To use the API, see the following:</span></span>

- [<span data-ttu-id="fa45d-112">Получение списка людей</span><span class="sxs-lookup"><span data-stu-id="fa45d-112">List people</span></span>](../api/user-list-people.md)


## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="fa45d-113">Помощь пользователям в получении наиболее важных документов для работы</span><span class="sxs-lookup"><span data-stu-id="fa45d-113">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="fa45d-114">Функция: аналитика на основе документов</span><span class="sxs-lookup"><span data-stu-id="fa45d-114">Feature: Document insights</span></span>

<span data-ttu-id="fa45d-115">Используйте API аналитики для определения наиболее важных документов для пользователя:</span><span class="sxs-lookup"><span data-stu-id="fa45d-115">Use the insights API to identify the most relevant documents for a user:</span></span>

- <span data-ttu-id="fa45d-116">Список [популярных документов](../api/insights-list-trending.md) пользователя</span><span class="sxs-lookup"><span data-stu-id="fa45d-116">List documents [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="fa45d-117">Список документов, [используемых](../api/insights-list-used.md) пользователем</span><span class="sxs-lookup"><span data-stu-id="fa45d-117">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="fa45d-118">Список документов, [к которым пользователю предоставлен доступ или к которым пользователь предоставил доступ](../api/insights-list-shared.md)</span><span class="sxs-lookup"><span data-stu-id="fa45d-118">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>

## <a name="whats-new"></a><span data-ttu-id="fa45d-119">Что нового</span><span class="sxs-lookup"><span data-stu-id="fa45d-119">What's new</span></span>
<span data-ttu-id="fa45d-120">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="fa45d-120">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>
