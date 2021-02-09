---
title: Тип ресурса notification
description: 'Представляет уведомление, опубликованного сервером приложений, которое ориентировано на указанного пользователя. Уведомление хранится в Microsoft Graph и распространяется на разные конечные точки устройств, владельцем которые является пользователь. '
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: abd17119e80e4e8a7967197356811ee519d813ba
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159453"
---
# <a name="notification-resource-type"></a><span data-ttu-id="da47a-104">Тип ресурса notification</span><span class="sxs-lookup"><span data-stu-id="da47a-104">notification resource type</span></span>

<span data-ttu-id="da47a-105">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="da47a-105">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="da47a-106">Представляет уведомление, опубликованного сервером приложений, которое ориентировано на указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="da47a-106">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="da47a-107">Уведомление хранится в Microsoft Graph и распространяется на разные конечные точки устройств, владельцем которые является пользователь.</span><span class="sxs-lookup"><span data-stu-id="da47a-107">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="da47a-108">Уведомление может быть полезной нагрузкой визуального уведомления, которая может интерпретироваться операционной системой (платформы Windows, Android и iOS).</span><span class="sxs-lookup"><span data-stu-id="da47a-108">A notification can be a visual notification payload that can be interpreted by the operating system (Windows, Android, and iOS platforms).</span></span> <span data-ttu-id="da47a-109">Это также может быть полезной нагрузкой данных (rawContent), которая доставляется и обрабатывается клиентами приложений (в том числе через Интернет), которые затем определяют соответствующий пользовательский интерфейс на каждом устройстве.</span><span class="sxs-lookup"><span data-stu-id="da47a-109">It can also be a data payload (rawContent) that's delivered to and handled by app clients (including web), which then determine the corresponding user experience on each device.</span></span>  <span data-ttu-id="da47a-110">Обычно это визуальный пользовательский интерфейс уведомления, созданный локально, соответствующий содержимому в исходных данных.</span><span class="sxs-lookup"><span data-stu-id="da47a-110">This is usually a visual notification UI, generated locally, that corresponds to the content in the original data payload.</span></span> 

<span data-ttu-id="da47a-111">Когда пользователь работает с визуальным уведомлением, клиент приложения может использовать клиентский SDK уведомлений для обновления состояния соответствующего канала уведомлений в Microsoft Graph, например, пометив уведомление как отклоненное.</span><span class="sxs-lookup"><span data-stu-id="da47a-111">When a user acts on a visual notification, the app client can then use the client-side notifications SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="da47a-112">Затем обновление распространяется на все остальные конечные точки клиента приложения, и клиенты обрабатывают изменение соответствующим образом, например, замещение уведомления, чтобы пользователь не видел избыточные сведения.</span><span class="sxs-lookup"><span data-stu-id="da47a-112">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="da47a-113">Клиенты приложений могут получить доступ к одному ресурсу уведомлений позже, прежде чем он истечет (даже после его пометки как отклоненный) в качестве истории уведомлений через [SDK уведомлений.](https://aka.ms/GNSDK)</span><span class="sxs-lookup"><span data-stu-id="da47a-113">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [notification SDK](https://aka.ms/GNSDK).</span></span> 

> [!NOTE]
> <span data-ttu-id="da47a-114">Обновления состояния уведомлений, такие как чтение или отклонение, не будут развещены на веб-конечных точках.</span><span class="sxs-lookup"><span data-stu-id="da47a-114">Notification state updates, such as read or dismissed, will not be fanned out to web endpoints.</span></span> <span data-ttu-id="da47a-115">Это необходимо, поскольку для веб-push-уведомлений в различных браузерах пользователю требуются визуальные всплывающие уведомления.</span><span class="sxs-lookup"><span data-stu-id="da47a-115">This is because web pushes across various browsers require visual toast notifications to be displayed to a user.</span></span> <span data-ttu-id="da47a-116">Поскольку изменения состояния не имеют соответствующего визуального содержимого, они будут развещены только для уведомлений, нацеленных на платформы Windows, iOS или Android.</span><span class="sxs-lookup"><span data-stu-id="da47a-116">Because state changes have no corresponding visual content, they will only be fanned-out for notifications targeting Windows, iOS, or Android platforms.</span></span>

## <a name="methods"></a><span data-ttu-id="da47a-117">Методы</span><span class="sxs-lookup"><span data-stu-id="da47a-117">Methods</span></span>
|<span data-ttu-id="da47a-118">Метод</span><span class="sxs-lookup"><span data-stu-id="da47a-118">Method</span></span> | <span data-ttu-id="da47a-119">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="da47a-119">Return Type</span></span> | <span data-ttu-id="da47a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="da47a-120">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="da47a-121">Создание уведомления</span><span class="sxs-lookup"><span data-stu-id="da47a-121">Create notification</span></span>](../api/user-post-notifications.md) | [<span data-ttu-id="da47a-122">notification</span><span class="sxs-lookup"><span data-stu-id="da47a-122">notification</span></span>](projectrome-notification.md) |<span data-ttu-id="da47a-123">Создание и отправка уведомления.</span><span class="sxs-lookup"><span data-stu-id="da47a-123">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="da47a-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="da47a-124">Properties</span></span>
|<span data-ttu-id="da47a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="da47a-125">Name</span></span> | <span data-ttu-id="da47a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="da47a-126">Type</span></span> | <span data-ttu-id="da47a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="da47a-127">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="da47a-128">targetHostName</span><span class="sxs-lookup"><span data-stu-id="da47a-128">targetHostName</span></span> | <span data-ttu-id="da47a-129">String</span><span class="sxs-lookup"><span data-stu-id="da47a-129">String</span></span> | <span data-ttu-id="da47a-130">Представляет имя хоста приложения, для которого служба звонков хочет опубликовать уведомление для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="da47a-130">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> <span data-ttu-id="da47a-131">При нацеливании на конечные точки веб-сайта (см. **targetPolicy.platformTypes),** убедитесь, что **targetHostName** является тем же именем, которое используется при создании подписки на стороне клиента в свойстве JSON приложения.</span><span class="sxs-lookup"><span data-stu-id="da47a-131">If targeting web endpoints (see **targetPolicy.platformTypes**), ensure that **targetHostName** is the same as the name used when creating a subscription on the client side within the application JSON property.</span></span> |
| <span data-ttu-id="da47a-132">appNotificationId</span><span class="sxs-lookup"><span data-stu-id="da47a-132">appNotificationId</span></span> | <span data-ttu-id="da47a-133">String</span><span class="sxs-lookup"><span data-stu-id="da47a-133">String</span></span> | <span data-ttu-id="da47a-134">Уникальный ИД, установленный сервером приложений уведомления, используемого для идентификации и определения отдельного уведомления.</span><span class="sxs-lookup"><span data-stu-id="da47a-134">The unique ID set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="da47a-135">groupName</span><span class="sxs-lookup"><span data-stu-id="da47a-135">groupName</span></span> | <span data-ttu-id="da47a-136">String</span><span class="sxs-lookup"><span data-stu-id="da47a-136">String</span></span> | <span data-ttu-id="da47a-137">Имя группы, к которой принадлежит это уведомление.</span><span class="sxs-lookup"><span data-stu-id="da47a-137">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="da47a-138">Он устанавливается разработчиком для группировки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="da47a-138">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="da47a-139">targetPolicy</span><span class="sxs-lookup"><span data-stu-id="da47a-139">targetPolicy</span></span> | [<span data-ttu-id="da47a-140">targetPolicyEndpoints</span><span class="sxs-lookup"><span data-stu-id="da47a-140">targetPolicyEndpoints</span></span>](targetpolicyendpoints.md) | <span data-ttu-id="da47a-141">Объект целевой политики обрабатывает политику доставки уведомлений для типов конечных точек, которые должны быть целевыми (Windows, iOS, Android и WebPush) для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="da47a-141">Target policy object handles notification delivery policy for endpoint types that should be targeted (Windows, iOS, Android and WebPush) for the given user.</span></span> |
| <span data-ttu-id="da47a-142">payload</span><span class="sxs-lookup"><span data-stu-id="da47a-142">payload</span></span> | [<span data-ttu-id="da47a-143">payloadTypes</span><span class="sxs-lookup"><span data-stu-id="da47a-143">payloadTypes</span></span>](payloadtypes.md)| <span data-ttu-id="da47a-144">Это содержимое данных необработанных или визуальных уведомлений пользователя, которые будут доставляться и потребляться клиентом приложения, получившего это уведомление.</span><span class="sxs-lookup"><span data-stu-id="da47a-144">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="da47a-145">displayTimeToLive</span><span class="sxs-lookup"><span data-stu-id="da47a-145">displayTimeToLive</span></span> | <span data-ttu-id="da47a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="da47a-146">Int32</span></span> | <span data-ttu-id="da47a-147">Задает время (в секундах) для этого содержимого уведомлений в представлении уведомлений каждой платформы.</span><span class="sxs-lookup"><span data-stu-id="da47a-147">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="da47a-148">Например, когда уведомление доставляется на устройство с Windows, значение этого свойства передается в ToastNotification.ExpirationTime, которое определяет, как долго всплывающее уведомление будет оставаться в центре уведомлений Windows пользователя.</span><span class="sxs-lookup"><span data-stu-id="da47a-148">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="da47a-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="da47a-149">expirationDateTime</span></span> | <span data-ttu-id="da47a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da47a-150">DateTimeOffset</span></span> | <span data-ttu-id="da47a-151">Задает дату и время окончания срока действия в формате UTC для уведомления пользователя в формате ISO 8601 (например, полночь 1 января 2019 г. в формате UTC выглядит так: `'2019-01-01T00:00:00Z'` ).</span><span class="sxs-lookup"><span data-stu-id="da47a-151">Sets a UTC expiration date and time on a user notification using ISO 8601 format (for example, midnight UTC on Jan 1, 2019 would look like this: `'2019-01-01T00:00:00Z'`).</span></span> <span data-ttu-id="da47a-152">После того как время работы, уведомление полностью удаляется из веб-канала уведомлений Microsoft Graph и больше не является частью истории уведомлений.</span><span class="sxs-lookup"><span data-stu-id="da47a-152">When time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="da47a-153">Максимальное значение — 30 дней.</span><span class="sxs-lookup"><span data-stu-id="da47a-153">Max value is 30 days.</span></span> |
| <span data-ttu-id="da47a-154">priority</span><span class="sxs-lookup"><span data-stu-id="da47a-154">priority</span></span> | <span data-ttu-id="da47a-155">string</span><span class="sxs-lookup"><span data-stu-id="da47a-155">string</span></span> | <span data-ttu-id="da47a-156">Указывает приоритет необработанных уведомлений пользователя.</span><span class="sxs-lookup"><span data-stu-id="da47a-156">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="da47a-157">Визуальные уведомления отправляются с высоким приоритетом по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="da47a-157">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="da47a-158">Допустимые значения: `None`, `High` и `Low`.</span><span class="sxs-lookup"><span data-stu-id="da47a-158">Valid values are `None`, `High` and `Low`.</span></span> |
| <span data-ttu-id="da47a-159">fallbackPolicy</span><span class="sxs-lookup"><span data-stu-id="da47a-159">fallbackPolicy</span></span> | [<span data-ttu-id="da47a-160">fallbackpolicy</span><span class="sxs-lookup"><span data-stu-id="da47a-160">fallbackpolicy</span></span>](fallbackpolicy.md) | <span data-ttu-id="da47a-161">Необязательный объект политики отката обрабатывает политику отката уведомлений только для конечных точек iOS и предназначен для использования для необработанных уведомлений с высоким приоритетом, которые могут не доставляться на устройства из-за определенных ограничений платформы (например, режима экономии заряда).</span><span class="sxs-lookup"><span data-stu-id="da47a-161">Optional fallback policy object handles notification fallback policy for iOS endpoints only and is designed to be used for high-priority raw notifications that might not be delivered to devices due to platform specific restrictions (e.g. battery saver mode).</span></span> |


## <a name="relationships"></a><span data-ttu-id="da47a-162">Связи</span><span class="sxs-lookup"><span data-stu-id="da47a-162">Relationships</span></span>
<span data-ttu-id="da47a-163">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="da47a-163">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="da47a-164">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="da47a-164">JSON representation</span></span>
<span data-ttu-id="da47a-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da47a-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notification",
  "keyProperty": "id"
}-->

```json
{
  "targetHostName": "String",
  "appNotificationid": "String (identifier)",
  "groupName": "String", 
  "targetPolicy": {"@odata.type": "microsoft.graph.targetPolicyEndpoints"},
  "payload": {"@odata.type": "microsoft.graph.payloadTypes"},
  "displayTimeToLive": 1024,
  "expirationDateTime": "String (timestamp)",
  "priority": "string",
  "fallbackPolicy": {"@odata.type": "microsoft.graph.fallbackpolicy"},  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


