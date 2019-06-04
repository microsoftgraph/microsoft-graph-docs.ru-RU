---
title: Интеграция приложения iOS с клиентским пакетом SDK для уведомления пользователей
description: Интеграция приложения iOS с клиентским пакетом SDK уведомления пользователей.
localization_priority: Priority
ms.prod: Microsoft Graph notifications
ms.openlocfilehash: 1e0f809e5f6acea272268b76e69e0d86cc18bff0
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063395"
---
# <a name="integrate-your-ios-app-with-the-client-side-sdk-for-user-notifications"></a><span data-ttu-id="65b80-103">Интеграция приложения iOS с клиентским пакетом SDK для уведомления пользователей</span><span class="sxs-lookup"><span data-stu-id="65b80-103">Integrate your iOS app with the client-side SDK for user notifications</span></span>

<span data-ttu-id="65b80-104">После [регистрации приложения](notifications-integration-app-registration.md) на портале Azure и подключения [кроссплатформенных интерфейсов](notifications-integration-cross-device-experiences-onboarding.md) в партнерском центре разработки следующий этап состоит в интеграции вашего клиентского приложения с клиентским пакетом SDK для приложений iOS.</span><span class="sxs-lookup"><span data-stu-id="65b80-104">After you [register your app](notifications-integration-app-registration.md) in the Azure Portal and onboard your [cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md) in the Partner Dev Center, the next step is to integrate your client app with the client-side SDK foriOS apps.</span></span>  

<span data-ttu-id="65b80-105">С помощью клиентского пакета SDK ваше приложение может выполнять необходимые действия регистрации, чтобы начать получение уведомлений, опубликованных вашим сервером приложений и предназначенных для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="65b80-105">With the client-side SDK, your app can perform the necessary registration steps to start receiving notifications published from your app server targeted at the user who is currently signed in.</span></span> <span data-ttu-id="65b80-106">После этого пакет SDK управляет уведомлениями на стороне клиента, включая получение новых входящих уведомлений и управление состоянием уведомлений для осуществления таких сценариев, как универсальное закрытие и получение полного журнала уведомлений.</span><span class="sxs-lookup"><span data-stu-id="65b80-106">The SDK then manages the notifications on the client side, including receiving new incoming notifications, managing the state of notifications to achieve scenarios like universal dismiss, and retrieving full notification history.</span></span> 

## <a name="new-incoming-notification-flow"></a><span data-ttu-id="65b80-107">Поток новых входящих уведомлений</span><span class="sxs-lookup"><span data-stu-id="65b80-107">New incoming notification flow</span></span>

<span data-ttu-id="65b80-108">Поток данных для получения новых входящих уведомлений показан на схеме ниже.</span><span class="sxs-lookup"><span data-stu-id="65b80-108">For receiving new incoming notifications, the data flow is shown in the following diagram.</span></span>

![Поток данных новых уведомлений для приложения iOS](images/notifications-new-notification-ios.png)

<span data-ttu-id="65b80-110">Этот процесс включает несколько компонентов:</span><span class="sxs-lookup"><span data-stu-id="65b80-110">The process involves a few components:</span></span>

* <span data-ttu-id="65b80-111">Сервер приложений — серверный компонент вашего приложения</span><span class="sxs-lookup"><span data-stu-id="65b80-111">App server - The back end of your application</span></span>
* <span data-ttu-id="65b80-112">Клиент приложения — внешний интерфейс вашего приложения (приложение UWP, приложение Android или приложение iOS)</span><span class="sxs-lookup"><span data-stu-id="65b80-112">App client - The front end of your application (a UWP app, an Android app, or an iOS app)</span></span>
* <span data-ttu-id="65b80-113">Уведомления Microsoft Graph — компонент службы, позволяющий публиковать, хранить и синхронизировать уведомления пользователей на разных экземплярах клиентов приложения для разных устройств и платформ</span><span class="sxs-lookup"><span data-stu-id="65b80-113">Microsoft Graph notifications - The service component that enables user notifications to be published, stored, and synced across different instances of app clients across devices and platforms</span></span>
* <span data-ttu-id="65b80-114">APNs — служба push-уведомлений Apple Push Notification Service, предоставленная корпорацией Apple для приложений iOS.</span><span class="sxs-lookup"><span data-stu-id="65b80-114">APNs - The Apple Push Notification Service provided by Apple for iOS apps.</span></span> <span data-ttu-id="65b80-115">Уведомления Microsoft Graph используют эти службы для сообщения клиентам приложений iOS об изменениях данных уведомления пользователя.</span><span class="sxs-lookup"><span data-stu-id="65b80-115">Microsoft Graph notifications use this service to signal the iOS app clients about user notification data changes.</span></span>  

<span data-ttu-id="65b80-116">На схеме показаны следующие шаги:</span><span class="sxs-lookup"><span data-stu-id="65b80-116">The accompanying diagram shows the following scenario:</span></span> 

1. <span data-ttu-id="65b80-117">Логика приложения.</span><span class="sxs-lookup"><span data-stu-id="65b80-117">Application logic.</span></span> <span data-ttu-id="65b80-118">Этот шаг фиксирует событие, запускающее публикацию уведомления для пользователя.</span><span class="sxs-lookup"><span data-stu-id="65b80-118">This step captures what triggers the notification to be published to the user.</span></span> <span data-ttu-id="65b80-119">Эта логика зависит от приложения и может относиться к обновлению события или данных других элементов в Microsoft Graph, например новому событию календаря, назначению задачи или другому действию, о котором ваша служба приложений хочет уведомить пользователя.</span><span class="sxs-lookup"><span data-stu-id="65b80-119">This is app-specific logic, and can be an event or data update about something else in Microsoft Graph, such as a new calendar event or task assignment, or else your app service wants to notify the user about.</span></span>
2. <span data-ttu-id="65b80-120">Сервер приложений публикует уведомление для целевого пользователя с помощью API уведомлений Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="65b80-120">The app server publishes a notification to the targeted user via the Microsoft Graph notifications API.</span></span> <span data-ttu-id="65b80-121">Дополнительные сведения см. в статье [Серверная интеграция](notifications-integrating-app-server.md).</span><span class="sxs-lookup"><span data-stu-id="65b80-121">For more details, see [server side integration](notifications-integrating-app-server.md).</span></span>
3. <span data-ttu-id="65b80-122">После получения веб-запроса, содержащего новое уведомление, служба уведомлений Microsoft Graph безопасно сохраняет контент уведомления в облаке для этого приложения и этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="65b80-122">On receiving the web request containing the new notification, Microsoft Graph notifications persists the content of the notification securely in the cloud for this app and this user.</span></span>
4. <span data-ttu-id="65b80-123">Для каждого экземпляра клиента приложения, подписывающегося на получение уведомлений для этого пользователя, служба уведомлений Microsoft Graph отправляет сигнал для уведомления клиента приложения посредством собственной службы push-уведомлений, предоставляемой операционной системой.</span><span class="sxs-lookup"><span data-stu-id="65b80-123">For each app client instance subscribing to receive notifications for this user, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="65b80-124">В этом случае мы имеем дело с приложением iOS, в нем для отправки сигнала используется [фоновое уведомление APNs об обновлении].</span><span class="sxs-lookup"><span data-stu-id="65b80-124">In this case, the application is an iOS app, and it uses [APNs background update notification] to send the signal.</span></span> 
5. <span data-ttu-id="65b80-125">После того, как приложение получит сигнал с помощью входящего push-уведомления, оно обращается к пакету SDK за получением изменений в хранилище уведомлений пользователя.</span><span class="sxs-lookup"><span data-stu-id="65b80-125">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
6. <span data-ttu-id="65b80-126">SDK создает безопасное и соответствующее соединение с хранилищем уведомлений пользователя в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="65b80-126">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
7. <span data-ttu-id="65b80-127">SDK получает изменения данных, то есть, в этом случае, — новый контент уведомления.</span><span class="sxs-lookup"><span data-stu-id="65b80-127">The SDK gets the data changes - in this case, the new notification contents.</span></span> 
8. <span data-ttu-id="65b80-128">SDK выполняет обратные вызовы события срабатывает обратные вызовы события, чтобы уведомить приложение после успешного получения изменений.</span><span class="sxs-lookup"><span data-stu-id="65b80-128">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
9. <span data-ttu-id="65b80-129">Логика приложения.</span><span class="sxs-lookup"><span data-stu-id="65b80-129">Application logic.</span></span> <span data-ttu-id="65b80-130">Этот шаг фиксирует выбор приложения внутри обратного вызова события.</span><span class="sxs-lookup"><span data-stu-id="65b80-130">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="65b80-131">Обычно это приводит к локальным изменениям данных приложения и локальным обновлениям пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="65b80-131">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="65b80-132">В этом случае приложение обычно создает оповещение iOS, чтобы уведомить пользователя о содержимом уведомления.</span><span class="sxs-lookup"><span data-stu-id="65b80-132">In this case,  the app usually constructs an iOS alert to notify the user about the notification contents.</span></span>

## <a name="notification-update-flow"></a><span data-ttu-id="65b80-133">Поток обновления уведомлений</span><span class="sxs-lookup"><span data-stu-id="65b80-133">Notification update flow</span></span>

<span data-ttu-id="65b80-134">Одно из основных преимуществ использования уведомлений Microsoft Graph заключается в безопасном сохранении уведомлений в облаке и преобразование их в тип ресурса с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="65b80-134">One of the main benefits for using Microsoft Graph notifications is that it persists notifications in the cloud securely and turns them into a stateful resource type.</span></span> <span data-ttu-id="65b80-135">Это может помочь вашему приложению управлять правильным состоянием уведомлений и синхронизировать его на разных устройствах для того же вошедшего пользователя в сценарии с несколькими устройствами.</span><span class="sxs-lookup"><span data-stu-id="65b80-135">Therefore, it can help your application to manage and sync the correct state of the notifications across different devices for the same signed in user in a cross-device scenario.</span></span> <span data-ttu-id="65b80-136">Если уведомление помечено как закрытое или прочитанное на одном устройстве, другие устройства могут уведомляться в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="65b80-136">When a notification is marked as dismissed, or marked as read on one device, the other devices can be notified in real-time.</span></span> <span data-ttu-id="65b80-137">"Обработано однажды, закрыто везде" может стать истинным обещанием в рамках интерфейса уведомлений для ваших пользователей.</span><span class="sxs-lookup"><span data-stu-id="65b80-137">"Handled once, dismissed everywhere" can become a true promise as part of the notification experience for your users.</span></span> 

<span data-ttu-id="65b80-138">На схеме ниже показан поток данных для изменения состояния уведомления или удаления уведомления на одном устройстве и получения/обработки изменения состояния или удаления на другом устройстве.</span><span class="sxs-lookup"><span data-stu-id="65b80-138">The following diagram shows the data flow for changing the state of a notification or deleting the notification on one device, and receiving/handling the state change or the deletion on another device.</span></span>

![Поток данных обновления уведомлений для приложения iOS](images/notifications-notification-update-ios.png)

<span data-ttu-id="65b80-140">Обратите внимание, что вторая часть потока похожа на поток для обработки новых входящих уведомлений.</span><span class="sxs-lookup"><span data-stu-id="65b80-140">Notice that the second part of the flow is similar to the flow for handling new incoming notifications.</span></span> <span data-ttu-id="65b80-141">Это сделано намеренно. Шаблон программирования пакета SDK создан таким образом, чтобы клиент приложения мог обрабатывать все типы изменений данных уведомлений пользователей (новые входящие уведомления, изменения состояния уведомления, удаление уведомления) аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="65b80-141">This is by design - the  programming pattern of the SDK is designed so that the application client can handle all types of user notification data changes (new incoming notifications, notification state changes, notification deleted) in a similar way.</span></span>  

<span data-ttu-id="65b80-142">На схеме показаны следующие шаги:</span><span class="sxs-lookup"><span data-stu-id="65b80-142">The accompanying diagram shows the following scenario:</span></span>

1. <span data-ttu-id="65b80-143">Логика приложения.</span><span class="sxs-lookup"><span data-stu-id="65b80-143">Application logic.</span></span> <span data-ttu-id="65b80-144">Некоторое событие запускает изменение или удаление уведомления.</span><span class="sxs-lookup"><span data-stu-id="65b80-144">Something triggers the notification to be changed or deleted.</span></span> <span data-ttu-id="65b80-145">В принципе, любое событие может запустить изменение уведомления.</span><span class="sxs-lookup"><span data-stu-id="65b80-145">In general, any event can trigger a notification to change.</span></span> 
2. <span data-ttu-id="65b80-146">Приложение вызывает SDK клиента, чтобы обновить или удалить уведомление.</span><span class="sxs-lookup"><span data-stu-id="65b80-146">App calling into the client SDK to update or delete a notification.</span></span> <span data-ttu-id="65b80-147">В настоящее время представлено два свойства, связанных с изменением состояния: **userActionState** и **readState**, но ваше приложение может определять эти состояния и необходимость их обновления.</span><span class="sxs-lookup"><span data-stu-id="65b80-147">Currently, we expose two properties regarding state changes - **userActionState** and **readState** - but your application can define these states and when they need to be updated.</span></span> <span data-ttu-id="65b80-148">Например, если пользователь закрывает всплывающее уведомление, вы можете обновить свойство **userActionState**, присвоив ему значение Dismissed.</span><span class="sxs-lookup"><span data-stu-id="65b80-148">For example, when a user dismisses the notification popup, you can update the **userActionState** to be Dismissed.</span></span> <span data-ttu-id="65b80-149">Когда пользователь щелкает всплывающее уведомление и запускает приложение для использования соответствующего контента приложения, вы можете обновить свойство **userActionState**, присвоив ему значение Activated, и обновить свойство **readState**, присвоив ему значение Read.</span><span class="sxs-lookup"><span data-stu-id="65b80-149">When a user clicks the notification popup and launches the app to consume corresponding app content, you can update the **userActionState** to be Activated and update the **readState** to be Read.</span></span> 
3. <span data-ttu-id="65b80-150">После вызова соответствующего API для обновления или удаления уведомления пакет SDK вызовет хранилище уведомлений пользователя в облаке, чтобы развернуть это изменение для других экземпляров клиента приложения с этим вошедшим пользователем.</span><span class="sxs-lookup"><span data-stu-id="65b80-150">After the corresponding API is called to update or delete a notification, the SDK will call into the user notification store in the cloud in order to fan-out this change to the other app client instances with the same signed in user.</span></span> 
4. <span data-ttu-id="65b80-151">После получения от клиента запроса на обновление или удаление служба уведомлений Microsoft Graph обновит хранилище уведомлений и определит другие экземпляры клиентов приложения, подписанные на это изменение.</span><span class="sxs-lookup"><span data-stu-id="65b80-151">On receiving the update/delete request from a client, Microsoft Graph notifications will update the notification store, and identify the other app client instances that subscribed to this change.</span></span>
5. <span data-ttu-id="65b80-152">Для каждой подписки экземпляра клиента приложения служба уведомлений Microsoft Graph отправляет сигнал для уведомления клиента приложения посредством собственной службы push-уведомлений, предоставляемой операционной системой.</span><span class="sxs-lookup"><span data-stu-id="65b80-152">For each app client subscription, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="65b80-153">В этом случае мы имеем дело с iOS, где для отправки сигнала используется [фоновое уведомление APNs об обновлении](https://developer.apple.com/library/archive/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/CreatingtheNotificationPayload.html#//apple_ref/doc/uid/TP40008194-CH10-SW8).</span><span class="sxs-lookup"><span data-stu-id="65b80-153">In this case, this is an iOS, and it uses [APNs background update notification](https://developer.apple.com/library/archive/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/CreatingtheNotificationPayload.html#//apple_ref/doc/uid/TP40008194-CH10-SW8) to send the signal.</span></span> 
6. <span data-ttu-id="65b80-154">После того, как приложение получит сигнал с помощью входящего push-уведомления, оно обращается к пакету SDK за получением изменений в хранилище уведомлений пользователя.</span><span class="sxs-lookup"><span data-stu-id="65b80-154">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
7. <span data-ttu-id="65b80-155">SDK создает безопасное и соответствующее соединение с хранилищем уведомлений пользователя в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="65b80-155">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
8. <span data-ttu-id="65b80-156">SDK получает изменения данных: в этом случае изменениями являются обновления состояния уведомления или удаления уведомления.</span><span class="sxs-lookup"><span data-stu-id="65b80-156">The SDK gets the data changes - in this case, the changes are notification state updates or notification deletions.</span></span> 
9. <span data-ttu-id="65b80-157">SDK выполняет обратные вызовы события срабатывает обратные вызовы события, чтобы уведомить приложение после успешного получения изменений.</span><span class="sxs-lookup"><span data-stu-id="65b80-157">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
10. <span data-ttu-id="65b80-158">Логика приложения.</span><span class="sxs-lookup"><span data-stu-id="65b80-158">Application logic.</span></span> <span data-ttu-id="65b80-159">Этот шаг фиксирует выбор приложения внутри обратного вызова события.</span><span class="sxs-lookup"><span data-stu-id="65b80-159">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="65b80-160">Обычно это приводит к локальным изменениям данных приложения и локальным обновлениям пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="65b80-160">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="65b80-161">В этом случае приложение должно локально обновить пользовательский интерфейс, чтобы отобразить изменение состояния, так как имеются обновления уведомлений.</span><span class="sxs-lookup"><span data-stu-id="65b80-161">In this case, because there are notification updates, the app should update the UI locally to reflect the state change.</span></span> <span data-ttu-id="65b80-162">Например, если уведомление помечено как активированное, вы можете удалить соответствующее сообщение в центре уведомлений iOS, чтобы достичь результата "обработано однажды, закрыто везде".</span><span class="sxs-lookup"><span data-stu-id="65b80-162">For example, if a notification is marked as activated, you can remove the corresponding alert UI inside the iOS notification center to achieve "handled once, dismissed everywhere".</span></span> 

<span data-ttu-id="65b80-163">Дополнительные сведения об уведомлениях Microsoft Graph см. в статье [Общие сведения об уведомлениях Microsoft Graph](notifications-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="65b80-163">For more information about Microsoft Graph notifications, see [Microsoft Graph Notifications overview](notifications-concept-overview.md).</span></span> <span data-ttu-id="65b80-164">Дополнительные сведения о всех действиях, требующихся для интеграции с уведомлениями Microsoft Graph см. в [обзоре интеграции](notifications-integration-e2e-overview.md) уведомлений Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="65b80-164">For more information about the steps required to integrate with Microsoft Graph notifications from end to end, see Microsoft Graph notifications [integration overview](notifications-integration-e2e-overview.md).</span></span>

## <a name="adding-the-sdk-to-your-project"></a><span data-ttu-id="65b80-165">Добавление SDK в проект</span><span class="sxs-lookup"><span data-stu-id="65b80-165">Adding the OfficeThemes.css file to your project</span></span>

<span data-ttu-id="65b80-166">Самый простой способ добавить платформу подключенных устройств в приложение iOS — воспользоваться диспетчером зависимостей [CocoaPods](https://cocoapods.org/).</span><span class="sxs-lookup"><span data-stu-id="65b80-166">The simplest way to add the Connected Devices Platform to your iOS app is by using the [CocoaPods](https://cocoapods.org/) dependency manager.</span></span> <span data-ttu-id="65b80-167">Перейдите в раздел *Podfile* проекта для iOS и вставьте следующую запись:</span><span class="sxs-lookup"><span data-stu-id="65b80-167">Go to your iOS project's *Podfile* and insert the following entry:</span></span>

```ObjectiveC
platform :ios, "10.0"
workspace 'iOSSample'

target 'iOSSample' do
  # Uncomment the next line if you're using Swift or would like to use dynamic frameworks
  # use_frameworks!

    pod 'ProjectRomeSdk'

  # Pods for iOSSample
```

> [!NOTE]
> <span data-ttu-id="65b80-168">Для использования CocoaPod необходимо использовать в проекте файл _.xcworkspace_.</span><span class="sxs-lookup"><span data-stu-id="65b80-168">In order to consume CocoaPod, you must use the _.xcworkspace_ file in your project.</span></span>

## <a name="initializing-the-connected-device-platforms"></a><span data-ttu-id="65b80-169">Инициализация платформы подключенных устройств</span><span class="sxs-lookup"><span data-stu-id="65b80-169">Initializing the Connected Device Platforms</span></span>

<span data-ttu-id="65b80-170">Клиентский SDK создан на основе инфраструктуры, называемой платформой подключенных устройств.</span><span class="sxs-lookup"><span data-stu-id="65b80-170">The client-side SDK is built on top of an infrastructure called Connected Device Platform.</span></span> <span data-ttu-id="65b80-171">Перед использованием каких-либо функций необходимо инициализировать платформу в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="65b80-171">Before any feature can be used, the platform must be initialized within your app.</span></span> <span data-ttu-id="65b80-172">Действия по инициализации должны находиться в методе **AppDelegate**, поскольку они должны быть выполнены до использования сценариев уведомлений.</span><span class="sxs-lookup"><span data-stu-id="65b80-172">The initialization steps should occur in your **AppDelegate** method, because they are required before the notification scenarios can take place.</span></span>

<span data-ttu-id="65b80-173">Необходимо создать и инициализировать платформу путем создания экземпляра класса [**MCDConnectedDevicesPlatform**](https://docs.microsoft.com/ru-RU/windows/project-rome/objectivec-api/connecteddevices/mcdconnecteddevicesplatform).</span><span class="sxs-lookup"><span data-stu-id="65b80-173">You must construct and initialize the platform by instantiating the [**MCDConnectedDevicesPlatform**](https://docs.microsoft.com/en-us/windows/project-rome/objectivec-api/connecteddevices/mcdconnecteddevicesplatform) class.</span></span> <span data-ttu-id="65b80-174">Перед этим подключите обработчики событий, как показано здесь, поскольку после запуска платформы могут начать возникать события.</span><span class="sxs-lookup"><span data-stu-id="65b80-174">efore doing that, make sure to hook up event handlers, as shown, because after platform is started, the events might begin to fire.</span></span>  

```ObjectiveC
MCDConnectedDevicesPlatform* platform = [MCDConnectedDevicesPlatform new];
        
[platform.accountManager.accessTokenRequested subscribe:^(MCDConnectedDevicesAccountManager* _Nonnull manager, MCDConnectedDevicesAccessTokenRequestedEventArgs* _Nonnull args) {
    // implement the callback;
}];
        
[self.platform.accountManager.accessTokenInvalidated
    subscribe:^(MCDConnectedDevicesAccountManager* _Nonnull manager __unused,
        MCDConnectedDevicesAccessTokenInvalidatedEventArgs* _Nonnull request) {
    // implement the callback;
}];
        
[self.platform.notificationRegistrationManager.notificationRegistrationStateChanged subscribe:^(MCDConnectedDevicesNotificationRegistrationManager* _Nonnull manager __unused, MCDConnectedDevicesNotificationRegistrationStateChangedEventArgs* _Nonnull args) {
    // implement the callback
}];
        
[platform start];
```

### <a name="handling-account-access-token"></a><span data-ttu-id="65b80-175">Обработка маркера доступа учетной записи</span><span class="sxs-lookup"><span data-stu-id="65b80-175">Handling account access token</span></span>

<span data-ttu-id="65b80-176">Все веб-вызовы, выполняемые SDK, включая получение контента нового входящего уведомления, обновление состояний уведомлений и т. д., считываются из данных пользователя или записываются в них, поэтому всегда требуется действующий маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="65b80-176">All the web calls the SDK makes, including retrieving the content of a new incoming notification, updating notification states, and more, are reading from or writing to the user's data, and therefore always require a valid access token.</span></span> <span data-ttu-id="65b80-177">При использовании SDK требуется, чтобы вы обеспечили обработку следующих событий, вызываемых, когда маркер доступа запрашивается или становится недействительным. Это необходимо, чтобы правильно обрабатывать маркер доступа пользователя после инициализации платформы.</span><span class="sxs-lookup"><span data-stu-id="65b80-177">The SDK requires you to handle the following events - invoked when an access token is requested or invalidated - to make sure that after the platform is initialized, your access token for the user is handled correctly.</span></span> 

#### <a name="accesstokenrequested"></a><span data-ttu-id="65b80-178">accessTokenRequested</span><span class="sxs-lookup"><span data-stu-id="65b80-178">accessTokenRequested</span></span>

<span data-ttu-id="65b80-179">Полную реализацию см. в [примере приложения iOS](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m).</span><span class="sxs-lookup"><span data-stu-id="65b80-179">For a full implementation, see the [iOS sample app](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m).</span></span> 

#### <a name="accesstokeninvalidated"></a><span data-ttu-id="65b80-180">accessTokenInvalidated</span><span class="sxs-lookup"><span data-stu-id="65b80-180">accessTokenInvalidated</span></span>

<span data-ttu-id="65b80-181">Полную реализацию см. в [примере приложения iOS](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m).</span><span class="sxs-lookup"><span data-stu-id="65b80-181">For a full implementation, see the [iOS sample app](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m).</span></span> 

```ObjectiveC
[platform.accountManager.accessTokenInvalidated
    subscribe:^(MCDConnectedDevicesAccountManager* _Nonnull manager __unused,
        MCDConnectedDevicesAccessTokenInvalidatedEventArgs* _Nonnull request) {
}];
```

### <a name="handling-push-registration-expiration"></a><span data-ttu-id="65b80-182">Обработка истечения срока регистрации для push-уведомлений</span><span class="sxs-lookup"><span data-stu-id="65b80-182">Handling push registration expiration</span></span> 

<span data-ttu-id="65b80-183">Уведомления Microsoft Graph используют APNs (собственная платформа push-уведомлений в iOS) для отправки клиентскому приложению сигнала об изменениях данных в уведомлениях пользователя.</span><span class="sxs-lookup"><span data-stu-id="65b80-183">Microsoft Graph notifications use APNs, the native push platform on iOS, to signal the client application on user notifications data changes.</span></span> <span data-ttu-id="65b80-184">Это происходит, когда новые входящие уведомления публикуются с вашего сервера приложений или когда обновляется состояние любого уведомления на другом устройстве с тем же вошедшим пользователем в сценарии с разными устройствами.</span><span class="sxs-lookup"><span data-stu-id="65b80-184">This happens when new incoming notifications are published from your app server, or when any notification's state is updated on a different device with the same signed in user in a cross-device scenario.</span></span> 

<span data-ttu-id="65b80-185">Поэтому требуется действующий маркер APNs, обеспечивающий передачу фоновых уведомлений об обновлениях.</span><span class="sxs-lookup"><span data-stu-id="65b80-185">For this reason, a valid APNs token that allows background update notifications to come through successfully is required.</span></span> <span data-ttu-id="65b80-186">Следующий обратный вызов события обрабатывает истечение срока действия маркеров push-уведомлений APNs.</span><span class="sxs-lookup"><span data-stu-id="65b80-186">The following event callback handles APNs push token expirations.</span></span> 

#### <a name="notificationregistrationstatechanged"></a><span data-ttu-id="65b80-187">notificationRegistrationStateChanged</span><span class="sxs-lookup"><span data-stu-id="65b80-187">notificationRegistrationStateChanged</span></span>

<span data-ttu-id="65b80-188">Полную реализацию см. в [примере приложения iOS](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m).</span><span class="sxs-lookup"><span data-stu-id="65b80-188">For a full implementation, see the [iOS sample app](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m).</span></span> 

## <a name="signing-in-your-user"></a><span data-ttu-id="65b80-189">Вход пользователя в систему</span><span class="sxs-lookup"><span data-stu-id="65b80-189">Signing in your user</span></span>

<span data-ttu-id="65b80-190">Уведомления в Microsoft Graph, как и многие другие типы ресурсов в Microsoft Graph, работают на основе доступа пользователей в систему.</span><span class="sxs-lookup"><span data-stu-id="65b80-190">Microsoft Graph notifications, like many other resource types inside Microsoft Graph, are centralized around users.</span></span> <span data-ttu-id="65b80-191">Чтобы приложение могло подписаться на уведомления и могло начать получать уведомления для пользователя, вошедшего в систему, сначала необходимо получить действующий маркер OAuth для использования в процессе регистрации.</span><span class="sxs-lookup"><span data-stu-id="65b80-191">In order for your app to subscribe to and start receiving notifications for the signed in user, you first need to obtain a valid OAuth token to be used in the registration process.</span></span> <span data-ttu-id="65b80-192">Вы можете использовать любой удобный способ формирования маркеров OAuth и управления ими.</span><span class="sxs-lookup"><span data-stu-id="65b80-192">You can use your preferred method of generating and managing the OAuth tokens.</span></span> <span data-ttu-id="65b80-193">В примере приложения используется ADAL.</span><span class="sxs-lookup"><span data-stu-id="65b80-193">The sample app uses ADAL.</span></span> 

<span data-ttu-id="65b80-194">Если вы используете учетную запись Майкрософт, необходимо включить следующие разрешения в запрос входа: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry` и `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span><span class="sxs-lookup"><span data-stu-id="65b80-194">If you're using a Microsoft account, you will need to include the following permissions in your sign-in request: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, and `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span></span> 

<span data-ttu-id="65b80-195">Если вы используете учетную запись Azure AD, необходимо запросить следующую аудиторию: `https://cdpcs.access.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="65b80-195">If you're using an Azure AD account, you'll need to request the following audience: `https://cdpcs.access.microsoft.com`.</span></span>

## <a name="adding-the-user-account-to-the-platform"></a><span data-ttu-id="65b80-196">Добавление учетной записи пользователя на платформу</span><span class="sxs-lookup"><span data-stu-id="65b80-196">Adding the user account to the platform</span></span> 

<span data-ttu-id="65b80-197">Необходимо зарегистрировать в SDK учетную запись вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="65b80-197">You need to register the signed in user account with the SDK.</span></span> <span data-ttu-id="65b80-198">Для этого необходимо добавить учетную запись и зарегистрировать push-канал, чтобы получать начальные push-уведомления через службу APNs.</span><span class="sxs-lookup"><span data-stu-id="65b80-198">This involves adding the account and registering a push channel to receive the initial push notifications through APNs.</span></span> <span data-ttu-id="65b80-199">Дополнительные сведения см. в методе [prepareAccountAsync](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m) в примере.</span><span class="sxs-lookup"><span data-stu-id="65b80-199">For details, see the [prepareAccountAsync](https://github.com/Microsoft/project-rome/blob/master/iOS/samples/GraphNotifications/GraphNotificationsSample/ConnectedDevicesPlatformManager.m) method in the sample.</span></span>

```ObjectiveC
MCDConnectedDevicesPlatform* platform = [MCDConnectedDevicesPlatform new];
MCDConnectedDevicesAccount* mcdAccount = [MCDConnectedDevicesAccount new];

[platform.accountManager addAccountAsync:mcdAccount callback:adapter]; 
```

## <a name="subscribing-to-receive-users-notifications"></a><span data-ttu-id="65b80-200">Подписка для получения уведомлений пользователей</span><span class="sxs-lookup"><span data-stu-id="65b80-200">Subscribing to receive user's notifications</span></span> 

<span data-ttu-id="65b80-201">Для вашего приложения необходимо создать экземпляр объекта **UserDataFeed** для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="65b80-201">You need to instantiate a **UserDataFeed** object for your application for this signed in user.</span></span> <span data-ttu-id="65b80-202">Ваше приложение определяется по идентификатору кроссплатформенного приложения, указанному в процессе [подключения интерфейсов различных устройств](notifications-integration-cross-device-experiences-onboarding.md).</span><span class="sxs-lookup"><span data-stu-id="65b80-202">Your application is identified by the cross-platform app ID you provided during the [Cross-Device Experiences onboarding](notifications-integration-cross-device-experiences-onboarding.md) process.</span></span>

```ObjectiveC
// Initialize the feed and subscribe for notifications
MCDUserDataFeed* feed = [MCDUserDataFeed getForAccount:account
                        platform:platform
                        activitySourceHost:APP_HOST_NAME];

NSArray<MCDUserDataFeedSyncScope*>* syncScopes = @[ [MCDUserNotificationChannel syncScope] ];
[feed subscribeToSyncScopesAsync:syncScopes
        callback:^(BOOL success __unused, NSError* _Nullable error __unused) {
    // Start syncing down notifications
    [feed startSync];
}];
```

## <a name="receiving-and-managing-user-notifications"></a><span data-ttu-id="65b80-203">Получение уведомлений пользователей и управление ими</span><span class="sxs-lookup"><span data-stu-id="65b80-203">Receiving and managing user notifications</span></span>

<span data-ttu-id="65b80-204">На схеме, представленной ранее в этой статье, показано, что шаблоны программирования для обработки новых входящих уведомлений из сервера приложений и обновление или удаление уведомления, запущенное из другого экземпляра клиента приложения, похожи.</span><span class="sxs-lookup"><span data-stu-id="65b80-204">The flow diagram earlier in this topic shows that the programming patterns to handle a new incoming notifications from an app server and a notification update or deletion initiated from another app client instance are similar.</span></span> <span data-ttu-id="65b80-205">Ниже представлены действия для обработки этих изменений данных.</span><span class="sxs-lookup"><span data-stu-id="65b80-205">The following are the steps for handling these data changes.</span></span> 

### <a name="handling-incoming-push-notification-signal"></a><span data-ttu-id="65b80-206">Обработка сигналов входящих push-уведомлений</span><span class="sxs-lookup"><span data-stu-id="65b80-206">Handling incoming push notification signal</span></span>

<span data-ttu-id="65b80-207">Все типы изменений данных в уведомлениях пользователей создают сигнал, доставляемый клиентам приложений в виде push-уведомления.</span><span class="sxs-lookup"><span data-stu-id="65b80-207">All types of user notification data changes generate a signal that gets delivered to the app clients as a push notification.</span></span> <span data-ttu-id="65b80-208">Для приложений iOS сигнал доставляется как фоновое уведомление APNs об обновлении.</span><span class="sxs-lookup"><span data-stu-id="65b80-208">In the case of an iOS app, the signal is delivered as an APNs background update notification.</span></span> <span data-ttu-id="65b80-209">После получения сигнала сообщения с данными приложение должно вызвать метод **TryParse**, чтобы запустить в SDK получение изменений фактических данных от службы уведомлений Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="65b80-209">On receiving the data message signal, the app should call **TryParse** to trigger the SDK to fetch from the Microsoft Graph notifications service for the actual data changes.</span></span>

```ObjectiveC
// App running in background and received a push notification, launched by user tapping the alert view
MCDConnectedDevicesNotification* notification = [MCDConnectedDevicesNotification tryParse:notificationInfo];
if (notification != nil) {
    [_platformManager.platform processNotificationAsync:notification
            completion:^(NSError* error __unused) {
        // NOTE: it may be useful to attach completion to this async in order to know when the
        // notification is done being processed.
        // This would be a good time to stop a background service or otherwise cleanup.
    }];
} else {
    NSLog(@"Remote notification is not for ConnectedDevicesPlatform, skip processing");
}
```

### <a name="handling-user-notification-data-changes"></a><span data-ttu-id="65b80-210">Обработка изменений данных в уведомлениях пользователей</span><span class="sxs-lookup"><span data-stu-id="65b80-210">Handling user notification data changes</span></span>

<span data-ttu-id="65b80-211">После получения пакетом SDK изменений данных выполняется обратный вызов события, при этом ожидается, что клиент приложения обработает создание, обновление или удаление уведомления.</span><span class="sxs-lookup"><span data-stu-id="65b80-211">After the SDK successfully fetches the data changes, an event callback is invoked and the app client is expected to handle notification creation, update, or deletion.</span></span>

```ObjectiveC
[reader readBatchAsyncWithMaxSize:100 completion:^(NSArray<MCDUserNotification *> * _Nullable notifications,
                                                    NSError * _Nullable error) {
    if (error) {
    } else {
        for (MCDUserNotification* notification in self.notifications) {
        // Handle notification change based on change type;
        }
        }
    }
}];
```

### <a name="update-state-of-a-notification"></a><span data-ttu-id="65b80-212">Обновление состояния уведомлений</span><span class="sxs-lookup"><span data-stu-id="65b80-212">Update state of a notification</span></span>

<span data-ttu-id="65b80-213">Если изменение состояния уведомления инициируется в этом экземпляре клиента приложения (например, если всплывающее уведомление на этом устройстве активировано пользователем), приложение должно вызвать SDK, чтобы обновить состояние уведомления для синхронизации изменения этого состояния на всех устройствах, используемых тем же пользователем.</span><span class="sxs-lookup"><span data-stu-id="65b80-213">If a notification state change is initiated from this app client instance (for example, if the toast notification popup on this device is activated by the user), the app needs to call the SDK to update the notification's state in order to have this state change synced across all devices used by the same user.</span></span> 

```ObjectiveC
- (void)dismissNotification:(MCDUserNotification*)notification {
    if (notification.userActionState == MCDUserNotificationUserActionStateNoInteraction) {
        [self dismissNotificationFromTrayWithId:notification.notificationId];
        notification.userActionState = MCDUserNotificationUserActionStateDismissed;
        [notification saveAsync:^(__unused MCDUserNotificationUpdateResult * _Nullable result, __unused NSError * _Nullable error) {
        // handle result;
         }];
    }
}
```

### <a name="delete-a-notifications"></a><span data-ttu-id="65b80-214">Удаление уведомлений</span><span class="sxs-lookup"><span data-stu-id="65b80-214">Delete a notifications</span></span>

<span data-ttu-id="65b80-215">Если удаление уведомления инициируется в этом экземпляре клиента приложения (например, если связанная с этим уведомлением задача помечена как завершенная и удалена из базы данных вашего приложения), приложение должно вызвать SDK для удаления уведомления, чтобы синхронизировать эту операцию удаления на всех устройствах, используемых тем же пользователем.</span><span class="sxs-lookup"><span data-stu-id="65b80-215">If a notification deletion is initiated from this app client instance (for example, if the task corresponding to this notification is marked as complete and is removed from your app's database), the app needs to call the SDK to delete the notification in order to have this delete operation synced across all devices used by the same user.</span></span> 

<span data-ttu-id="65b80-216">Уведомление удаляется из хранилища уведомлений пользователя только при истечении срока действия уведомления или при удалении явным образом.</span><span class="sxs-lookup"><span data-stu-id="65b80-216">A notification is removed from the user notification store only if it is expired or explicitly deleted.</span></span> <span data-ttu-id="65b80-217">Уведомление пользователя не удаляется при обновлении свойства **UserActionState** с присвоением значения Dismissed, так как семантическое определение **UserActionState** задается самим приложением.</span><span class="sxs-lookup"><span data-stu-id="65b80-217">A user notification is not deleted when you update the **UserActionState** to be Dismissed, because the semantic definition of **UserActionState** is defined by the application itself.</span></span>

```Obj-C
- (void)deleteNotification:(MCDUserNotification*)notification {
    [_channel deleteUserNotificationAsync:notification.notificationId
     completion:^(__unused MCDUserNotificationUpdateResult* _Nullable result, NSError* _Nullable error) {
        // handle result;
     }];
}
```

## <a name="see-also"></a><span data-ttu-id="65b80-218">См. также</span><span class="sxs-lookup"><span data-stu-id="65b80-218">See also</span></span>

- <span data-ttu-id="65b80-219">[Справочник по API](https://docs.microsoft.com/ru-RU/windows/project-rome/notifications/api-reference-for-ios/) содержит информацию о всех API-интерфейсах, связанных с функциями уведомлений в SDK.</span><span class="sxs-lookup"><span data-stu-id="65b80-219">[API reference](https://docs.microsoft.com/en-us/windows/project-rome/notifications/api-reference-for-ios/) for the full set of APIs related to notification features in the SDK.</span></span> 
- <span data-ttu-id="65b80-220">[Пример клиентского кода](https://github.com/Microsoft/project-rome/tree/master/iOS/samples/GraphNotifications) для приложений Android.</span><span class="sxs-lookup"><span data-stu-id="65b80-220">[Client-side sample](https://github.com/Microsoft/project-rome/tree/master/iOS/samples/GraphNotifications) for Android apps.</span></span>
- <span data-ttu-id="65b80-221">[Пример серверного кода приложения](notifications-integrating-app-server.md) для публикации уведомлений.</span><span class="sxs-lookup"><span data-stu-id="65b80-221">[App server sample](notifications-integrating-app-server.md) for publishing notifications.</span></span> 
