---
title: Тип ресурса уведомлений
description: 'Представляет уведомления, который был опубликован на сервере приложений, предназначенное для указанного пользователя. Уведомление, сохраненных в Microsoft Graph и распространять на разные устройства конечных точек владеет пользователь. '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: af130c9806511b0afbdaedb602790c7c40d3ca2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509261"
---
# <a name="notification-resource-type"></a><span data-ttu-id="78c73-104">Тип ресурса уведомлений</span><span class="sxs-lookup"><span data-stu-id="78c73-104">notification resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78c73-105">Представляет уведомления, который был опубликован на сервере приложений, предназначенное для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="78c73-105">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="78c73-106">Уведомление, сохраненных в Microsoft Graph и распространять на разные устройства конечных точек владеет пользователь.</span><span class="sxs-lookup"><span data-stu-id="78c73-106">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="78c73-107">Уведомление может быть полезные данные visual уведомлений, позволяя распознавать звук с операционной системы, включая платформы Windows, Android и операций ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="78c73-107">A notification can be a visual notification payload that can be interpreted by the operating system, including Windows, Android, and iOS platforms.</span></span> <span data-ttu-id="78c73-108">Это может быть полезных данных, доставки и обрабатываться клиентами приложения, которые затем определить соответствующий пользователь работать на каждом устройстве — обычно visual уведомлений пользовательского интерфейса, соответствующий контент исходного полезных данных, который создается локально.</span><span class="sxs-lookup"><span data-stu-id="78c73-108">It can also be a data payload that's delivered to and handled by app clients, which then determine the corresponding user experience on each device – usually, a visual notification UI that corresponds to the content in the original data payload that's generated locally.</span></span> 

<span data-ttu-id="78c73-109">Когда пользователь выполняет visual уведомления, клиентского приложения, затем можно использовать пакет SDK для Project рим со стороны клиента для обновления состояния соответствующее уведомление, веб-канала в Microsoft Graph -, например, пометьте уведомление при закрытии.</span><span class="sxs-lookup"><span data-stu-id="78c73-109">When a user acts on a visual notification, the app client can then use client-side Project Rome SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="78c73-110">Обновление затем будет распространяться все другие приложения клиентским конечным точкам и клиентов обрабатывать изменения соответствующим образом, например, отключения уведомлений, чтобы запретить пользователям просматривать сведения о избыточной.</span><span class="sxs-lookup"><span data-stu-id="78c73-110">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="78c73-111">Приложение возможность доступа клиентов к один и тот же ресурс уведомлений в дальнейшем до истечения срока действия (даже после помечена как закрытия), как журнал уведомлений, с помощью пакета [SDK для Project рим](https://github.com/Microsoft/project-rome).</span><span class="sxs-lookup"><span data-stu-id="78c73-111">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [Project Rome SDK](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="methods"></a><span data-ttu-id="78c73-112">Методы</span><span class="sxs-lookup"><span data-stu-id="78c73-112">Methods</span></span>
|<span data-ttu-id="78c73-113">Метод</span><span class="sxs-lookup"><span data-stu-id="78c73-113">Method</span></span> | <span data-ttu-id="78c73-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="78c73-114">Return Type</span></span> | <span data-ttu-id="78c73-115">Описание</span><span class="sxs-lookup"><span data-stu-id="78c73-115">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="78c73-116">Создание уведомлений</span><span class="sxs-lookup"><span data-stu-id="78c73-116">Create notification</span></span>](../api/projectrome-notification-post.md) | <span data-ttu-id="78c73-117">Уведомление</span><span class="sxs-lookup"><span data-stu-id="78c73-117">[notification](projectrome-notification.md)</span></span> |<span data-ttu-id="78c73-118">Создание и отправка уведомления.</span><span class="sxs-lookup"><span data-stu-id="78c73-118">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="78c73-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="78c73-119">Properties</span></span>
|<span data-ttu-id="78c73-120">Имя</span><span class="sxs-lookup"><span data-stu-id="78c73-120">Name</span></span> | <span data-ttu-id="78c73-121">Тип</span><span class="sxs-lookup"><span data-stu-id="78c73-121">Type</span></span> | <span data-ttu-id="78c73-122">Описание</span><span class="sxs-lookup"><span data-stu-id="78c73-122">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="78c73-123">targetHostName</span><span class="sxs-lookup"><span data-stu-id="78c73-123">targetHostName</span></span> | <span data-ttu-id="78c73-124">String</span><span class="sxs-lookup"><span data-stu-id="78c73-124">String</span></span> | <span data-ttu-id="78c73-125">Представляет имя узла приложения, к которому вызова службы, где требуется реализовать для отправки уведомления для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="78c73-125">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> |
| <span data-ttu-id="78c73-126">appNotificationId</span><span class="sxs-lookup"><span data-stu-id="78c73-126">appNotificationId</span></span> | <span data-ttu-id="78c73-127">String</span><span class="sxs-lookup"><span data-stu-id="78c73-127">String</span></span> | <span data-ttu-id="78c73-128">Уникальный идентификатор, установка с сервера приложений уведомлений, используемый для идентификации и предназначенных для отдельных уведомлений.</span><span class="sxs-lookup"><span data-stu-id="78c73-128">The unique id set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="78c73-129">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="78c73-129">expirationDateTime</span></span> | <span data-ttu-id="78c73-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78c73-130">DateTimeOffset</span></span> | <span data-ttu-id="78c73-131">Задает время истечения срока действия UTC уведомления пользователя - при — это время, полностью удаляется из хранилища веб-канала уведомлений Microsoft Graph уведомления и больше не является частью журнал уведомлений.</span><span class="sxs-lookup"><span data-stu-id="78c73-131">Sets a UTC expiration time on a user notification - when time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="78c73-132">Максимальное значение — 30 дней.</span><span class="sxs-lookup"><span data-stu-id="78c73-132">Max value is 30 days.</span></span> |
| <span data-ttu-id="78c73-133">payload</span><span class="sxs-lookup"><span data-stu-id="78c73-133">payload</span></span> | <span data-ttu-id="78c73-134">Edm.ComplexType, объект JSON</span><span class="sxs-lookup"><span data-stu-id="78c73-134">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="78c73-135">Это содержимое данных уведомления необработанные или visual пользователя, который будет доставлено и используемых клиентских приложений, получать это уведомление.</span><span class="sxs-lookup"><span data-stu-id="78c73-135">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="78c73-136">payload.rawContent</span><span class="sxs-lookup"><span data-stu-id="78c73-136">payload.rawContent</span></span> | <span data-ttu-id="78c73-137">String</span><span class="sxs-lookup"><span data-stu-id="78c73-137">String</span></span> | <span data-ttu-id="78c73-138">Содержимое уведомлений уведомление необработанные пользователя, который будет доставлено и используемых клиентских приложений, получать это уведомление.</span><span class="sxs-lookup"><span data-stu-id="78c73-138">The notification content of a raw user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> <span data-ttu-id="78c73-139">По крайней мере один из Payload.RawContent и Payload.VisualContent должен быть допустимый для запрос POST уведомления.</span><span class="sxs-lookup"><span data-stu-id="78c73-139">At least one of Payload.RawContent and Payload.VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="78c73-140">payload.Visual</span><span class="sxs-lookup"><span data-stu-id="78c73-140">payload.visual</span></span> | <span data-ttu-id="78c73-141">Edm.ComplexType, объект JSON</span><span class="sxs-lookup"><span data-stu-id="78c73-141">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="78c73-142">Содержимое visual уведомления visual пользователя, который будет использоваться платформой уведомлений на каждой мобильной платформы и отображаться для пользователей.</span><span class="sxs-lookup"><span data-stu-id="78c73-142">The visual content of a visual user notification, which will be consumed by the notification platform on each mobile platform and rendered for the users.</span></span> <span data-ttu-id="78c73-143">По крайней мере один из контента и VisualContent должен быть допустимый для запрос POST уведомления.</span><span class="sxs-lookup"><span data-stu-id="78c73-143">At least one of Content and VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="78c73-144">payload.Visual.Title</span><span class="sxs-lookup"><span data-stu-id="78c73-144">payload.visual.title</span></span> | <span data-ttu-id="78c73-145">String</span><span class="sxs-lookup"><span data-stu-id="78c73-145">String</span></span> | <span data-ttu-id="78c73-146">Заголовок visual пользовательского уведомления.</span><span class="sxs-lookup"><span data-stu-id="78c73-146">The title of a visual user notification.</span></span> <span data-ttu-id="78c73-147">Необходимо иметь заголовок или текст.</span><span class="sxs-lookup"><span data-stu-id="78c73-147">Must have either title or body.</span></span> |
| <span data-ttu-id="78c73-148">payload.Visual.Body</span><span class="sxs-lookup"><span data-stu-id="78c73-148">payload.visual.body</span></span> | <span data-ttu-id="78c73-149">String</span><span class="sxs-lookup"><span data-stu-id="78c73-149">String</span></span> | <span data-ttu-id="78c73-150">Основная часть visual пользовательского уведомления.</span><span class="sxs-lookup"><span data-stu-id="78c73-150">The body of a visual user notification.</span></span> <span data-ttu-id="78c73-151">Необходимо иметь заголовок или текст.</span><span class="sxs-lookup"><span data-stu-id="78c73-151">Must have either title or body.</span></span> |
| <span data-ttu-id="78c73-152">displayTimeToLive</span><span class="sxs-lookup"><span data-stu-id="78c73-152">displayTimeToLive</span></span> | <span data-ttu-id="78c73-153">Int</span><span class="sxs-lookup"><span data-stu-id="78c73-153">Int</span></span> | <span data-ttu-id="78c73-154">Задает, сколько времени (в секундах) этот контент уведомления будут оставаться в средстве просмотра уведомления для каждой платформы.</span><span class="sxs-lookup"><span data-stu-id="78c73-154">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="78c73-155">Например при доставке уведомления в устройства Windows, значение этого свойства передается ToastNotification.ExpirationTime, который определяет, сколько времени всплывающее уведомление будут оставаться в центр поддержки пользователя Windows.</span><span class="sxs-lookup"><span data-stu-id="78c73-155">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="78c73-156">priority</span><span class="sxs-lookup"><span data-stu-id="78c73-156">priority</span></span> | <span data-ttu-id="78c73-157">EnumType</span><span class="sxs-lookup"><span data-stu-id="78c73-157">EnumType</span></span> | <span data-ttu-id="78c73-158">Указывает приоритет необработанные пользовательского уведомления.</span><span class="sxs-lookup"><span data-stu-id="78c73-158">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="78c73-159">Визуальные уведомления отправляются с наивысший приоритет по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78c73-159">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="78c73-160">Допустимые значения: максимальное и минимальное.</span><span class="sxs-lookup"><span data-stu-id="78c73-160">Valid values are High and Low.</span></span> |
| <span data-ttu-id="78c73-161">GroupName</span><span class="sxs-lookup"><span data-stu-id="78c73-161">groupName</span></span> | <span data-ttu-id="78c73-162">String</span><span class="sxs-lookup"><span data-stu-id="78c73-162">String</span></span> | <span data-ttu-id="78c73-163">Имя группы, к которой принадлежит это уведомление.</span><span class="sxs-lookup"><span data-stu-id="78c73-163">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="78c73-164">Оно установлено разработчика для группирования уведомлений.</span><span class="sxs-lookup"><span data-stu-id="78c73-164">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="78c73-165">targetPolicy</span><span class="sxs-lookup"><span data-stu-id="78c73-165">targetPolicy</span></span> | <span data-ttu-id="78c73-166">Edm.ComplexType, объект JSON</span><span class="sxs-lookup"><span data-stu-id="78c73-166">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="78c73-167">Целевой объект политики обрабатывает политики доставки уведомлений на двух уровнях - типы конечной точки (Windows, iOS и Android), которые должны быть сделаны и конкретных конечных точках (определяются по подписке идентификаторы), которые должны быть сделаны.</span><span class="sxs-lookup"><span data-stu-id="78c73-167">Target policy object handles notification delivery policy at two different levels - endpoint types (Windows, iOS and Android) that should be targeted, and specific endpoints (identified by subscription ids) that should be targeted.</span></span> |
| <span data-ttu-id="78c73-168">targetPolicy.platformTypes</span><span class="sxs-lookup"><span data-stu-id="78c73-168">targetPolicy.platformTypes</span></span> | <span data-ttu-id="78c73-169">Edm.ComplexType коллекции (EnumType)</span><span class="sxs-lookup"><span data-stu-id="78c73-169">Edm.ComplexType, Collection (EnumType)</span></span> | <span data-ttu-id="78c73-170">Используйте для фильтрации рассылки уведомлений для конкретных платформ или платформ.</span><span class="sxs-lookup"><span data-stu-id="78c73-170">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="78c73-171">По умолчанию включены все типы конечных точек push (операций ввода-вывода, Windows и Android).</span><span class="sxs-lookup"><span data-stu-id="78c73-171">By default, all push endpoint types (iOS, Windows, and Android) are enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="78c73-172">Отношения</span><span class="sxs-lookup"><span data-stu-id="78c73-172">Relationships</span></span>
<span data-ttu-id="78c73-173">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="78c73-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78c73-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="78c73-174">JSON representation</span></span>
<span data-ttu-id="78c73-175">Ниже представлена JSON ресурса при публикации прямого visual уведомление, которое доставляется в целевой операционной системы.</span><span class="sxs-lookup"><span data-stu-id="78c73-175">The following is a JSON representation of the resource when you publish a direct visual notification that is delivered to the destination operating system.</span></span>

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

<span data-ttu-id="78c73-176">Ниже представлена JSON ресурса при публикации необработанные данные уведомление, которое доставляется клиентам app.</span><span class="sxs-lookup"><span data-stu-id="78c73-176">The following is a JSON representation of the resource when you publish a raw data notification that is delivered to app clients.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-notification.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
