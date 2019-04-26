---
title: Тип ресурса Notification
description: 'Представляет уведомление, которое публикует сервер приложений, предназначенный для указанного пользователя. Уведомление хранится в Microsoft Graph и распространяется на другие конечные точки устройств, принадлежащие пользователю. '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: af130c9806511b0afbdaedb602790c7c40d3ca2e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563366"
---
# <a name="notification-resource-type"></a><span data-ttu-id="0991f-104">Тип ресурса Notification</span><span class="sxs-lookup"><span data-stu-id="0991f-104">notification resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0991f-105">Представляет уведомление, которое публикует сервер приложений, предназначенный для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="0991f-105">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="0991f-106">Уведомление хранится в Microsoft Graph и распространяется на другие конечные точки устройств, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="0991f-106">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="0991f-107">Уведомление может представлять собой полезные данные визуального уведомления, которые могут интерпретироваться операционной системой, включая платформы Windows, Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="0991f-107">A notification can be a visual notification payload that can be interpreted by the operating system, including Windows, Android, and iOS platforms.</span></span> <span data-ttu-id="0991f-108">Кроме того, это может быть полезная нагрузка данных, которая доставляется и обрабатывается клиентами приложений, что затем определяет соответствующий пользовательский интерфейс на каждом устройстве, обычно — визуальный пользовательский интерфейс уведомления, соответствующий содержимому в создаваемых исходных полезных данных. локально.</span><span class="sxs-lookup"><span data-stu-id="0991f-108">It can also be a data payload that's delivered to and handled by app clients, which then determine the corresponding user experience on each device – usually, a visual notification UI that corresponds to the content in the original data payload that's generated locally.</span></span> 

<span data-ttu-id="0991f-109">Когда пользователь работает с визуальным уведомлением, клиент приложения может использовать пакет SDK для клиентского проекта, чтобы обновить состояние соответствующего канала уведомлений в Microsoft Graph, например, пометив уведомление как закрытое.</span><span class="sxs-lookup"><span data-stu-id="0991f-109">When a user acts on a visual notification, the app client can then use client-side Project Rome SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="0991f-110">После этого обновление будет распространяться во все остальные конечные точки клиентов приложений, а клиенты соответствующим образом обрабатывают изменения, например отправляют уведомление, чтобы запретить пользователю просматривать избыточные данные.</span><span class="sxs-lookup"><span data-stu-id="0991f-110">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="0991f-111">Клиенты приложений могут получить доступ к одному и тому же ресурсу уведомлений позже до истечения срока его действия (даже после того, как он помечается как заблокированный), как журнал уведомлений, с помощью [пакета SDK для Project Рим](https://github.com/Microsoft/project-rome).</span><span class="sxs-lookup"><span data-stu-id="0991f-111">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [Project Rome SDK](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="methods"></a><span data-ttu-id="0991f-112">Методы</span><span class="sxs-lookup"><span data-stu-id="0991f-112">Methods</span></span>
|<span data-ttu-id="0991f-113">Метод</span><span class="sxs-lookup"><span data-stu-id="0991f-113">Method</span></span> | <span data-ttu-id="0991f-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0991f-114">Return Type</span></span> | <span data-ttu-id="0991f-115">Описание</span><span class="sxs-lookup"><span data-stu-id="0991f-115">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="0991f-116">Создание уведомления</span><span class="sxs-lookup"><span data-stu-id="0991f-116">Create notification</span></span>](../api/projectrome-notification-post.md) | [<span data-ttu-id="0991f-117">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="0991f-117">notification</span></span>](projectrome-notification.md) |<span data-ttu-id="0991f-118">Создание и отправка уведомления.</span><span class="sxs-lookup"><span data-stu-id="0991f-118">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="0991f-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="0991f-119">Properties</span></span>
|<span data-ttu-id="0991f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0991f-120">Name</span></span> | <span data-ttu-id="0991f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0991f-121">Type</span></span> | <span data-ttu-id="0991f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0991f-122">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="0991f-123">Таржесостнаме</span><span class="sxs-lookup"><span data-stu-id="0991f-123">targetHostName</span></span> | <span data-ttu-id="0991f-124">String</span><span class="sxs-lookup"><span data-stu-id="0991f-124">String</span></span> | <span data-ttu-id="0991f-125">Представляет имя узла приложения, для которого вызывающая служба хочет отправить уведомление для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="0991f-125">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> |
| <span data-ttu-id="0991f-126">Аппнотификатионид</span><span class="sxs-lookup"><span data-stu-id="0991f-126">appNotificationId</span></span> | <span data-ttu-id="0991f-127">String</span><span class="sxs-lookup"><span data-stu-id="0991f-127">String</span></span> | <span data-ttu-id="0991f-128">Уникальный идентификатор, заданный сервером приложений уведомления, который используется для идентификации и назначения отдельного уведомления.</span><span class="sxs-lookup"><span data-stu-id="0991f-128">The unique id set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="0991f-129">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0991f-129">expirationDateTime</span></span> | <span data-ttu-id="0991f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0991f-130">DateTimeOffset</span></span> | <span data-ttu-id="0991f-131">Задает время истечения срока действия в формате UTC для уведомления пользователя (когда время ожидания) уведомление удаляется из хранилища уведомлений Microsoft Graph полностью и больше не входит в журнал уведомлений.</span><span class="sxs-lookup"><span data-stu-id="0991f-131">Sets a UTC expiration time on a user notification - when time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="0991f-132">Максимальное значение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="0991f-132">Max value is 30 days.</span></span> |
| <span data-ttu-id="0991f-133">payload</span><span class="sxs-lookup"><span data-stu-id="0991f-133">payload</span></span> | <span data-ttu-id="0991f-134">Объект EDM. ComplexType, объект JSON</span><span class="sxs-lookup"><span data-stu-id="0991f-134">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="0991f-135">Это содержимое данных необработанного или визуального пользователя, которое будет доставлено клиенту приложения, получающему это уведомление, и использоваться им.</span><span class="sxs-lookup"><span data-stu-id="0991f-135">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="0991f-136">Полезная нагрузка. Равконтент</span><span class="sxs-lookup"><span data-stu-id="0991f-136">payload.rawContent</span></span> | <span data-ttu-id="0991f-137">String</span><span class="sxs-lookup"><span data-stu-id="0991f-137">String</span></span> | <span data-ttu-id="0991f-138">Содержимое уведомления необработанного пользователя, которое будет доставлено клиенту приложения, получающему это уведомление, и использоваться им.</span><span class="sxs-lookup"><span data-stu-id="0991f-138">The notification content of a raw user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> <span data-ttu-id="0991f-139">По крайней мере один из полезных данных. Равконтент и полезные данные. Висуалконтент должны быть допустимыми для запроса на уведомление POST.</span><span class="sxs-lookup"><span data-stu-id="0991f-139">At least one of Payload.RawContent and Payload.VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="0991f-140">полезные данные. Visual</span><span class="sxs-lookup"><span data-stu-id="0991f-140">payload.visual</span></span> | <span data-ttu-id="0991f-141">Объект EDM. ComplexType, объект JSON</span><span class="sxs-lookup"><span data-stu-id="0991f-141">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="0991f-142">Визуальное содержимое уведомления визуального пользователя, которое будет использоваться платформой уведомлений на каждой платформе для мобильных устройств и визуализировано для пользователей.</span><span class="sxs-lookup"><span data-stu-id="0991f-142">The visual content of a visual user notification, which will be consumed by the notification platform on each mobile platform and rendered for the users.</span></span> <span data-ttu-id="0991f-143">По крайней мере одно из контента и Висуалконтент должно быть допустимым для запроса на уведомление POST.</span><span class="sxs-lookup"><span data-stu-id="0991f-143">At least one of Content and VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="0991f-144">полезные данные. Visual. Title</span><span class="sxs-lookup"><span data-stu-id="0991f-144">payload.visual.title</span></span> | <span data-ttu-id="0991f-145">String</span><span class="sxs-lookup"><span data-stu-id="0991f-145">String</span></span> | <span data-ttu-id="0991f-146">Название визуального уведомления пользователя.</span><span class="sxs-lookup"><span data-stu-id="0991f-146">The title of a visual user notification.</span></span> <span data-ttu-id="0991f-147">Должен иметь либо заголовок, либо основной текст.</span><span class="sxs-lookup"><span data-stu-id="0991f-147">Must have either title or body.</span></span> |
| <span data-ttu-id="0991f-148">полезные данные. Visual. Body</span><span class="sxs-lookup"><span data-stu-id="0991f-148">payload.visual.body</span></span> | <span data-ttu-id="0991f-149">String</span><span class="sxs-lookup"><span data-stu-id="0991f-149">String</span></span> | <span data-ttu-id="0991f-150">Текст уведомления визуального пользователя.</span><span class="sxs-lookup"><span data-stu-id="0991f-150">The body of a visual user notification.</span></span> <span data-ttu-id="0991f-151">Должен иметь либо заголовок, либо основной текст.</span><span class="sxs-lookup"><span data-stu-id="0991f-151">Must have either title or body.</span></span> |
| <span data-ttu-id="0991f-152">Дисплайтиметоливе</span><span class="sxs-lookup"><span data-stu-id="0991f-152">displayTimeToLive</span></span> | <span data-ttu-id="0991f-153">Порог</span><span class="sxs-lookup"><span data-stu-id="0991f-153">Int</span></span> | <span data-ttu-id="0991f-154">Задает время (в секундах), в течение которого содержимое этого уведомления будет оставаться в средстве просмотра уведомлений каждой платформы.</span><span class="sxs-lookup"><span data-stu-id="0991f-154">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="0991f-155">Например, когда уведомление доставляется на устройство Windows, значение этого свойства передается в Тоастнотификатион. Експиратионтиме, которое определяет время, в течение которого всплывающее уведомление остается в центре действий Windows пользователя.</span><span class="sxs-lookup"><span data-stu-id="0991f-155">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="0991f-156">priority</span><span class="sxs-lookup"><span data-stu-id="0991f-156">priority</span></span> | <span data-ttu-id="0991f-157">EnumType</span><span class="sxs-lookup"><span data-stu-id="0991f-157">EnumType</span></span> | <span data-ttu-id="0991f-158">Указывает приоритет уведомления необработанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="0991f-158">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="0991f-159">По умолчанию визуальные уведомления отправляются с высоким приоритетом.</span><span class="sxs-lookup"><span data-stu-id="0991f-159">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="0991f-160">Допустимые значения: высокая и минимальная.</span><span class="sxs-lookup"><span data-stu-id="0991f-160">Valid values are High and Low.</span></span> |
| <span data-ttu-id="0991f-161">groupName</span><span class="sxs-lookup"><span data-stu-id="0991f-161">groupName</span></span> | <span data-ttu-id="0991f-162">String</span><span class="sxs-lookup"><span data-stu-id="0991f-162">String</span></span> | <span data-ttu-id="0991f-163">Имя группы, которой принадлежит это уведомление.</span><span class="sxs-lookup"><span data-stu-id="0991f-163">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="0991f-164">Он задается разработчиком для совместного группирования уведомлений.</span><span class="sxs-lookup"><span data-stu-id="0991f-164">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="0991f-165">Таржетполици</span><span class="sxs-lookup"><span data-stu-id="0991f-165">targetPolicy</span></span> | <span data-ttu-id="0991f-166">Объект EDM. ComplexType, объект JSON</span><span class="sxs-lookup"><span data-stu-id="0991f-166">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="0991f-167">Объект целевой политики обрабатывает политику доставки уведомлений на двух различных типах (Windows, iOS и Android), которые должны быть нацелены, и определенных конечных точках (идентифицируемых идентификаторами подписки), которые должны быть нацелены.</span><span class="sxs-lookup"><span data-stu-id="0991f-167">Target policy object handles notification delivery policy at two different levels - endpoint types (Windows, iOS and Android) that should be targeted, and specific endpoints (identified by subscription ids) that should be targeted.</span></span> |
| <span data-ttu-id="0991f-168">Таржетполици. Платформтипес</span><span class="sxs-lookup"><span data-stu-id="0991f-168">targetPolicy.platformTypes</span></span> | <span data-ttu-id="0991f-169">Модель EDM. ComplexType, Collection (EnumType)</span><span class="sxs-lookup"><span data-stu-id="0991f-169">Edm.ComplexType, Collection (EnumType)</span></span> | <span data-ttu-id="0991f-170">Используется для фильтрации распространения уведомлений на определенную платформу или платформы.</span><span class="sxs-lookup"><span data-stu-id="0991f-170">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="0991f-171">По умолчанию все типы конечных точек Push (iOS, Windows и Android) включены.</span><span class="sxs-lookup"><span data-stu-id="0991f-171">By default, all push endpoint types (iOS, Windows, and Android) are enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0991f-172">Связи</span><span class="sxs-lookup"><span data-stu-id="0991f-172">Relationships</span></span>
<span data-ttu-id="0991f-173">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0991f-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0991f-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0991f-174">JSON representation</span></span>
<span data-ttu-id="0991f-175">Ниже представлено представление ресурса в формате JSON при публикации прямого визуального уведомления, которое доставляется в целевую операционную систему.</span><span class="sxs-lookup"><span data-stu-id="0991f-175">The following is a JSON representation of the resource when you publish a direct visual notification that is delivered to the destination operating system.</span></span>

```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "visualContent": 
    {
      "title": "String",
      "body": "String"
    },
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```

<span data-ttu-id="0991f-176">Ниже представлено представление ресурса в формате JSON при публикации необработанных уведомлений о необработанных данных, доставляемых клиентам приложений.</span><span class="sxs-lookup"><span data-stu-id="0991f-176">The following is a JSON representation of the resource when you publish a raw data notification that is delivered to app clients.</span></span>
```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "rawContent": "String"
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```
