---
title: Использование REST API уведомлений в Microsoft Graph
description: Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. Просто укажите учетную запись пользователя для отправки уведомления, и платформа доставит уведомление во все конечные точки устройства. Запросы API уведомлений выполняются от имени пользователя посредством делегированных разрешений и [разрешения на уведомления]( /graph/permissions_reference), которые можно использовать с учетными записями Майкрософт, рабочими или учебными учетными записями.
localization_priority: Priority
ms.prod: project-rome
doc_type: conceptualPageType
author: ''
ms.openlocfilehash: 2faaa7272ce1a093fc855d432c1992b9de150965
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009589"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="b6c8f-105">Использование REST API уведомлений в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b6c8f-105">Use the notifications REST API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6c8f-106">Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b6c8f-106">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="b6c8f-107">Просто укажите учетную запись пользователя для отправки уведомления, и платформа доставит уведомление во все конечные точки устройства.</span><span class="sxs-lookup"><span data-stu-id="b6c8f-107">Simply target a user account to send a notification to, and the platform will deliver the notification to all device endpoints.</span></span> <span data-ttu-id="b6c8f-108">Запросы API уведомлений выполняются от имени пользователя посредством [делегированных разрешений](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) и [разрешения на уведомления]( /graph/permissions_reference), которые можно использовать с учетными записями Майкрософт, рабочими или учебными учетными записями.</span><span class="sxs-lookup"><span data-stu-id="b6c8f-108">Notifications API requests are performed on behalf of a user via [delegated permissions](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) and the [notification permission]( /graph/permissions_reference), which can be used with either Microsoft accounts or work or school accounts.</span></span>
<span data-ttu-id="b6c8f-109">Этот тип уведомления, ориентированного на пользователя, представлен ресурсом [notification](../resources/projectrome-notification.md) и хранится в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b6c8f-109">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored in Microsoft Graph.</span></span> <span data-ttu-id="b6c8f-110">Доступ к нему и управление можно обеспечить путем публикации приложения с помощью [клиентских API SDK](https://github.com/Microsoft/project-rome).</span><span class="sxs-lookup"><span data-stu-id="b6c8f-110">It can then be accessed and managed by the publishing app via the [Project Rome SDK APIs](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="next-steps"></a><span data-ttu-id="b6c8f-111">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b6c8f-111">Next steps</span></span>
- <span data-ttu-id="b6c8f-112">См. статью [Ресурс notification](../resources/projectrome-notification.md) и создавайте уведомления для взаимодействия с пользователями.</span><span class="sxs-lookup"><span data-stu-id="b6c8f-112">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="b6c8f-113">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="b6c8f-113">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="b6c8f-114">Начните работу с использованием интеграции с клиентом, следуя инструкциям, указанным в [обзоре интеграции](/graph/notifications-integration-e2e-overview).</span><span class="sxs-lookup"><span data-stu-id="b6c8f-114">Get started with client integration, following the steps outlined in the [integration overview](/graph/notifications-integration-e2e-overview).</span></span>
