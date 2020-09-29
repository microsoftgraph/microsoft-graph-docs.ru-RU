---
title: Интеграция приложения Android с клиентским пакетом SDK для уведомления пользователей
description: Интеграция приложения Android с клиентским пакетом SDK уведомления пользователей
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: c56aef1befa98c2082d3476900a8e40c4034653f
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288681"
---
# <a name="integrate-your-android-app-with-the-client-side-sdk-for-user-notifications"></a><span data-ttu-id="8c886-103">Интеграция приложения Android с клиентским пакетом SDK для уведомления пользователей</span><span class="sxs-lookup"><span data-stu-id="8c886-103">Integrate your Android app with the client-side SDK for user notifications</span></span>

<span data-ttu-id="8c886-104">После [регистрации своего приложения](notifications-integration-app-registration.md) на портале Azure и внедрения [использования разных устройств](notifications-integration-cross-device-experiences-onboarding.md) в Центре разработки партнеров следующий этап состоит в интеграции вашего клиентского приложения с клиентским пакетом SDK для приложений Android.</span><span class="sxs-lookup"><span data-stu-id="8c886-104">After you [register your app](notifications-integration-app-registration.md) in the Azure Portal and onboard your [cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md) in the Partner Dev Center, the next step is to integrate your client app with the client-side SDK for Android apps.</span></span>  

<span data-ttu-id="8c886-105">С помощью клиентского пакета SDK ваше приложение может выполнять необходимые действия регистрации, чтобы начать получение уведомлений, опубликованных вашим сервером приложений и предназначенных для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c886-105">With the client-side SDK, your app can perform the necessary registration steps to start receiving notifications published from your app server targeted at the user who is currently signed in.</span></span> <span data-ttu-id="8c886-106">После этого SDK управляет уведомлениями на стороне клиента, включая получение новых входящих уведомлений, управление состоянием уведомлений для осуществления таких сценариев, как универсальное закрытие и получение полного журнала уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8c886-106">The SDK then manages the notifications on the client side, including receiving new incoming notifications, managing the state of notifications to achieve scenarios like universal dismiss, and retrieving full notification history.</span></span> 

## <a name="new-incoming-notification-flow"></a><span data-ttu-id="8c886-107">Поток новых входящих уведомлений</span><span class="sxs-lookup"><span data-stu-id="8c886-107">New incoming notification flow</span></span>

<span data-ttu-id="8c886-108">Поток данных для получения новых входящих уведомлений показан на схеме ниже.</span><span class="sxs-lookup"><span data-stu-id="8c886-108">For receiving new incoming notifications, the data flow is shown in the following diagram.</span></span>

![Поток новых уведомлений для приложения Android](images/notifications-new-notification-android.png)

<span data-ttu-id="8c886-110">Процесс включает несколько компонентов:</span><span class="sxs-lookup"><span data-stu-id="8c886-110">he process involves a few components:</span></span>

* <span data-ttu-id="8c886-111">Сервер приложений — серверный компонент вашего приложения</span><span class="sxs-lookup"><span data-stu-id="8c886-111">App server - The back end of your application</span></span>
* <span data-ttu-id="8c886-112">Клиент приложения — внешний интерфейс вашего приложения (приложение UWP, приложение Android или приложение iOS)</span><span class="sxs-lookup"><span data-stu-id="8c886-112">App client - The front end of your application (a UWP app, an Android app, or an iOS app)</span></span>
* <span data-ttu-id="8c886-113">Уведомления Microsoft Graph — компонент службы, позволяющий публиковать, хранить и синхронизировать уведомления пользователей на разных экземплярах клиентов приложения для разных устройств и платформ</span><span class="sxs-lookup"><span data-stu-id="8c886-113">Microsoft Graph notifications - The service component that enables user notifications to be published, stored, and synced across different instances of app clients across devices and platforms</span></span>
* <span data-ttu-id="8c886-114">FCM (Firebase Cloud Messaging) — служба push-уведомлений, предусмотренная в Android в составе сервисов Google Play.</span><span class="sxs-lookup"><span data-stu-id="8c886-114">FCM - Firebase Cloud Messaging, the push notification service provided by Android as a part of Google Play Services.</span></span> <span data-ttu-id="8c886-115">Уведомления Microsoft Graph используют эту службу для сообщения клиентам приложений Android об изменениях данных в уведомлениях пользователей.</span><span class="sxs-lookup"><span data-stu-id="8c886-115">Microsoft Graph notifications use this service to signal the Android app clients about user notification data changes.</span></span>  

<span data-ttu-id="8c886-116">На схеме показаны следующие шаги:</span><span class="sxs-lookup"><span data-stu-id="8c886-116">The diagram shows the following steps:</span></span> 

1. <span data-ttu-id="8c886-117">Логика приложения.</span><span class="sxs-lookup"><span data-stu-id="8c886-117">Application logic.</span></span> <span data-ttu-id="8c886-118">Этот шаг фиксирует событие, запускающее публикацию уведомления для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c886-118">This step captures what triggers the notification to be published to the user.</span></span> <span data-ttu-id="8c886-119">Эта логика зависит от приложения и может относиться к обновлению события или данных других элементов в Microsoft Graph, например новому событию календаря, назначению задачи или другому действию, о котором ваша служба приложений хочет уведомить пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c886-119">This is app-specific logic, and can be an event or data update about something else in Microsoft Graph, such as a new calendar event or task assignment, or else your app service wants to notify the user about.</span></span>
2. <span data-ttu-id="8c886-120">Сервер приложений публикует уведомление для целевого пользователя с помощью API уведомлений Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8c886-120">The app server publishes a notification to the targeted user via the Microsoft Graph notifications API.</span></span> <span data-ttu-id="8c886-121">Дополнительные сведения см. в статье [Серверная интеграция](notifications-integrating-app-server.md).</span><span class="sxs-lookup"><span data-stu-id="8c886-121">For more details, see [server side integration](notifications-integrating-app-server.md).</span></span>
3. <span data-ttu-id="8c886-122">После получения веб-запроса, содержащего новое уведомление, служба уведомлений Microsoft Graph безопасно сохраняет контент уведомления в облаке для этого приложения и этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c886-122">On receiving the web request containing the new notification, Microsoft Graph notifications persists the content of the notification securely in the cloud for this app and this user.</span></span>
4. <span data-ttu-id="8c886-123">Для каждого экземпляра клиента приложения, подписывающегося на получение уведомлений для этого пользователя, служба уведомлений Microsoft Graph отправляет сигнал для уведомления клиента приложения посредством собственной службы push-уведомлений, предоставляемой операционной системой.</span><span class="sxs-lookup"><span data-stu-id="8c886-123">For each app client instance subscribing to receive notifications for this user, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="8c886-124">В этом случае мы имеем дело с приложением Android, использующим [сообщение с данными FCM](https://firebase.google.com/docs/cloud-messaging/concept-options) для отправки сигнала.</span><span class="sxs-lookup"><span data-stu-id="8c886-124">In this case, the application is an Android app, and it uses [FCM data message](https://firebase.google.com/docs/cloud-messaging/concept-options) to send the signal.</span></span> 
5. <span data-ttu-id="8c886-125">После того, как приложение получит сигнал с помощью входящего push-уведомления, оно обращается к пакету SDK за получением изменений в хранилище уведомлений пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c886-125">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
6. <span data-ttu-id="8c886-126">SDK создает безопасное и соответствующее требованиям соединение с хранилищем уведомлений пользователя в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8c886-126">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
7. <span data-ttu-id="8c886-127">SDK получает изменения данных, то есть, в этом случае, — новый контент уведомления.</span><span class="sxs-lookup"><span data-stu-id="8c886-127">The SDK gets the data changes - in this case, the new notification contents.</span></span> 
8. <span data-ttu-id="8c886-128">SDK выполняет обратные вызовы события, чтобы уведомить приложение после успешного получения изменений.</span><span class="sxs-lookup"><span data-stu-id="8c886-128">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
9. <span data-ttu-id="8c886-129">Логика приложения.</span><span class="sxs-lookup"><span data-stu-id="8c886-129">Application logic.</span></span> <span data-ttu-id="8c886-130">Этот шаг фиксирует выбранное приложением действие внутри обратного вызова события.</span><span class="sxs-lookup"><span data-stu-id="8c886-130">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="8c886-131">Обычно это приводит к локальным изменениям данных приложения и локальным обновлениям пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8c886-131">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="8c886-132">В этом случае приложение обычно создает всплывающее уведомление, чтобы уведомить пользователя о содержимом уведомления.</span><span class="sxs-lookup"><span data-stu-id="8c886-132">In this case,  the app usually constructs a toast notification popup to notify the user about the notification contents.</span></span>

## <a name="notification-update-flow"></a><span data-ttu-id="8c886-133">Поток обновления уведомлений</span><span class="sxs-lookup"><span data-stu-id="8c886-133">Notification update flow</span></span>

<span data-ttu-id="8c886-134">Одно из основных преимуществ использования уведомлений Microsoft Graph заключается в безопасном сохранении уведомлений в облаке и преобразование их в тип ресурса с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="8c886-134">One of the main benefits for using Microsoft Graph notifications is that it persists notifications in the cloud securely and turns them into a stateful resource type.</span></span> <span data-ttu-id="8c886-135">Это может помочь вашему приложению управлять правильным состоянием уведомлений и синхронизировать его на разных устройствах для этого же вошедшего пользователя в сценарии с разными устройствами.</span><span class="sxs-lookup"><span data-stu-id="8c886-135">Therefore, it can help your application to manage and sync the correct state of the notifications across different devices for the same signed in user in a cross-device scenario.</span></span> <span data-ttu-id="8c886-136">Если уведомление помечено как закрытое или прочитанное на одном устройстве, другие устройства могут уведомляться в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="8c886-136">When a notification is marked as dismissed, or marked as read on one device, the other devices can be notified in real-time.</span></span> <span data-ttu-id="8c886-137">"Обработано однажды, закрыто везде" может стать истинным обещанием в рамках интерфейса уведомлений для ваших пользователей.</span><span class="sxs-lookup"><span data-stu-id="8c886-137">"Handled once, dismissed everywhere" can become a true promise as part of the notification experience for your users.</span></span> 

<span data-ttu-id="8c886-138">На схеме ниже показан поток данных для изменения состояния уведомления или удаления уведомления на одном устройстве и получения/обработки изменения состояния или удаления на другом устройстве.</span><span class="sxs-lookup"><span data-stu-id="8c886-138">The following diagram shows the data flow for changing the state of a notification or deleting the notification on one device, and receiving/handling the state change or the deletion on another device.</span></span>

![Поток обновления уведомлений для приложения Android](images/notifications-notification-update-android.png)

<span data-ttu-id="8c886-140">Обратите внимание, что вторая часть потока похожа на поток для обработки новых входящих уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8c886-140">Notice that the second part of the flow is similar to the flow for handling new incoming notifications.</span></span> <span data-ttu-id="8c886-141">Это сделано намеренно. Шаблон программирования SDK создан таким образом, чтобы клиент приложения мог обрабатывать все типы изменений данных в уведомлениях пользователей (новые входящие уведомления, изменения состояния уведомления, удаление уведомления) аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="8c886-141">This is by design - the  programming pattern of the SDK is designed so that the application client can handle all types of user notification data changes (new incoming notifications, notification state changes, notification deleted) in a similar way.</span></span>  

<span data-ttu-id="8c886-142">На схеме показаны следующие шаги:</span><span class="sxs-lookup"><span data-stu-id="8c886-142">The diagram shows the following steps:</span></span>

1. <span data-ttu-id="8c886-143">Логика приложения.</span><span class="sxs-lookup"><span data-stu-id="8c886-143">Application logic.</span></span> <span data-ttu-id="8c886-144">Некоторое событие запускает изменение или удаление уведомления.</span><span class="sxs-lookup"><span data-stu-id="8c886-144">Something triggers the notification to be changed or deleted.</span></span> <span data-ttu-id="8c886-145">В принципе, любое событие может вызвать изменение уведомления.</span><span class="sxs-lookup"><span data-stu-id="8c886-145">In general, any event can trigger a notification to change.</span></span> 
2. <span data-ttu-id="8c886-146">Приложение вызывает SDK клиента, чтобы обновить или удалить уведомление.</span><span class="sxs-lookup"><span data-stu-id="8c886-146">App calling into the client SDK to update or delete a notification.</span></span> <span data-ttu-id="8c886-147">В настоящее время представлено два свойства, связанных с изменением состояния: **userActionState** и **readState**, но ваше приложение может определять эти состояния и необходимость их обновления.</span><span class="sxs-lookup"><span data-stu-id="8c886-147">Currently, we expose two properties regarding state changes - **userActionState** and **readState** - but your application can define these states and when they need to be updated.</span></span> <span data-ttu-id="8c886-148">Например, если пользователь закрывает всплывающее уведомление, вы можете обновить свойство **userActionState**, присвоив ему значение Dismissed.</span><span class="sxs-lookup"><span data-stu-id="8c886-148">For example, when a user dismisses the notification popup, you can update the **userActionState** to be Dismissed.</span></span> <span data-ttu-id="8c886-149">Когда пользователь щелкает всплывающее уведомление и запускает приложение для использования соответствующего контента приложения, вы можете обновить свойство **userActionState**, присвоив ему значение Activated, и обновить свойство **readState**, присвоив ему значение Read.</span><span class="sxs-lookup"><span data-stu-id="8c886-149">When a user clicks the notification popup and launches the app to consume corresponding app content, you can update the **userActionState** to be Activated and update the **readState** to be Read.</span></span> 
3. <span data-ttu-id="8c886-150">После вызова соответствующего API для обновления или удаления уведомления пакет SDK вызовет хранилище уведомлений пользователя в облаке, чтобы развернуть это изменение для других экземпляров клиента приложения с этим вошедшим пользователем.</span><span class="sxs-lookup"><span data-stu-id="8c886-150">After the corresponding API is called to update or delete a notification, the SDK will call into the user notification store in the cloud in order to fan-out this change to the other app client instances with the same signed in user.</span></span> 
4. <span data-ttu-id="8c886-151">После получения от клиента запроса на обновление или удаление служба уведомлений Microsoft Graph обновит хранилище уведомлений и определит другие экземпляры клиентов приложения, подписанные на это изменение.</span><span class="sxs-lookup"><span data-stu-id="8c886-151">On receiving the update/delete request from a client, Microsoft Graph notifications will update the notification store, and identify the other app client instances that subscribed to this change.</span></span>
5. <span data-ttu-id="8c886-152">Для каждой подписки экземпляра клиента приложения служба уведомлений Microsoft Graph отправляет сигнал для уведомления клиента приложения посредством собственной службы push-уведомлений, предоставляемой операционной системой.</span><span class="sxs-lookup"><span data-stu-id="8c886-152">For each app client subscription, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="8c886-153">В этом случае применяется приложение Android, использующее [сообщение с данными FCM](https://firebase.google.com/docs/cloud-messaging/concept-options) для отправки сигнала.</span><span class="sxs-lookup"><span data-stu-id="8c886-153">In this case, this is an Android app, and it uses [FCM data message](https://firebase.google.com/docs/cloud-messaging/concept-options) to send the signal.</span></span> 
6. <span data-ttu-id="8c886-154">После того, как приложение получит сигнал с помощью входящего push-уведомления, оно обращается к пакету SDK за получением изменений в хранилище уведомлений пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c886-154">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
7. <span data-ttu-id="8c886-155">SDK создает безопасное и соответствующее требованиям соединение с хранилищем уведомлений пользователя в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8c886-155">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
8. <span data-ttu-id="8c886-156">SDK получает изменения данных: в этом случае изменениями являются обновления состояния уведомления или удаления уведомления.</span><span class="sxs-lookup"><span data-stu-id="8c886-156">The SDK gets the data changes - in this case, the changes are notification state updates or notification deletions.</span></span> 
9. <span data-ttu-id="8c886-157">SDK выполняет обратные вызовы события, чтобы уведомить приложение после успешного получения изменений.</span><span class="sxs-lookup"><span data-stu-id="8c886-157">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
10. <span data-ttu-id="8c886-158">Логика приложения.</span><span class="sxs-lookup"><span data-stu-id="8c886-158">Application logic.</span></span> <span data-ttu-id="8c886-159">Этот шаг фиксирует выбранное приложением действие внутри обратного вызова события.</span><span class="sxs-lookup"><span data-stu-id="8c886-159">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="8c886-160">Обычно это приводит к локальным изменениям данных приложения и локальным обновлениям пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8c886-160">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="8c886-161">В этом случае приложение должно локально обновить пользовательский интерфейс, чтобы отобразить изменение состояния, так как имеются обновления уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8c886-161">In this case, because there are notification updates, the app should update the UI locally to reflect the state change.</span></span> <span data-ttu-id="8c886-162">Например, если уведомление помечено как активированное, вы можете удалить соответствующее сообщение в области уведомлений Android, чтобы достичь результата "обработано однажды, закрыто везде".</span><span class="sxs-lookup"><span data-stu-id="8c886-162">For example, if a notification is marked as activated, you can remove the corresponding notification message inside Android's notification tray to achieve "handled once, dismissed everywhere".</span></span> 

<span data-ttu-id="8c886-163">Дополнительные сведения об уведомлениях Microsoft Graph см. в статье [Общие сведения об уведомлениях Microsoft Graph](notifications-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8c886-163">For more information about Microsoft Graph notifications, see [Microsoft Graph Notifications overview](notifications-concept-overview.md).</span></span> <span data-ttu-id="8c886-164">Дополнительные сведения о всех действиях, требующихся для интеграции с уведомлениями Microsoft Graph, см. в [обзоре интеграции](notifications-integration-e2e-overview.md) уведомлений Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8c886-164">For more information about the steps required to integrate with Microsoft Graph notifications from end to end, see Microsoft Graph notifications [integration overview](notifications-integration-e2e-overview.md).</span></span>

## <a name="development-environment-and-requirements"></a><span data-ttu-id="8c886-165">Среда и требования разработки</span><span class="sxs-lookup"><span data-stu-id="8c886-165">Development environment and requirements</span></span>

<span data-ttu-id="8c886-166">Чтобы использовать уведомления Microsoft Graph, вам потребуется среда IDE для разработки приложений Android и устройство Android с одной из поддерживаемых архитектур (**armeabi-v7a**, **arm64-v8a**, **x86** или **x86_64**) или эмулятор.</span><span class="sxs-lookup"><span data-stu-id="8c886-166">To use Microsoft Graph notifications, you will need an Android app development IDE and an Android device with one of the supported architectures (**armeabi-v7a**, **arm64-v8a**, **x86**, or **x86_64**) or an emulator.</span></span> <span data-ttu-id="8c886-167">Система должна работать под управлением Android 4.4.2 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="8c886-167">The system must be running Android 4.4.2 or later.</span></span>

## <a name="adding-the-sdk-to-your-project"></a><span data-ttu-id="8c886-168">Добавление SDK в проект</span><span class="sxs-lookup"><span data-stu-id="8c886-168">Adding the SDK to your project</span></span>

<span data-ttu-id="8c886-169">Вставьте следующие ссылки на репозиторий в файл *build.gradle* в корневой папке проекта.</span><span class="sxs-lookup"><span data-stu-id="8c886-169">Insert the following repository references into the *build.gradle* file at the root of your project.</span></span>

```Java
allprojects {
    repositories {
    jcenter()
    maven { url 'https://maven.google.com' }
    maven { url 'https://projectrome.bintray.com/maven/' }
    }
}
```

<span data-ttu-id="8c886-170">Затем вставьте следующую зависимость в файл _build.gradle_, находящийся в папке проекта.</span><span class="sxs-lookup"><span data-stu-id="8c886-170">Then, insert the following dependency into the _build.gradle_ file that is in your project folder.</span></span>

```Java
dependencies { 
    ...
    implementation 'com.microsoft.connecteddevices:connecteddevices-sdk:+'
}
```

<span data-ttu-id="8c886-171">Если вы хотите использовать ProGuard в своем приложении, добавьте правила ProGuard для этих новых API.</span><span class="sxs-lookup"><span data-stu-id="8c886-171">If you want to use ProGuard in your app, add the ProGuard Rules for these new APIs.</span></span> <span data-ttu-id="8c886-172">Создайте файл *proguard rules.txt* в папке *App* своего проекта и вставьте содержимое файла [ProGuard_Rules_for_Android_Rome_SDK.txt](https://github.com/Microsoft/project-rome/blob/master/Android/ProGuard_Rules_for_Android_Rome_SDK.txt).</span><span class="sxs-lookup"><span data-stu-id="8c886-172">Create a file called *proguard-rules.txt* in the *App* folder of your project, and paste in the contents of [ProGuard_Rules_for_Android_Rome_SDK.txt](https://github.com/Microsoft/project-rome/blob/master/Android/ProGuard_Rules_for_Android_Rome_SDK.txt).</span></span>
<span data-ttu-id="8c886-173">В файле *AndroidManifest.xml* своего проекта добавьте следующие разрешения в элемент `manifest` (если они там отсутствуют).</span><span class="sxs-lookup"><span data-stu-id="8c886-173">In your project's *AndroidManifest.xml* file, add the following permissions inside the `manifest` element (if they are not already present).</span></span> <span data-ttu-id="8c886-174">Это дает вашему приложению разрешение на подключение к Интернету и включение обнаружения Bluetooth на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8c886-174">This gives your app permission to connect to the Internet and to enable Bluetooth discovery on your device.</span></span>
<span data-ttu-id="8c886-175">Обратите внимание, что разрешения, связанные с Bluetooth, необходимы только для использования обнаружения Bluetooth; они не нужны для других функций на платформе подключенных устройств.</span><span class="sxs-lookup"><span data-stu-id="8c886-175">Note that the Bluetooth-related permissions are only necessary for using Bluetooth discovery; they are not needed for the other features in the Connected Devices Platform.</span></span> <span data-ttu-id="8c886-176">Кроме того, `ACCESS_COARSE_LOCATION` требуется только для Android SDK 21 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="8c886-176">Additionally, `ACCESS_COARSE_LOCATION` is only required on Android SDKs 21 and later.</span></span> <span data-ttu-id="8c886-177">На Android SDK 23 и более поздних версиях вы также должны запрашивать у пользователя предоставление доступа к расположению во время выполнения.</span><span class="sxs-lookup"><span data-stu-id="8c886-177">On Android SDKs 23 and later, you must also prompt the user to grant location access at runtime.</span></span>

```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.BLUETOOTH" />
<uses-permission android:name="android.permission.BLUETOOTH_ADMIN" />
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
```
<span data-ttu-id="8c886-178">Затем перейдите к классам действий, в которых нужно разместить функции подключенных устройств.</span><span class="sxs-lookup"><span data-stu-id="8c886-178">Next, go to the activity classes where you would like the Connected Devices functionality to be located.</span></span> <span data-ttu-id="8c886-179">Импортируйте указанные ниже пространства имен.</span><span class="sxs-lookup"><span data-stu-id="8c886-179">Import the following namespaces.</span></span>

```java
import com.microsoft.connecteddevices;
import com.microsoft.connecteddevices.userdata;
import com.microsoft.connecteddevices.userdata.usernotifications;
```

## <a name="initializing-the-connected-device-platforms"></a><span data-ttu-id="8c886-180">Инициализация платформ подключенных устройств</span><span class="sxs-lookup"><span data-stu-id="8c886-180">Initializing the Connected Device Platforms</span></span>

<span data-ttu-id="8c886-181">Клиентский SDK создан на основе инфраструктуры, называемой платформой подключенных устройств.</span><span class="sxs-lookup"><span data-stu-id="8c886-181">The client-side SDK is built on top of an infrastructure called Connected Device Platform.</span></span> <span data-ttu-id="8c886-182">Перед использованием каких-либо функций необходимо инициализировать платформу в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="8c886-182">Before any feature can be used, the platform must be initialized within your app.</span></span> <span data-ttu-id="8c886-183">Действия по инициализации должны находиться в методе **OnCreate** класса main, так как они должны быть выполнены до использования сценариев уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8c886-183">The initialization steps should occur in your main class **OnCreate** method, because they are required before the notification scenarios can take place.</span></span>

<span data-ttu-id="8c886-184">Необходимо создать и инициализировать платформу путем создания экземпляра класса [**ConnectedDevicesPlatform**](/java/api/com.microsoft.connecteddevices.connecteddevicesplatform?view=rome-android-latest).</span><span class="sxs-lookup"><span data-stu-id="8c886-184">You must construct and initialize the platform by instantiating the [**ConnectedDevicesPlatform**](/java/api/com.microsoft.connecteddevices.connecteddevicesplatform?view=rome-android-latest) class.</span></span> <span data-ttu-id="8c886-185">Перед этим подключите обработчики событий, так как после запуска платформы могут начать возникать события.</span><span class="sxs-lookup"><span data-stu-id="8c886-185">Before doing that, make sure to hook up event handlers, because after the platform is started, the events might begin to fire.</span></span> 

```java
ConnectedDevicesPlatform platform = new ConnectedDevicesPlatform(context);

platform.getAccountManager().accessTokenRequested().subscribe((accountManager, args) -> onAccessTokenRequested(accountManager, args));
platform.getAccountManager().accessTokenInvalidated().subscribe((accountManager, args) -> onAccessTokenInvalidated(accountManager, args));
platform.getNotificationRegistrationManager().notificationRegistrationStateChanged().subscribe((notificationRegistrationManager, args) -> onNotificationRegistrationStateChanged(notificationRegistrationManager, args));

platform.start();
```

### <a name="handling-account-access-token"></a><span data-ttu-id="8c886-186">Обработка маркера доступа учетной записи</span><span class="sxs-lookup"><span data-stu-id="8c886-186">Handling account access token</span></span>

<span data-ttu-id="8c886-187">Все веб-вызовы, выполняемые SDK, включая получение контента нового входящего уведомления, обновление состояний уведомлений и т. д., считываются из данных пользователя или записываются в них, поэтому всегда требуется действующий маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="8c886-187">All the web calls the SDK makes, including retrieving the content of a new incoming notification, updating notification states, and more, are reading from or writing to the user's data, and therefore always require a valid access token.</span></span> <span data-ttu-id="8c886-188">При использовании SDK требуется обработка следующих событий, вызываемых, когда маркер доступа запрашивается или становится недействительным. Это необходимо, чтобы правильно обрабатывать маркер доступа пользователя после инициализации платформы.</span><span class="sxs-lookup"><span data-stu-id="8c886-188">The SDK requires you to handle the following events - invoked when an access token is requested or invalidated - to make sure that after the platform is initialized, your access token for the user is handled correctly.</span></span> 

#### <a name="accesstokenrequested"></a><span data-ttu-id="8c886-189">accessTokenRequested</span><span class="sxs-lookup"><span data-stu-id="8c886-189">accessTokenRequested</span></span> 

<span data-ttu-id="8c886-190">Полную реализацию см. в [примере приложения Android](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span><span class="sxs-lookup"><span data-stu-id="8c886-190">For a full implementation, see the [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

```Java
private void onAccessTokenRequested(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenRequestedEventArgs args) {
    ConnectedDevicesAccessTokenRequest request = args.getRequest();
    List<String> scopes = request.getScopes();

    // We always need to complete the request, even if a matching account is not found
    if (account == null) {
        request.completeWithErrorMessage("The app could not find a matching ConnectedDevicesAccount to get a token");
        return;
    }

    // Complete the request with a token
    account.getAccessTokenAsync(scopes)
        .thenAcceptAsync((String token) -> {
            request.completeWithAccessToken(token);
        }).exceptionally(throwable -> {
            request.completeWithErrorMessage("The Account could not return a token with those scopes");
            return null;
    });
}
```

#### <a name="accesstokeninvalidated"></a><span data-ttu-id="8c886-191">accessTokenInvalidated</span><span class="sxs-lookup"><span data-stu-id="8c886-191">accessTokenInvalidated</span></span>

<span data-ttu-id="8c886-192">Полную реализацию см. в [примере приложения Android](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span><span class="sxs-lookup"><span data-stu-id="8c886-192">For a full implementation, see the  [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

```Java
private void onAccessTokenInvalidated(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenInvalidatedEventArgs args, List<Account> accounts) {
    Log.i(TAG, "Token invalidated for account: " + args.getAccount().getId());
}
```

### <a name="handling-push-registration-expiration"></a><span data-ttu-id="8c886-193">Обработка истечения срока регистрации для push-уведомлений</span><span class="sxs-lookup"><span data-stu-id="8c886-193">Handling push registration expiration</span></span> 

<span data-ttu-id="8c886-194">Уведомления Microsoft Graph используют FCM (собственная платформа push-уведомлений в Android) для отправки сигнала клиентскому приложению об изменениях данных в уведомлениях пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c886-194">Microsoft Graph notifications uses FCM, the native push platform on Android, to signal the client application on user notifications data changes.</span></span> <span data-ttu-id="8c886-195">Это происходит, когда новые входящие уведомления публикуются с вашего сервера приложений или когда обновляется состояние любого уведомления на другом устройстве с тем же вошедшим пользователем в сценарии с разными устройствами.</span><span class="sxs-lookup"><span data-stu-id="8c886-195">This happens when new incoming notifications are published from your app server, or when any notification's state is updated on a different device with the same signed in user in a cross-device scenario.</span></span> 

<span data-ttu-id="8c886-196">Поэтому требуется действующий маркер FCM, обеспечивающий передачу сообщений с уведомлениями о данных.</span><span class="sxs-lookup"><span data-stu-id="8c886-196">Therefore, a valid FCM token that allows data notification messages to come through successfully is required.</span></span> <span data-ttu-id="8c886-197">Следующий обратный вызов события обрабатывает истечения срока действия маркера FCM для push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8c886-197">The following event callback handles FCM push token expirations.</span></span> 

#### <a name="notificationregistrationstatechanged"></a><span data-ttu-id="8c886-198">notificationRegistrationStateChanged</span><span class="sxs-lookup"><span data-stu-id="8c886-198">notificationRegistrationStateChanged</span></span>

<span data-ttu-id="8c886-199">Полную реализацию см. в [примере приложения Android](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span><span class="sxs-lookup"><span data-stu-id="8c886-199">For a full implementation, see the  [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

## <a name="signing-in-your-user"></a><span data-ttu-id="8c886-200">Вход пользователя в систему</span><span class="sxs-lookup"><span data-stu-id="8c886-200">Signing in your user</span></span>

<span data-ttu-id="8c886-201">Уведомления Microsoft Graph, как и многие другие типы ресурсов в Microsoft Graph, ориентированы на пользователей.</span><span class="sxs-lookup"><span data-stu-id="8c886-201">Microsoft Graph notifications, like many other resource types in Microsoft Graph, are centralized around users.</span></span> <span data-ttu-id="8c886-202">Чтобы приложение могло подписаться на уведомления и могло начать получать уведомления для пользователя, вошедшего в систему, сначала необходимо получить действующий маркер OAuth для использования в процессе регистрации.</span><span class="sxs-lookup"><span data-stu-id="8c886-202">In order for your app to subscribe to and start receiving notifications for the signed in user, you first need to obtain a valid OAuth token to be used in the registration process.</span></span> <span data-ttu-id="8c886-203">Вы можете использовать любой удобный способ создания маркеров OAuth и управления ими.</span><span class="sxs-lookup"><span data-stu-id="8c886-203">You can use your preferred method of generating and managing the OAuth tokens.</span></span> <span data-ttu-id="8c886-204">В примере приложения используется ADAL.</span><span class="sxs-lookup"><span data-stu-id="8c886-204">The sample app used ADAL.</span></span> 

<span data-ttu-id="8c886-205">Если вы используете учетную запись Майкрософт, необходимо включить следующие разрешения в запрос входа: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry` и `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span><span class="sxs-lookup"><span data-stu-id="8c886-205">If you're using a Microsoft account, you will need to include the following permissions in your sign-in request: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, and `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span></span> 

<span data-ttu-id="8c886-206">Если вы используете учетную запись Azure AD, необходимо запросить следующую аудиторию: `https://cdpcs.access.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="8c886-206">If you're using an Azure AD account, you'll need to request the following audience: `https://cdpcs.access.microsoft.com`.</span></span>

## <a name="adding-the-user-account-to-the-platform"></a><span data-ttu-id="8c886-207">Добавление учетной записи пользователя в платформу</span><span class="sxs-lookup"><span data-stu-id="8c886-207">Adding the user account to the platform</span></span> 

<span data-ttu-id="8c886-208">Необходимо зарегистрировать учетную запись вошедшего пользователя в SDK, что включает добавление учетной записи и регистрацию канала push-уведомлений для получения начальных push-уведомлений через FCM.</span><span class="sxs-lookup"><span data-stu-id="8c886-208">You need to register the signed in user account with the SDK, which involves adding the account and registering a push channel in order to receive the initial push notifications through FCM.</span></span> 

```Java
public AsyncOperation<Boolean> prepareAccountAsync(final Context context) {
    // Accounts can be in 3 different scenarios:
    // 1: cached account in good standing (initialized in the SDK and our token cache).
    // 2: account missing from the SDK but present in our cache: Add and initialize account.
    // 3: account missing from our cache but present in the SDK. Log the account out async

    // Subcomponents (e.g. UserDataFeed) can only be initialized when an account is in both the app cache
    // and the SDK cache.
    // For scenario 1, initialize our subcomponents.
    // For scenario 2, subcomponents will be initialized after InitializeAccountAsync registers the account with the SDK.
    // For scenario 3, InitializeAccountAsync will unregister the account and subcomponents will never be initialized.
    switch (mState) {
        // Scenario 1
        case IN_APP_CACHE_AND_SDK_CACHE:
            mUserNotificationsManager = new UserNotificationsManager(context, mAccount, mPlatform);
            return registerAccountWithSdkAsync();
        // Scenario 2
        case IN_APP_CACHE_ONLY: {
            // Add the this account to the ConnectedDevicesPlatform.AccountManager
            return mPlatform.getAccountManager().addAccountAsync(mAccount).thenComposeAsync((ConnectedDevicesAddAccountResult result) -> {
                // We failed to add the account, so exit with a failure to prepare bool
                if (result.getStatus() != ConnectedDevicesAccountAddedStatus.SUCCESS) {
                    result.getStatus());
                    return AsyncOperation.completedFuture(false);
                }

                // Set the registration state of this account as in both app and sdk cache
                mState = AccountRegistrationState.IN_APP_CACHE_AND_SDK_CACHE;
                mUserNotificationsManager = new UserNotificationsManager(context, mAccount, mPlatform);
                return registerAccountWithSdkAsync();
            });
        }
        // Scenario 3
        case IN_SDK_CACHE_ONLY:
            // Remove the account from the SDK since the app has no knowledge of it
            mPlatform.getAccountManager().removeAccountAsync(mAccount);
            // This account could not be prepared
            return AsyncOperation.completedFuture(false);
        default:
            // This account could not be prepared
            Log.e(TAG, "Failed to prepare account " + mAccount.getId() + " due to unknown state!");
            return AsyncOperation.completedFuture(false);
    }
}
```

```Java
public AsyncOperation<Boolean> registerAccountWithSdkAsync() {
    if (mState != AccountRegistrationState.IN_APP_CACHE_AND_SDK_CACHE) {
        AsyncOperation<Boolean> toReturn = new AsyncOperation<>();
        toReturn.completeExceptionally(new IllegalStateException("Cannot register this account due to bad state: " + mAccount.getId()));
        return toReturn;
    }

    // Grab the shared GCM/FCM notification token from this app's BroadcastReceiver
    return RomeNotificationReceiver.getNotificationRegistrationAsync().thenComposeAsync((ConnectedDevicesNotificationRegistration notificationRegistration) -> {
        // Perform the registration using the NotificationRegistration
        return mPlatform.getNotificationRegistrationManager().registerAsync(mAccount, notificationRegistration)
            .thenComposeAsync((result) -> {
                if (result.getStatus() == ConnectedDevicesNotificationRegistrationStatus.SUCCESS) {
                    Log.i(TAG, "Successfully registered account " + mAccount.getId() + " for cloud notifications");
                } else {
                    // It would be a good idea for apps to take a look at the different statuses here and perhaps attempt some sort of remediation.
                    // For example, token request failed could mean that the user needs to sign in again. An app could prompt the user for this action 
                    // and retry the operation afterwards.
                    Log.e(TAG, "Failed to register account " + mAccount.getId() + " for cloud notifications!");
                    return AsyncOperation.completedFuture(false);
                }

                return mUserNotificationsManager.registerForAccountAsync();
            });
    });
}
```

## <a name="subscribing-to-receive-users-notifications"></a><span data-ttu-id="8c886-209">Подписка для получения уведомлений пользователей</span><span class="sxs-lookup"><span data-stu-id="8c886-209">Subscribing to receive user's notifications</span></span> 

<span data-ttu-id="8c886-210">Для вашего приложения необходимо создать экземпляр объекта **UserDataFeed** для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c886-210">You need to instantiate a **UserDataFeed** object for your application for this logged in user.</span></span> <span data-ttu-id="8c886-211">Ваше приложение определяется по идентификатору кроссплатформенного приложения, указанному при [внедрении использования разных устройств](notifications-integration-cross-device-experiences-onboarding.md).</span><span class="sxs-lookup"><span data-stu-id="8c886-211">Your application is identified by the cross-platform app ID you provided during the [Cross-Device Experiences onboarding](notifications-integration-cross-device-experiences-onboarding.md).</span></span>

```Java
public UserNotificationsManager(@NonNull Context context, @NonNull ConnectedDevicesAccount account, @NonNull ConnectedDevicesPlatform platform)
{
    Context context = new Context;
    UserDataFeed feed = UserDataFeed.getForAccount(account, platform, Secrets.APP_HOST_NAME);
    UserNotificationChannel channel = new UserNotificationChannel(feed);
    UserNotificationReader reader = channel.createReader();
    reader.dataChanged().subscribe((reader, aVoid) -> readFromCache(reader));
    }
}
```

## <a name="receiving-and-managing-user-notifications"></a><span data-ttu-id="8c886-212">Получение уведомлений пользователей и управление ими</span><span class="sxs-lookup"><span data-stu-id="8c886-212">Receiving and managing user notifications</span></span>

<span data-ttu-id="8c886-213">На схеме, представленной ранее в этой статье, показано, что шаблоны программирования для обработки новых входящих уведомлений из сервера приложений и обновление или удаление уведомления, запущенное из другого экземпляра клиента приложения, похожи.</span><span class="sxs-lookup"><span data-stu-id="8c886-213">The flow diagram earlier in this topic shows that the programming patterns to handle a new incoming notifications from an app server and a notification update or deletion initiated from another app client instance are similar.</span></span> <span data-ttu-id="8c886-214">Ниже представлены действия для обработки этих изменений данных.</span><span class="sxs-lookup"><span data-stu-id="8c886-214">The following are the steps for handling these data changes.</span></span> 

### <a name="handling-incoming-push-notification-signal"></a><span data-ttu-id="8c886-215">Обработка сигналов входящих push-уведомлений</span><span class="sxs-lookup"><span data-stu-id="8c886-215">Handling incoming push notification signal</span></span>

<span data-ttu-id="8c886-216">Все типы изменений данных в уведомлениях пользователей создают сигнал, доставляемый клиентам приложений в виде push-уведомления.</span><span class="sxs-lookup"><span data-stu-id="8c886-216">All types of user notification data changes generate a signal that gets delivered to the app clients as a push notification.</span></span> <span data-ttu-id="8c886-217">Для приложений Android сигнал доставляется как push-сообщение с данными FCM.</span><span class="sxs-lookup"><span data-stu-id="8c886-217">For Android apps, the signal is delivered as a FCM push data message.</span></span> <span data-ttu-id="8c886-218">После получения сигнала сообщения с данными приложение должно вызвать метод **TryParse**, чтобы запустить в SDK получение от службы уведомлений Microsoft Graph изменений фактических данных.</span><span class="sxs-lookup"><span data-stu-id="8c886-218">On receiving the data message signal, the app should call **TryParse** to trigger the SDK to fetch from the Microsoft Graph notifications service for the actual data changes.</span></span>

```Java
public void onMessageReceived(RemoteMessage message) {
    Map data = message.getData();
    ConnectedDevicesNotification notification = ConnectedDevicesNotification.tryParse(data);

    if (notification != null) {
        try {
            ConnectedDevicesPlatform platform = ConnectedDevicesManager.getConnectedDevicesManager(getApplicationContext()).getPlatform();

            // NOTE: it may be useful to attach completion to this async in order to know when the notification is done being processed.
            // This would be a good time to stop a background service or otherwise cleanup.
            platform.processNotificationAsync(notification);
        } catch (Exception e) {
            Log.e(TAG, "Failed to process FCM notification" + e.getMessage());
        }
    }
}
```

### <a name="handling-user-notification-data-changes"></a><span data-ttu-id="8c886-219">Обработка изменений данных в уведомлениях пользователей</span><span class="sxs-lookup"><span data-stu-id="8c886-219">Handling user notification data changes</span></span>

<span data-ttu-id="8c886-220">После получения пакетом SDK изменений данных выполняется обратный вызов события, при этом ожидается, что клиент приложения обработает создание, обновление или удаление уведомления.</span><span class="sxs-lookup"><span data-stu-id="8c886-220">After the SDK successfully completes fetching the data changes, an event callback is invoked and the app client is expected to handle notification creation, update, or deletion.</span></span>

```Java
private void readFromCache(final UserNotificationReader reader)
{
    reader.readBatchAsync(Long.MAX_VALUE).thenAccept(notifications -> {
        synchronized (this) {
            for (final UserNotification notification : notifications) {
                if (notification.getStatus() == UserNotificationStatus.ACTIVE) {
                    removeIf(mNewNotifications, item -> notification.getId().equals(item.getId()));

                    if (notification.getUserActionState() == UserNotificationUserActionState.NO_INTERACTION) {
                        mNewNotifications.add(notification);
                        if (notification.getReadState() != UserNotificationReadState.READ) {
                            clearNotification(mContext.getApplicationContext(), notification.getId());
                            addNotification(mContext.getApplicationContext(), notification.getContent(), notification.getId());
                        }
                    } else {
                        clearNotification(mContext.getApplicationContext(), notification.getId());
                    }

                    removeIf(mHistoricalNotifications, item -> notification.getId().equals(item.getId()));
                    mHistoricalNotifications.add(0, notification);
                } else {
                    removeIf(mNewNotifications, item -> notification.getId().equals(item.getId()));
                    removeIf(mHistoricalNotifications, item -> notification.getId().equals(item.getId()));
                    clearNotification(mContext.getApplicationContext(), notification.getId());
                }
            }
        }

    });
}
```

### <a name="update-state-of-a-notification"></a><span data-ttu-id="8c886-221">Обновление состояния уведомлений</span><span class="sxs-lookup"><span data-stu-id="8c886-221">Update state of a notification</span></span>

<span data-ttu-id="8c886-222">Если изменение состояния уведомления инициируется в этом экземпляре клиента приложения (например, если всплывающее уведомление на этом устройстве активировано пользователем), приложение должно вызвать SDK, чтобы обновить состояние уведомления для синхронизации изменения этого состояния на всех устройствах, используемых тем же пользователем.</span><span class="sxs-lookup"><span data-stu-id="8c886-222">If a notification state change is initiated from this app client instance (for example, if the toast notification popup on this device is activated by the user), the app needs to call the SDK to update the notification's state in order to have this state change synced across all devices used by the same user.</span></span> 

```Java
notification.setUserActionState(UserNotificationUserActionState.ACTIVATED);
notification.saveAsync().whenCompleteAsync((userNotificationUpdateResult, throwable) -> {
    if (throwable == null && userNotificationUpdateResult != null && userNotificationUpdateResult.getSucceeded()) {
        Log.d(TAG, "Successfully activated the notification");
    }
});
```

### <a name="delete-a-notification"></a><span data-ttu-id="8c886-223">Удаление уведомления</span><span class="sxs-lookup"><span data-stu-id="8c886-223">Delete a notification</span></span>

<span data-ttu-id="8c886-224">Если удаление уведомления инициируется в этом экземпляре клиента приложения (например, если связанная с этим уведомлением задача помечена как завершенная и удалена из базы данных вашего приложения), приложение должно вызвать SDK, чтобы удалить уведомление для синхронизации этого удаления на всех устройствах, используемых тем же пользователем.</span><span class="sxs-lookup"><span data-stu-id="8c886-224">If a notification deletion is initiated from this app client instance (for example, if the task corresponding to this notification is marked as complete and is removed from your app's database), the app needs to call the SDK to delete the notification in order to have this delete operation synced across all devices used by the same user.</span></span> 

<span data-ttu-id="8c886-225">Уведомление удаляется из хранилища уведомлений пользователя только при истечении срока действия уведомления или при удалении явным образом.</span><span class="sxs-lookup"><span data-stu-id="8c886-225">A notification is removed from the user notification store only if it is expired or explicitly deleted.</span></span> <span data-ttu-id="8c886-226">Уведомление пользователя не удаляется при обновлении свойства **UserActionState** с присвоением значения Dismissed, так как семантическое определение **UserActionState** задается самим приложением.</span><span class="sxs-lookup"><span data-stu-id="8c886-226">A user notification is not deleted when you update the **UserActionState** to be Dismissed, because the semantic definition of **UserActionState** is defined by the application itself.</span></span>

```Java
channel.deleteUserNotificationAsync(notification.getId()).whenCompleteAsync((userNotificationUpdateResult, throwable) -> {
    if (throwable == null && userNotificationUpdateResult != null && userNotificationUpdateResult.getSucceeded()) {
        Log.d(TAG, "Successfully deleted the notification");
    }
});
```

## <a name="see-also"></a><span data-ttu-id="8c886-227">См. также</span><span class="sxs-lookup"><span data-stu-id="8c886-227">See also</span></span>

- <span data-ttu-id="8c886-228">[Справочник по API](/windows/project-rome/notifications/api-reference-for-android) содержит информацию о всех API-интерфейсах, связанных с функциями уведомлений в SDK.</span><span class="sxs-lookup"><span data-stu-id="8c886-228">[API reference](/windows/project-rome/notifications/api-reference-for-android) for the full set of APIs related to notification features in the SDK.</span></span> 
- <span data-ttu-id="8c886-229">[Пример клиентского кода](https://github.com/Microsoft/project-rome/tree/master/Android/samples/graphnotificationssample) для приложений Android.</span><span class="sxs-lookup"><span data-stu-id="8c886-229">[Client-side sample](https://github.com/Microsoft/project-rome/tree/master/Android/samples/graphnotificationssample) for Android apps.</span></span>
- <span data-ttu-id="8c886-230">[Пример серверного кода приложения](notifications-integrating-app-server.md) для публикации уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8c886-230">[App server sample](notifications-integrating-app-server.md) for publishing notifications.</span></span>
