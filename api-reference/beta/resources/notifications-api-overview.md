---
title: Использование REST API уведомлений в Microsoft Graph
description: Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. Просто укажите учетную запись пользователя для отправки уведомления, и платформа доставит уведомление во все конечные точки устройства. Запросы API уведомлений выполняются от имени пользователя посредством делегированных разрешений и [разрешения на уведомления]( /graph/permissions_reference), которые можно использовать с учетными записями Майкрософт, рабочими или учебными учетными записями.
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 243f412162ed1427c766272d02d58c57ba47cf42
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342102"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="54696-105">Использование REST API уведомлений в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="54696-105">Use the notifications REST API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54696-106">Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="54696-106">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="54696-107">Просто укажите учетную запись пользователя для отправки уведомления, и платформа доставит уведомление во все конечные точки устройства.</span><span class="sxs-lookup"><span data-stu-id="54696-107">Simply target a user account to send a notification to, and the platform will deliver the notification to all device endpoints.</span></span> <span data-ttu-id="54696-108">Запросы API уведомлений выполняются от имени пользователя посредством [делегированных разрешений](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) и [разрешения на уведомления]( /graph/permissions_reference), которые можно использовать с учетными записями Майкрософт, рабочими или учебными учетными записями.</span><span class="sxs-lookup"><span data-stu-id="54696-108">Notifications API requests are performed on behalf of a user via [delegated permissions](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) and the [notification permission]( /graph/permissions_reference), which can be used with either Microsoft accounts or work or school accounts.</span></span>
<span data-ttu-id="54696-109">Этот тип уведомления, ориентированного на пользователя, представлен ресурсом [notification](../resources/projectrome-notification.md) и хранится в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="54696-109">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored in Microsoft Graph.</span></span> <span data-ttu-id="54696-110">Доступ к нему и управление можно обеспечить путем публикации приложения с помощью [API SDK Project Rome](https://github.com/Microsoft/project-rome).</span><span class="sxs-lookup"><span data-stu-id="54696-110">It can then be accessed and managed by the publishing app via the [Project Rome SDK APIs](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="next-steps"></a><span data-ttu-id="54696-111">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="54696-111">Next steps</span></span>
- <span data-ttu-id="54696-112">См. статью [Ресурс notification](../resources/projectrome-notification.md) и создавайте уведомления для взаимодействия с пользователями.</span><span class="sxs-lookup"><span data-stu-id="54696-112">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="54696-113">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="54696-113">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
