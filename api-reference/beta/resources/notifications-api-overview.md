---
title: Использование REST API уведомлений в Microsoft Graph
description: Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. .
localization_priority: Priority
ms.prod: notifications
doc_type: conceptualPageType
author: merzink
ms.openlocfilehash: 96b27aa9a57c26666ae9b4fc09c4dadca52b8d6a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033659"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="f9729-104">Использование REST API уведомлений в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f9729-104">Use the notifications REST API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9729-105">Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f9729-105">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="f9729-106">Просто отправьте уведомление целевому пользователю, и платформа доставит его во все конечные точки устройств, зарегистрированные для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f9729-106">Simply post a notification to your target user, and the platform will deliver the notification to all device endpoints registered to that user.</span></span> <span data-ttu-id="f9729-107">На высоком уровне процесс выглядит так:</span><span class="sxs-lookup"><span data-stu-id="f9729-107">The high-level flow is as follows:</span></span>

1. <span data-ttu-id="f9729-108">Пользователь входит в приложение, которое создает подписку в службе уведомлений Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f9729-108">User signs in to your application, which creates a subscription with the Microsoft Graph notification service.</span></span> <span data-ttu-id="f9729-109">Приложению, отправившему вызов, будет возвращен конкретный идентификатор подписки на уведомления пользователя, или UNSID.</span><span class="sxs-lookup"><span data-stu-id="f9729-109">A specific user notification subscription ID or UNSID will be returned to the calling application.</span></span>
2. <span data-ttu-id="f9729-110">Приложение отправляет этот UNSID в службу приложений.</span><span class="sxs-lookup"><span data-stu-id="f9729-110">The application sends this UNSID to your application service.</span></span>
3. <span data-ttu-id="f9729-111">Когда служба приложений будет готова отправить уведомление, она [проходит проверку подлинности на платформе удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) и отправляет уведомление через службу уведомлений Microsoft Graph, предоставляя маркер проверки подлинности, UNSID целевого пользователя и полезные данные уведомления.</span><span class="sxs-lookup"><span data-stu-id="f9729-111">When ready to send a notification, your application service [authenticates with the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) and posts a notification via the Microsoft Graph notification service, providing the auth token, target user's UNSID, and notification payload.</span></span>
4. <span data-ttu-id="f9729-112">Служба уведомлений Microsoft Graph рассылает уведомления всем конечным точкам пользователя с активной подпиской.</span><span class="sxs-lookup"><span data-stu-id="f9729-112">The Microsoft Graph notification service fans-out notifications to all endpoints of the user with an active subscription.</span></span>  

<span data-ttu-id="f9729-113">Уведомления такого типа, ориентированные на пользователя, представлены ресурсом [notification](../resources/projectrome-notification.md) и хранятся в службе уведомлений Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f9729-113">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored within the Microsoft Graph notification service.</span></span> <span data-ttu-id="f9729-114">Доступ к нему и управление осуществляется клиентским приложением с помощью [клиентских API SDK](https://aka.ms/GNSDK).</span><span class="sxs-lookup"><span data-stu-id="f9729-114">It can then be accessed and managed by the client application via the [client-side SDK APIs](https://aka.ms/GNSDK).</span></span> <span data-ttu-id="f9729-115">Если вы впервые работаете со службой уведомлений Microsoft Graph, ознакомьтесь с дополнительными сведениями в разделе [обзора уведомлений](https://docs.microsoft.com/graph/notifications-concept-overview).</span><span class="sxs-lookup"><span data-stu-id="f9729-115">If you're new to the Microsoft Graph notification service, check out the [notification overview](https://docs.microsoft.com/graph/notifications-concept-overview) section to learn more.</span></span>    

## <a name="whats-new"></a><span data-ttu-id="f9729-116">Что нового</span><span class="sxs-lookup"><span data-stu-id="f9729-116">What's new</span></span>
<span data-ttu-id="f9729-117">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="f9729-117">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f9729-118">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f9729-118">Next steps</span></span>
- <span data-ttu-id="f9729-119">См. статью [Ресурс notification](../resources/projectrome-notification.md) и создавайте уведомления для взаимодействия с пользователями.</span><span class="sxs-lookup"><span data-stu-id="f9729-119">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="f9729-120">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="f9729-120">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="f9729-121">Приступите к интеграции клиента, следуя инструкциями из [обзора интеграции](/graph/notifications-integration-e2e-overview).</span><span class="sxs-lookup"><span data-stu-id="f9729-121">Get started with client integration by following the steps in the [integration overview](/graph/notifications-integration-e2e-overview) topic.</span></span>


