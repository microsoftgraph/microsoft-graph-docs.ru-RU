---
title: Тип ресурса Notification
description: 'Представляет уведомление, которое публикует сервер приложений, предназначенный для указанного пользователя. Уведомление хранится в Microsoft Graph и распространяется на другие конечные точки устройств, принадлежащие пользователю. '
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 97b3d5be5039baff9f73019dbdc54947614d3c1b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078234"
---
# <a name="notification-resource-type"></a><span data-ttu-id="3216e-104">Тип ресурса Notification</span><span class="sxs-lookup"><span data-stu-id="3216e-104">notification resource type</span></span>

<span data-ttu-id="3216e-105">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="3216e-105">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="3216e-106">Представляет уведомление, которое публикует сервер приложений, предназначенный для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3216e-106">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="3216e-107">Уведомление хранится в Microsoft Graph и распространяется на другие конечные точки устройств, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="3216e-107">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="3216e-108">Уведомление может представлять собой полезные данные визуального уведомления, которые могут интерпретироваться операционной системой (платформами Windows, Android и iOS).</span><span class="sxs-lookup"><span data-stu-id="3216e-108">A notification can be a visual notification payload that can be interpreted by the operating system (Windows, Android, and iOS platforms).</span></span> <span data-ttu-id="3216e-109">Это также может быть полезная нагрузка данных (Равконтент), которая доставляется и обрабатывается клиентами приложения (в том числе веб), а затем определяет соответствующие пользовательские взаимодействия на каждом устройстве.</span><span class="sxs-lookup"><span data-stu-id="3216e-109">It can also be a data payload (rawContent) that's delivered to and handled by app clients (including web), which then determine the corresponding user experience on each device.</span></span>  <span data-ttu-id="3216e-110">Обычно это визуальный пользовательский интерфейс уведомления, созданный локально, соответствующий содержимому в исходных полезных данных.</span><span class="sxs-lookup"><span data-stu-id="3216e-110">This is usually a visual notification UI, generated locally, that corresponds to the content in the original data payload.</span></span> 

<span data-ttu-id="3216e-111">Когда пользователь работает с визуальным уведомлением, клиент приложения может использовать пакет SDK клиентских уведомлений для обновления состояния соответствующего канала уведомлений в Microsoft Graph, например, помечая уведомление как закрытое.</span><span class="sxs-lookup"><span data-stu-id="3216e-111">When a user acts on a visual notification, the app client can then use the client-side notifications SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="3216e-112">После этого обновление будет распространяться во все остальные конечные точки клиентов приложений, а клиенты соответствующим образом обрабатывают изменения, например отправляют уведомление, чтобы запретить пользователю просматривать избыточные данные.</span><span class="sxs-lookup"><span data-stu-id="3216e-112">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="3216e-113">Клиенты приложений могут получить доступ к одному и тому же ресурсу уведомлений позже до истечения срока его действия (даже после того, как он помечается как заблокированный), как журнал уведомлений, через [пакет SDK уведомлений](https://aka.ms/GNSDK).</span><span class="sxs-lookup"><span data-stu-id="3216e-113">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [notification SDK](https://aka.ms/GNSDK).</span></span> 

> [!NOTE]
> <span data-ttu-id="3216e-114">Обновления состояния уведомлений, например чтение или закрытие, не будут развертывание которого выполняется для конечных точек веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="3216e-114">Notification state updates, such as read or dismissed, will not be fanned out to web endpoints.</span></span> <span data-ttu-id="3216e-115">Это связано с тем, что принудительная отправка веб-страниц в различных браузерах требует отображения уведомлений визуального уведомления для пользователя.</span><span class="sxs-lookup"><span data-stu-id="3216e-115">This is because web pushes across various browsers require visual toast notifications to be displayed to a user.</span></span> <span data-ttu-id="3216e-116">Так как изменения состояния не имеют соответствующего визуального содержимого, они будут развертывание которого выполняется только для уведомлений, предназначенных для платформ Windows, iOS и Android.</span><span class="sxs-lookup"><span data-stu-id="3216e-116">Because state changes have no corresponding visual content, they will only be fanned-out for notifications targeting Windows, iOS, or Android platforms.</span></span>

## <a name="methods"></a><span data-ttu-id="3216e-117">Методы</span><span class="sxs-lookup"><span data-stu-id="3216e-117">Methods</span></span>
|<span data-ttu-id="3216e-118">Метод</span><span class="sxs-lookup"><span data-stu-id="3216e-118">Method</span></span> | <span data-ttu-id="3216e-119">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3216e-119">Return Type</span></span> | <span data-ttu-id="3216e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3216e-120">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="3216e-121">Создание уведомления</span><span class="sxs-lookup"><span data-stu-id="3216e-121">Create notification</span></span>](../api/user-post-notifications.md) | [<span data-ttu-id="3216e-122">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="3216e-122">notification</span></span>](projectrome-notification.md) |<span data-ttu-id="3216e-123">Создание и отправка уведомления.</span><span class="sxs-lookup"><span data-stu-id="3216e-123">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="3216e-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="3216e-124">Properties</span></span>
|<span data-ttu-id="3216e-125">Имя</span><span class="sxs-lookup"><span data-stu-id="3216e-125">Name</span></span> | <span data-ttu-id="3216e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="3216e-126">Type</span></span> | <span data-ttu-id="3216e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3216e-127">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="3216e-128">таржесостнаме</span><span class="sxs-lookup"><span data-stu-id="3216e-128">targetHostName</span></span> | <span data-ttu-id="3216e-129">String</span><span class="sxs-lookup"><span data-stu-id="3216e-129">String</span></span> | <span data-ttu-id="3216e-130">Представляет имя узла приложения, для которого вызывающая служба хочет отправить уведомление для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3216e-130">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> <span data-ttu-id="3216e-131">Если целевые конечные точки веб-сайта (см **. таржетполици. платформтипес**), убедитесь, что **таржесостнаме** совпадает с именем, используемым при создании подписки на стороне клиента в свойстве JSON приложения.</span><span class="sxs-lookup"><span data-stu-id="3216e-131">If targeting web endpoints (see **targetPolicy.platformTypes**), ensure that **targetHostName** is the same as the name used when creating a subscription on the client side within the application JSON property.</span></span> |
| <span data-ttu-id="3216e-132">аппнотификатионид</span><span class="sxs-lookup"><span data-stu-id="3216e-132">appNotificationId</span></span> | <span data-ttu-id="3216e-133">String</span><span class="sxs-lookup"><span data-stu-id="3216e-133">String</span></span> | <span data-ttu-id="3216e-134">Уникальный идентификатор, заданный сервером приложений уведомления, который используется для идентификации и назначения отдельного уведомления.</span><span class="sxs-lookup"><span data-stu-id="3216e-134">The unique ID set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="3216e-135">groupName</span><span class="sxs-lookup"><span data-stu-id="3216e-135">groupName</span></span> | <span data-ttu-id="3216e-136">String</span><span class="sxs-lookup"><span data-stu-id="3216e-136">String</span></span> | <span data-ttu-id="3216e-137">Имя группы, которой принадлежит это уведомление.</span><span class="sxs-lookup"><span data-stu-id="3216e-137">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="3216e-138">Он задается разработчиком для совместного группирования уведомлений.</span><span class="sxs-lookup"><span data-stu-id="3216e-138">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="3216e-139">таржетполици</span><span class="sxs-lookup"><span data-stu-id="3216e-139">targetPolicy</span></span> | [<span data-ttu-id="3216e-140">таржетполициендпоинтс</span><span class="sxs-lookup"><span data-stu-id="3216e-140">targetPolicyEndpoints</span></span>](targetpolicyendpoints.md) | <span data-ttu-id="3216e-141">Объект целевой политики обрабатывает политику доставки уведомлений для типов конечных точек, которые должны быть нацелены (Windows, iOS, Android и The-Push) для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3216e-141">Target policy object handles notification delivery policy for endpoint types that should be targeted (Windows, iOS, Android and WebPush) for the given user.</span></span> |
| <span data-ttu-id="3216e-142">payload</span><span class="sxs-lookup"><span data-stu-id="3216e-142">payload</span></span> | [<span data-ttu-id="3216e-143">пайлоадтипес</span><span class="sxs-lookup"><span data-stu-id="3216e-143">payloadTypes</span></span>](payloadtypes.md)| <span data-ttu-id="3216e-144">Это содержимое данных необработанного или визуального пользователя, которое будет доставлено клиенту приложения, получающему это уведомление, и использоваться им.</span><span class="sxs-lookup"><span data-stu-id="3216e-144">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="3216e-145">дисплайтиметоливе</span><span class="sxs-lookup"><span data-stu-id="3216e-145">displayTimeToLive</span></span> | <span data-ttu-id="3216e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3216e-146">Int32</span></span> | <span data-ttu-id="3216e-147">Задает время (в секундах), в течение которого содержимое этого уведомления будет оставаться в средстве просмотра уведомлений каждой платформы.</span><span class="sxs-lookup"><span data-stu-id="3216e-147">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="3216e-148">Например, когда уведомление доставляется на устройство Windows, значение этого свойства передается в Тоастнотификатион. Експиратионтиме, которое определяет время, в течение которого всплывающее уведомление остается в центре действий Windows пользователя.</span><span class="sxs-lookup"><span data-stu-id="3216e-148">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="3216e-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3216e-149">expirationDateTime</span></span> | <span data-ttu-id="3216e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3216e-150">DateTimeOffset</span></span> | <span data-ttu-id="3216e-151">Задает дату и время истечения срока действия в формате UTC для уведомления пользователя с помощью формата ISO 8601 (например, полночь UTC на 1 января 2019 выглядит следующим образом: `'2019-01-01T00:00:00Z'` ).</span><span class="sxs-lookup"><span data-stu-id="3216e-151">Sets a UTC expiration date and time on a user notification using ISO 8601 format (for example, midnight UTC on Jan 1, 2019 would look like this: `'2019-01-01T00:00:00Z'`).</span></span> <span data-ttu-id="3216e-152">Когда время отключается, уведомление удаляется из хранилища каналов уведомлений Microsoft Graph полностью и больше не входит в журнал уведомлений.</span><span class="sxs-lookup"><span data-stu-id="3216e-152">When time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="3216e-153">Максимальное значение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="3216e-153">Max value is 30 days.</span></span> |
| <span data-ttu-id="3216e-154">priority</span><span class="sxs-lookup"><span data-stu-id="3216e-154">priority</span></span> | <span data-ttu-id="3216e-155">string</span><span class="sxs-lookup"><span data-stu-id="3216e-155">string</span></span> | <span data-ttu-id="3216e-156">Указывает приоритет уведомления необработанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3216e-156">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="3216e-157">По умолчанию визуальные уведомления отправляются с высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="3216e-157">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="3216e-158">Допустимые значения: `None`, `High` и `Low`.</span><span class="sxs-lookup"><span data-stu-id="3216e-158">Valid values are `None`, `High` and `Low`.</span></span> |
| <span data-ttu-id="3216e-159">фаллбаккполици</span><span class="sxs-lookup"><span data-stu-id="3216e-159">fallbackPolicy</span></span> | [<span data-ttu-id="3216e-160">фаллбаккполици</span><span class="sxs-lookup"><span data-stu-id="3216e-160">fallbackpolicy</span></span>](fallbackpolicy.md) | <span data-ttu-id="3216e-161">Необязательная резервная политика обработки уведомлений объекта политики для конечных точек iOS и предназначена для использования для необработанных уведомлений с высоким приоритетом, которые могут не доставляться на устройства из-за ограничений, определенных платформой (например, режим экономии заряда).</span><span class="sxs-lookup"><span data-stu-id="3216e-161">Optional fallback policy object handles notification fallback policy for iOS endpoints only and is designed to be used for high-priority raw notifications that might not be delivered to devices due to platform specific restrictions (e.g. battery saver mode).</span></span> |


## <a name="relationships"></a><span data-ttu-id="3216e-162">Отношения</span><span class="sxs-lookup"><span data-stu-id="3216e-162">Relationships</span></span>
<span data-ttu-id="3216e-163">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3216e-163">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3216e-164">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3216e-164">JSON representation</span></span>
<span data-ttu-id="3216e-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3216e-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notification",
  "baseType": "",
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


