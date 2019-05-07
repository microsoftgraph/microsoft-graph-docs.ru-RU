---
title: Перенос приложений Azure AD Graph в Microsoft Graph
description: Описывается перенос приложений API Azure Active Directory (Azure AD) в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 348bc7632c2e2e158d41bb1cc2da9fa3ea755ca6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630232"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a><span data-ttu-id="c35f2-103">Перенос приложений Azure AD Graph в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c35f2-103">Migrate Azure AD Graph apps to Microsoft Graph</span></span>

<span data-ttu-id="c35f2-104">Microsoft Graph полностью заменяет Graph Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c35f2-104">Microsoft Graph is fully replacing Azure Active Directory (Azure AD) Graph.</span></span> <span data-ttu-id="c35f2-105">Для большинства рабочих приложений Microsoft Graph уже может полностью поддерживать сценарии Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c35f2-105">For most production apps, Microsoft Graph can already fully support Azure AD scenarios.</span></span> <span data-ttu-id="c35f2-106">Теперь вы должны начать перемещение приложений Azure AD Graph в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c35f2-106">You should start moving your Azure AD Graph apps to Microsoft Graph now.</span></span>

<span data-ttu-id="c35f2-107">Кроме того, Microsoft Graph поддерживает множество новых наборов данных Azure AD и функций, недоступных в Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="c35f2-107">In addition, Microsoft Graph supports many new Azure AD datasets and features that are not available in Azure AD Graph.</span></span> <span data-ttu-id="c35f2-108">Переключитесь на Microsoft Graph, чтобы воспользоваться всеми преимуществами этих новых API, используя одну конечную точку, в том числе:</span><span class="sxs-lookup"><span data-stu-id="c35f2-108">Switch to Microsoft Graph to take advantage of these new APIs, all through one single endpoint, including:</span></span>

- [<span data-ttu-id="c35f2-109">Управление группами Office 365</span><span class="sxs-lookup"><span data-stu-id="c35f2-109">Office 365 group management</span></span>](/graph/office365-groups-concept-overview)
- [<span data-ttu-id="c35f2-110">Приглашения внешних пользователей</span><span class="sxs-lookup"><span data-stu-id="c35f2-110">External user invitations</span></span>](/graph/api/resources/invitation?view=graph-rest-1.0)
- <span data-ttu-id="c35f2-111">Возможность [восстановления пользователей и групп Office 365](/graph/api/resources/directory?view=graph-rest-1.0) после их удаления</span><span class="sxs-lookup"><span data-stu-id="c35f2-111">The ability to [restore users and Office 365 groups](/graph/api/resources/directory?view=graph-rest-1.0) after they've been deleted</span></span>
- [<span data-ttu-id="c35f2-112">Уведомления веб-перехватчика для пользователей и групп</span><span class="sxs-lookup"><span data-stu-id="c35f2-112">Webhook notifications on users and groups</span></span>](/graph/webhooks?toc=./ref/toc.json&view=graph-rest-1.0)
- <span data-ttu-id="c35f2-113">Функции управления удостоверениями, такие как:</span><span class="sxs-lookup"><span data-stu-id="c35f2-113">Identity governance features such as:</span></span>
  - <span data-ttu-id="c35f2-114">[Привилегированное управление удостоверениями](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) для повышения уровня доступа пользователей к привилегированным ролям только при необходимости и в течение ограниченного периода времени.</span><span class="sxs-lookup"><span data-stu-id="c35f2-114">[Privileged identity management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) to elevate users to privileged roles only when needed and for a limited time period</span></span>
  - <span data-ttu-id="c35f2-115">[Проверка доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta) для одноразовых или повторяющихся проверок доступа для аттестации прав доступа пользователя</span><span class="sxs-lookup"><span data-stu-id="c35f2-115">[Access reviews](/graph/api/resources/accessreviews-root?view=graph-rest-beta) for one-time or recurring access reviews for attestation of user's access rights</span></span>
  - <span data-ttu-id="c35f2-116">[Условия использования](/graph/api/resources/accessreviews-root?view=graph-rest-beta) для предоставления организациям сведений о юридических или нормативных требованиях, таких как уведомления об отказе от ответственности</span><span class="sxs-lookup"><span data-stu-id="c35f2-116">[Terms-of-use](/graph/api/resources/accessreviews-root?view=graph-rest-beta) to enable organizations to present information for legal or compliance requirements, like disclaimer notices</span></span>
- <span data-ttu-id="c35f2-117">Функции безопасности, такие как:</span><span class="sxs-lookup"><span data-stu-id="c35f2-117">Security features such as:</span></span>
  - [<span data-ttu-id="c35f2-118">События с риском для идентификации</span><span class="sxs-lookup"><span data-stu-id="c35f2-118">Identity risk events</span></span>](/graph/api/resources/identityriskevent?view=graph-rest-beta)
  - [<span data-ttu-id="c35f2-119">Рискованные пользователи</span><span class="sxs-lookup"><span data-stu-id="c35f2-119">Risky users</span></span>](/graph/api/resources/riskyuser?view=graph-rest-beta)
- <span data-ttu-id="c35f2-120">[Клиентские библиотеки и примеры](/graph/) доступны на многих других платформах и языках</span><span class="sxs-lookup"><span data-stu-id="c35f2-120">[Client libraries and samples](/graph/) available on many more platforms and languages</span></span>

<span data-ttu-id="c35f2-121">Microsoft Graph предоставляет доступ к большому количеству дополнительных служб, чем просто Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c35f2-121">Microsoft Graph offers access to many more services than just Azure Active Directory.</span></span> <span data-ttu-id="c35f2-122">Он также имеет [шлюз API для Microsoft 365 Services](/graph/).</span><span class="sxs-lookup"><span data-stu-id="c35f2-122">It's the [API gateway to Microsoft 365 services too](/graph/).</span></span>

<span data-ttu-id="c35f2-123">Остальные статьи в этом разделе помогут переместить приложение из Azure AD Graph в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c35f2-123">The rest of the articles in this section help you move your app from Azure AD Graph to Microsoft Graph.</span></span> <span data-ttu-id="c35f2-124">Вы найдете:</span><span class="sxs-lookup"><span data-stu-id="c35f2-124">You'll find:</span></span>

- <span data-ttu-id="c35f2-125">Контрольный список, который поможет вам спланировать.</span><span class="sxs-lookup"><span data-stu-id="c35f2-125">A checklist to help you plan.</span></span>
- <span data-ttu-id="c35f2-126">Руководство по определенным различиям между API.</span><span class="sxs-lookup"><span data-stu-id="c35f2-126">Guidance describing specific differences between the APIs.</span></span>
- <span data-ttu-id="c35f2-127">Ссылки на дополнительные ресурсы и примеры, иллюстрирующие конкретные различия.</span><span class="sxs-lookup"><span data-stu-id="c35f2-127">Links to additional resources and examples to illustrate specific differences.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c35f2-128">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="c35f2-128">Next Steps</span></span>

- <span data-ttu-id="c35f2-129">Изучите [Контрольный список миграции приложений](migrate-azure-ad-graph-planning-checklist.md) , чтобы помочь вам спланировать перемещение.</span><span class="sxs-lookup"><span data-stu-id="c35f2-129">Walk through the [app migration checklist](migrate-azure-ad-graph-planning-checklist.md) to help you plan the move.</span></span>
- <span data-ttu-id="c35f2-130">Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="c35f2-130">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="c35f2-131">Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .</span><span class="sxs-lookup"><span data-stu-id="c35f2-131">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
- <span data-ttu-id="c35f2-132">Чтобы узнать больше об обновлениях хода выполнения и временных шкалах, ознакомьтесь со статьей [Microsoft Graph или Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) в центре разработчиков Office.</span><span class="sxs-lookup"><span data-stu-id="c35f2-132">To learn more about progress updates and timelines, see [Microsoft Graph or the Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) in the Office Dev Center.</span></span>
