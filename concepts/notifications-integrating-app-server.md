---
title: Создание и отправка уведомления из службы приложений
description: 'Настройте свою службу приложений для отправки уведомлений, ориентированных на пользователя, в разные клиенты через Microsoft Graph. '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: cf40087aff3956a88f79197482db8126bbe8d96c
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34683512"
---
# <a name="create-and-send-a-notification-from-your-app-service"></a><span data-ttu-id="17bd9-103">Создание и отправка уведомления из службы приложений</span><span class="sxs-lookup"><span data-stu-id="17bd9-103">Create and send a notification from your app service</span></span>

<span data-ttu-id="17bd9-104">Вы можете создавать и отправлять уведомления пользователю с помощью API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="17bd9-104">You can create and send a notification to a user by using Microsoft Graph APIs.</span></span> <span data-ttu-id="17bd9-105">Уведомление хранится в хранилище веб-канала активности и отправляется всем клиентам приложений на всех устройствах, с которых целевой пользователь выполнил вход в систему.</span><span class="sxs-lookup"><span data-stu-id="17bd9-105">The notification is stored in the activity feed store and is sent to all app clients on all devices that the target user is signed in on.</span></span> 

## <a name="authentication"></a><span data-ttu-id="17bd9-106">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="17bd9-106">Authentication</span></span>

<span data-ttu-id="17bd9-107">Служба уведомлений Microsoft Graph требует, чтобы ваша служба приложений использовала поток On-Behalf-Of (OBO) для публикации уведомления для пользователя.</span><span class="sxs-lookup"><span data-stu-id="17bd9-107">Microsoft Graph notifications requires that your application service uses the On-Behalf-Of (OBO) flow to post a notification to a user.</span></span> <span data-ttu-id="17bd9-108">Ниже показан поток проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="17bd9-108">The following is a simple and typical authentication flow:</span></span>

1.  <span data-ttu-id="17bd9-109">Пользователь выполняет вход в приложение с помощью своей учетной записи Майкрософт, рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="17bd9-109">The user signs in to your application with their Microsoft or their work or school account.</span></span> <span data-ttu-id="17bd9-110">При входе служба удостоверений предоставляет вам маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="17bd9-110">When they sign in, the identity service gives you an access token.</span></span>

2.  <span data-ttu-id="17bd9-111">Вы отправляете маркер доступа в свою службу приложений.</span><span class="sxs-lookup"><span data-stu-id="17bd9-111">You send the access token to your app service.</span></span>

3.  <span data-ttu-id="17bd9-112">Ваша служба приложений выполняет проверку подлинности в службе удостоверений и запрашивает маркер OBO для уведомлений Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="17bd9-112">You app service authenticates against the identity service and requests an OBO token for Microsoft Graph notifications.</span></span>

4.  <span data-ttu-id="17bd9-113">Служба удостоверений возвращает маркер на основе OBO и маркер обновления.</span><span class="sxs-lookup"><span data-stu-id="17bd9-113">The identity service returns an OBO-based token and a refresh token.</span></span> <span data-ttu-id="17bd9-114">Ваша служба приложений может использовать этот маркер доступа, чтобы публиковать уведомления для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="17bd9-114">Your app service can use this access token to post notifications to this user.</span></span>

<span data-ttu-id="17bd9-115">Дополнительные сведения о потоке OBO OAuth 2.0 см. в статье [Вызовы между службами с использованием делегированного удостоверения пользователя в потоке On-Behalf-Of](https://docs.microsoft.com/ru-RU/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow).</span><span class="sxs-lookup"><span data-stu-id="17bd9-115">To learn more about OAuth 2.0 OBO flow, see [Service-to-service calls that use delegated user identity in the On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow).</span></span> <span data-ttu-id="17bd9-116">Дополнительные сведения о работе этого потока с уведомлениями Microsoft Graph см. в [примере службы приложений](https://aka.ms/gnsample-appservice).</span><span class="sxs-lookup"><span data-stu-id="17bd9-116">For details about how this flow works with Microsoft Graph notifications, see the [App Service sample](https://aka.ms/gnsample-appservice).</span></span>

> [!NOTE]
> <span data-ttu-id="17bd9-117">В настоящее время уведомления Microsoft Graph используют поток проверки подлинности OBO, но в будущем планируется упростить эту проверку подлинности и устранить необходимость хранения маркеров доступа и маркеров обновления.</span><span class="sxs-lookup"><span data-stu-id="17bd9-117">Microsoft Graph notifications currently uses OBO authentication flow with future plans to simplify this authentication further and eliminate the need to maintain access tokens and refresh tokens.</span></span>

<span data-ttu-id="17bd9-118">Дополнительные сведения о разрешениях API, а также заголовках запросов и откликов см. в статье [Создание и отправка уведомления](/graph/api/notifications-post) справочника по API.</span><span class="sxs-lookup"><span data-stu-id="17bd9-118">For more details on the API permissions and on the request and response headers, please see [Create and send a notification](/graph/api/notifications-post) in the API reference section.</span></span> 
