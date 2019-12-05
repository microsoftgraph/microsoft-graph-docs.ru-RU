---
title: Тип ресурса subscription
description: Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph. На данный момент подписки включены для указанных ниже ресурсов.
localization_priority: Normal
author: piotrci
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 70af093b6ed782ba7bf447c339e5187439849970
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844269"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="5215f-104">Тип ресурса subscription</span><span class="sxs-lookup"><span data-stu-id="5215f-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5215f-105">Подписка позволяет клиентскому приложению получать уведомления об изменениях данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5215f-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="5215f-106">На данный момент подписки включены для указанных ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5215f-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="5215f-107">[Оповещение][] из Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="5215f-107">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="5215f-108">[ChatMessage][] , отправленный через Teams или каналы в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5215f-108">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="5215f-109">[Беседа][] в группе Office 365</span><span class="sxs-lookup"><span data-stu-id="5215f-109">A [conversation][] in an Office 365 group</span></span>
- <span data-ttu-id="5215f-110">Контент в иерархии корневой папки [driveItem][] в OneDrive для бизнеса либо корневой или вложенной папке [driveItem][] в личном хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="5215f-110">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="5215f-111">[Сообщение][], [событие][] или [контакт][] в Outlook</span><span class="sxs-lookup"><span data-stu-id="5215f-111">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="5215f-112">[Пользователь][] или [группа][] в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="5215f-112">A [user][] or [group][] in Azure Active Directory</span></span>

## <a name="methods"></a><span data-ttu-id="5215f-113">Методы</span><span class="sxs-lookup"><span data-stu-id="5215f-113">Methods</span></span>

| <span data-ttu-id="5215f-114">Метод</span><span class="sxs-lookup"><span data-stu-id="5215f-114">Method</span></span> | <span data-ttu-id="5215f-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5215f-115">Return Type</span></span> | <span data-ttu-id="5215f-116">Описание</span><span class="sxs-lookup"><span data-stu-id="5215f-116">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="5215f-117">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="5215f-117">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="5215f-118">subscription</span><span class="sxs-lookup"><span data-stu-id="5215f-118">subscription</span></span>](subscription.md) | <span data-ttu-id="5215f-119">Создание подписки для приложения прослушивателя, чтобы можно было получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5215f-119">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="5215f-120">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="5215f-120">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="5215f-121">subscription</span><span class="sxs-lookup"><span data-stu-id="5215f-121">subscription</span></span>](subscription.md) | <span data-ttu-id="5215f-122">Продлить подписку, обновив срок ее действия.</span><span class="sxs-lookup"><span data-stu-id="5215f-122">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="5215f-123">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="5215f-123">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="5215f-124">subscription</span><span class="sxs-lookup"><span data-stu-id="5215f-124">subscription</span></span>](subscription.md) | <span data-ttu-id="5215f-125">Перечисление активных подписок.</span><span class="sxs-lookup"><span data-stu-id="5215f-125">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="5215f-126">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="5215f-126">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="5215f-127">subscription</span><span class="sxs-lookup"><span data-stu-id="5215f-127">subscription</span></span>](subscription.md) | <span data-ttu-id="5215f-128">Чтение свойств и связей объекта Subscription.</span><span class="sxs-lookup"><span data-stu-id="5215f-128">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="5215f-129">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="5215f-129">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="5215f-130">Нет</span><span class="sxs-lookup"><span data-stu-id="5215f-130">None</span></span> | <span data-ttu-id="5215f-131">Удаление объекта подписки.</span><span class="sxs-lookup"><span data-stu-id="5215f-131">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5215f-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="5215f-132">Properties</span></span>

| <span data-ttu-id="5215f-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="5215f-133">Property</span></span> | <span data-ttu-id="5215f-134">Тип</span><span class="sxs-lookup"><span data-stu-id="5215f-134">Type</span></span> | <span data-ttu-id="5215f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5215f-135">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="5215f-136">changeType</span><span class="sxs-lookup"><span data-stu-id="5215f-136">changeType</span></span> | <span data-ttu-id="5215f-137">строка</span><span class="sxs-lookup"><span data-stu-id="5215f-137">string</span></span> | <span data-ttu-id="5215f-138">Указывает тип изменения в ресурсе, на который оформлена подписка и при возникновении которого будет создано уведомление.</span><span class="sxs-lookup"><span data-stu-id="5215f-138">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="5215f-139">Поддерживаемые значения: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="5215f-139">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="5215f-140">Вы можете объединить несколько значений, указав их в списке с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="5215f-140">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="5215f-141">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5215f-141">Required.</span></span> <br><br><span data-ttu-id="5215f-142">Примечание. Уведомления о корневых элементах диска поддерживают только `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="5215f-142">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="5215f-143">Уведомления о пользователе и группе поддерживают `updated` и `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="5215f-143">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="5215f-144">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="5215f-144">notificationUrl</span></span> | <span data-ttu-id="5215f-145">строка</span><span class="sxs-lookup"><span data-stu-id="5215f-145">string</span></span> | <span data-ttu-id="5215f-146">URL-адрес конечной точки, принимающей уведомления.</span><span class="sxs-lookup"><span data-stu-id="5215f-146">The URL of the endpoint that receives the notifications.</span></span> <span data-ttu-id="5215f-147">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="5215f-147">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="5215f-148">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5215f-148">Required.</span></span> |
| <span data-ttu-id="5215f-149">лифецикленотификатионурл</span><span class="sxs-lookup"><span data-stu-id="5215f-149">lifecycleNotificationUrl</span></span> | <span data-ttu-id="5215f-150">string</span><span class="sxs-lookup"><span data-stu-id="5215f-150">string</span></span> | <span data-ttu-id="5215f-151">URL-адрес конечной точки, которая получает уведомления жизненного `subscriptionRemoved` цикла `missed` , включая и уведомления.</span><span class="sxs-lookup"><span data-stu-id="5215f-151">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="5215f-152">Если этот параметр не указан, уведомления будут доставляться в **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="5215f-152">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="5215f-153">Этот URL-адрес должен использовать протокол HTTPS.</span><span class="sxs-lookup"><span data-stu-id="5215f-153">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="5215f-154">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5215f-154">Optional.</span></span> <br><br><span data-ttu-id="5215f-155">[Узнайте больше](/graph/webhooks-outlook-authz) о том, как ресурсы Outlook используют Уведомления жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="5215f-155">[Read more](/graph/webhooks-outlook-authz) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="5215f-156">resource</span><span class="sxs-lookup"><span data-stu-id="5215f-156">resource</span></span> | <span data-ttu-id="5215f-157">string</span><span class="sxs-lookup"><span data-stu-id="5215f-157">string</span></span> | <span data-ttu-id="5215f-158">Указывает ресурс, для которого будут отслеживаться изменения.</span><span class="sxs-lookup"><span data-stu-id="5215f-158">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="5215f-159">Не включайте базовый URL-адрес (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="5215f-159">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="5215f-160">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5215f-160">Required.</span></span> |
| <span data-ttu-id="5215f-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5215f-161">expirationDateTime</span></span> | <span data-ttu-id="5215f-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5215f-162">DateTimeOffset</span></span> | <span data-ttu-id="5215f-163">Указывает дату и время истечения срока действия подписки на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="5215f-163">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="5215f-164">Используется время в формате UTC, и оно может представлять собой время с момента создания подписки, которое зависит от ресурса, на который оформлена подписка.</span><span class="sxs-lookup"><span data-stu-id="5215f-164">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="5215f-165">В приведенной ниже таблице указан максимально допустимый период подписки.</span><span class="sxs-lookup"><span data-stu-id="5215f-165">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="5215f-166">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5215f-166">Required.</span></span> |
| <span data-ttu-id="5215f-167">clientState</span><span class="sxs-lookup"><span data-stu-id="5215f-167">clientState</span></span> | <span data-ttu-id="5215f-168">string</span><span class="sxs-lookup"><span data-stu-id="5215f-168">string</span></span> | <span data-ttu-id="5215f-169">Задает значение свойства **clientState** , которое отправляется службой в каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="5215f-169">Specifies the value of the **clientState** property sent by the service in each notification.</span></span> <span data-ttu-id="5215f-170">Максимальная длина: 255 символов.</span><span class="sxs-lookup"><span data-stu-id="5215f-170">The maximum length is 255 characters.</span></span> <span data-ttu-id="5215f-171">Клиент может проверить, что уведомление поступило из службы, сравнив значение свойства **clientState** , отправленного с подпиской, со значением свойства **clientState** , полученного при каждом уведомлении.</span><span class="sxs-lookup"><span data-stu-id="5215f-171">The client can check that the notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each notification.</span></span> <span data-ttu-id="5215f-172">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5215f-172">Optional.</span></span> |
| <span data-ttu-id="5215f-173">id</span><span class="sxs-lookup"><span data-stu-id="5215f-173">id</span></span> | <span data-ttu-id="5215f-174">string</span><span class="sxs-lookup"><span data-stu-id="5215f-174">string</span></span> | <span data-ttu-id="5215f-p110">Уникальный идентификатор для подписки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5215f-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="5215f-177">applicationId</span><span class="sxs-lookup"><span data-stu-id="5215f-177">applicationId</span></span> | <span data-ttu-id="5215f-178">string</span><span class="sxs-lookup"><span data-stu-id="5215f-178">string</span></span> | <span data-ttu-id="5215f-179">Идентификатор приложения, использованного для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="5215f-179">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="5215f-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5215f-180">Read-only.</span></span> |
| <span data-ttu-id="5215f-181">creatorId</span><span class="sxs-lookup"><span data-stu-id="5215f-181">creatorId</span></span> | <span data-ttu-id="5215f-182">string</span><span class="sxs-lookup"><span data-stu-id="5215f-182">string</span></span> | <span data-ttu-id="5215f-183">Идентификатор пользователя или субъекта-службы, которые создали подписку.</span><span class="sxs-lookup"><span data-stu-id="5215f-183">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="5215f-184">Если приложение использовало делегированные разрешения для создания подписки, это поле содержит идентификатор пользователя, выполнившего вход в систему, вызываемую приложением от имени.</span><span class="sxs-lookup"><span data-stu-id="5215f-184">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="5215f-185">Если приложение использовало разрешения приложения, это поле содержит идентификатор участника службы, соответствующего приложению.</span><span class="sxs-lookup"><span data-stu-id="5215f-185">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="5215f-186">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5215f-186">Read-only.</span></span> |
| <span data-ttu-id="5215f-187">инклудересаурцедата</span><span class="sxs-lookup"><span data-stu-id="5215f-187">includeResourceData</span></span> | <span data-ttu-id="5215f-188">Логический</span><span class="sxs-lookup"><span data-stu-id="5215f-188">Boolean</span></span> | <span data-ttu-id="5215f-189">Если задано `true`значение, уведомления об изменении [включают данные ресурса](/graph/webhooks-with-resource-data) (например, содержимое сообщения чата).</span><span class="sxs-lookup"><span data-stu-id="5215f-189">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="5215f-190">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5215f-190">Optional.</span></span> | 
| <span data-ttu-id="5215f-191">енкриптионцертификате</span><span class="sxs-lookup"><span data-stu-id="5215f-191">encryptionCertificate</span></span> | <span data-ttu-id="5215f-192">string</span><span class="sxs-lookup"><span data-stu-id="5215f-192">string</span></span> | <span data-ttu-id="5215f-193">Представление сертификата с кодировкой base64 с открытым ключом, используемым для шифрования данных ресурсов в уведомлениях.</span><span class="sxs-lookup"><span data-stu-id="5215f-193">A base64-encoded representation of a certificate with a public key used to encrypt resource data in notifications.</span></span> <span data-ttu-id="5215f-194">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5215f-194">Optional.</span></span> <span data-ttu-id="5215f-195">Является обязательным, если **инклудересаурцедата** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="5215f-195">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="5215f-196">енкриптионцертификатеид</span><span class="sxs-lookup"><span data-stu-id="5215f-196">encryptionCertificateId</span></span> | <span data-ttu-id="5215f-197">string</span><span class="sxs-lookup"><span data-stu-id="5215f-197">string</span></span> | <span data-ttu-id="5215f-198">Настраиваемый идентификатор, предоставляемый приложением, для определения сертификата, необходимого для расшифровки данных ресурса.</span><span class="sxs-lookup"><span data-stu-id="5215f-198">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="5215f-199">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5215f-199">Optional.</span></span> <span data-ttu-id="5215f-200">Является обязательным, если **инклудересаурцедата** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="5215f-200">Required when **includeResourceData** is true.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="5215f-201">Максимальный период подписки для каждого из типов ресурсов</span><span class="sxs-lookup"><span data-stu-id="5215f-201">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="5215f-202">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5215f-202">Resource</span></span>            | <span data-ttu-id="5215f-203">Максимальное время истечения срока действия</span><span class="sxs-lookup"><span data-stu-id="5215f-203">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="5215f-204">**Оповещение** безопасности</span><span class="sxs-lookup"><span data-stu-id="5215f-204">Security **alert**</span></span>     | <span data-ttu-id="5215f-205">43200 минут (до 30 дней)</span><span class="sxs-lookup"><span data-stu-id="5215f-205">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="5215f-206">**ChatMessage** Teams</span><span class="sxs-lookup"><span data-stu-id="5215f-206">Teams **chatMessage**</span></span>    | <span data-ttu-id="5215f-207">60 минут (1 час)</span><span class="sxs-lookup"><span data-stu-id="5215f-207">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="5215f-208">Групповая **беседа**</span><span class="sxs-lookup"><span data-stu-id="5215f-208">Group **conversation**</span></span> | <span data-ttu-id="5215f-209">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="5215f-209">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="5215f-210">OneDrive для **driveItem**</span><span class="sxs-lookup"><span data-stu-id="5215f-210">OneDrive **driveItem**</span></span>    | <span data-ttu-id="5215f-211">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="5215f-211">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="5215f-212">**Сообщение**Outlook, **событие**, **контакт**</span><span class="sxs-lookup"><span data-stu-id="5215f-212">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="5215f-213">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="5215f-213">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="5215f-214">**Пользователи**, **группы**и другие ресурсы каталога</span><span class="sxs-lookup"><span data-stu-id="5215f-214">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="5215f-215">4230 минут (до 3 дней)</span><span class="sxs-lookup"><span data-stu-id="5215f-215">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="5215f-216">**Примечание.** Для существующих приложений и новых приложений не должно превышаться допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="5215f-216">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="5215f-217">В будущем любые запросы на создание или продление подписки со значением, превышающим максимальное, будут завершаться ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5215f-217">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="5215f-218">Отношения</span><span class="sxs-lookup"><span data-stu-id="5215f-218">Relationships</span></span>

<span data-ttu-id="5215f-219">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5215f-219">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5215f-220">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5215f-220">JSON representation</span></span>

<span data-ttu-id="5215f-221">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5215f-221">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string",
  "includeResourceData": "boolean",
  "encryptionCertificate": "string",
  "encryptionCertificateId": "string"
}
```

[contact]: ./contact.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
[chatMessage]: ./chatmessage.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
