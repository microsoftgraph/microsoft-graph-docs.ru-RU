---
title: Подписка на уведомления об изменениях из API облачной печати с использованием Microsoft Graph
description: Узнайте, как подписаться на уведомления об изменениях событий печати с помощью API Microsoft Graph.
author: jahsu
ms.localizationpriority: high
ms.prod: cloud-printing
ms.custom: scenarios:getting-started
ms.openlocfilehash: df511878bfebba02bd68ede445a26b66233caeae
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143462"
---
# <a name="subscribe-to-change-notifications-from-cloud-printing-apis-using-microsoft-graph"></a>Подписка на уведомления об изменениях из API облачной печати с использованием Microsoft Graph

Универсальная печать помогает пользователям переносить инфраструктуру печати в облако и является частью надежной экосистемы партнерских решений, предлагающих расширенные возможности печати. Эти решения могут быть еще эффективнее, если использовать API облачной печати в Microsoft Graph для интеграции с универсальной печатью.

Многие партнерские решения должны обрабатывать задания печати в режиме реального времени при их отправке с устройств пользователей на принтеры. Это означает, что они должны получать уведомления, когда задания печати доступны для обработки. Универсальная печать предоставляет обработчики для уведомления решений поставщиков печати, когда задания перемещаются в облаке, а также API, позволяющие управлять принтерами и заданиями печати.

В этой статье объясняется, как подписаться на уведомления о различных событиях заданий печати.


## <a name="get-started-with-change-notifications"></a>Начало работы с уведомлениями об изменениях

Чтобы использовать уведомления об изменениях посредством Microsoft Graph, вы должны [зарегистрировать свое приложение в Azure](/azure/active-directory/develop/howto-create-service-principal-portal#register-an-application-with-azure-ad-and-create-a-service-principal) и подготовить приложение в клиенте Azure Active Directory (Azure AD) пользователей. Включите требуемые области разрешений для приложения, как описано далее в этой статье.


### <a name="notifications-and-subscriptions"></a>Уведомления и подписки

В настоящее время универсальная печать поддерживает уведомления для двух сценариев, связанных с заданиями печати.

* Инициирована задача PrintTask (JobStarted): приложение может подписаться на получение уведомлений при инициировании printTask(hook).
Дополнительные сведения о том, как инициировать задачу, см. в разделе [Расширение универсальной печати для поддержки печати по запросу](./universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing). В настоящее задачу printTask можно инициировать только для события JobStarted. Событие JobStarted возникает, когда создано задание печати, загружены его полезные данные и запущена обработка задания.  

* JobFetchable: после запуска задания сторонние приложения печати или универсальная печать могут выполнять некоторую обработку (например, преобразовать полезные данные XPS в формат PDF для принтера PDF). После завершения обработки и готовности полезных данных к загрузке принтером возникает событие JobFetchable для соответствующего задания печати.

>[!NOTE]
>Чтобы прослушивать уведомления об изменениях для события JobFetchable, не требуется ресурс **printTaskDefinition**.

### <a name="create-an-application-to-listen-to-notifications"></a>Создание приложения для прослушивания уведомлений

Сведения о том, как прослушивать уведомления Microsoft Graph, см. в разделах [Использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph](/learn/modules/msgraph-changenotifications-trackchanges/) и [Настройка уведомлений об изменениях пользовательских данных — примеры кода](./webhooks.md#code-samples).


### <a name="scopes"></a>Области

Чтобы подписаться на уведомления о заданиях печати, для приложений должны быть утверждены следующие области разрешений в клиенте Azure AD пользователя. 

* Для инициированного события printTask (JobStarted) разрешения перечислены в статье [Получение taskDefinition](/graph/api/printtaskdefinition-get?view=graph-rest-v1.0&tabs=http%22%20%5Cl%20%22permissions%22%20%5C). 

* Для события JobFetchable разрешения перечислены в статье [Создание подписки](/graph/api/subscription-post-subscriptions?view=graph-rest-v1.0&tabs=http).

Приложения должны [создавать и использовать маркер безопасности Azure AD](/graph/auth-v2-service?context=graph%2Fapi%2F1.0) в заголовке запроса API Microsoft Graph. Маркер безопасности содержит утверждения согласно областям, одобренным администратором для клиента Azure AD.  


## <a name="create-subscription-printtask-triggered-jobstarted-event"></a>Создание подписки: инициировано событие printTask (JobStarted) 

Некоторые приложения отслеживают очереди печати для входящих заданий и хотят получать уведомления сразу при появлении действительного задания в очереди. После уведомления они могут собирать соответствующие метаданные задания или даже вносить изменения в задание печати, включая отмену задания или его перенаправление из текущей очереди печати в другую очередь после соответствующего изменения атрибутов задания. 

Перед созданием уведомления для инициированного события **printTask**, убедитесь, что приложение создало следующие элементы: 

- [printTaskDefinition](/graph/api/print-post-taskdefinitions?view=graph-rest-v1.0&tabs=http)  для клиента Azure AD пользователя. Одно определение задачи можно связать с одним или несколькими принтерами в одном клиенте Azure AD. 

- [printTaskTrigger](/graph/api/printer-post-tasktriggers?view=graph-rest-v1.0&tabs=http) для всех очередей принтеров, для которых партнер хочет получать уведомление при запуске нового задания печати. **printTaskTrigger** требуется связать с **printTaskDefinition**. 

>[!NOTE]
>Один принтер можно связать только с одним объектом **printTaskTrigger**, а один объект **printTaskTrigger** можно связать только с одним элементом **printTaskDefinition**. Однако один элемент **printTaskDefinition** можно связать с несколькими объектами **printTaskTriggers**. 

С помощью элемента **printTaskDefinition**, существующего для клиента Azure AD пользователя, приложение может [создать подписку на инициированное событие printTask (JobStarted) с помощью printTaskDefinition](/graph/api/subscription-post-subscriptions?view=graph-rest-v1.0&tabs=http). При создании подписки:  

* Полю `resource` требуется присвоить значение `print/taskDefinitions/{printTaskDefinition ID}/tasks`. 
* Полю `changeType` требуется присвоить значение `created`. 
* Поле `expirationDateTime` не должное превышать [максимальный срок действия](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type). 

Дополнительные сведения см. в разделе [Свойства типа ресурса subscription](/graph/api/resources/subscription?view=graph-rest-v1.0#properties).

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/v1.0/subscriptions 
Content-Type: application/json
{ 
    "changeType":"created", 
    "resource":"print/taskDefinitions/{printTaskDefinition ID}/tasks", 
    "clientState":"secret", 
    "notificationUrl":"{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "expirationDateTime":"2020-01-30T22:42:09Z" 
} 
```

### <a name="response"></a>Отклик

Ниже показан пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity", 
    "id": "{Subscription ID}", 
    "resource": "print/taskDefinitions/{printTaskDefinition ID}/tasks", 
    "applicationId": "{application ID}", 
    "changeType": "created", 
    "clientState": "secret", 
    "notificationUrl": "{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "notificationQueryOptions": null, 
    "lifecycleNotificationUrl": null, 
    "expirationDateTime": "2020-12-30T22:42:09Z", 
    "creatorId": "{Creator ID}", 
    "includeResourceData": null, 
    "latestSupportedTlsVersion": "v1_2", 
    "encryptionCertificate": null, 
    "encryptionCertificateId": null 
}
```


## <a name="create-subscription-jobfetchable-event"></a>Создание подписки: событие JobFetchable 
Некоторым облачным приложениям требуется скачивать задания печати из универсальной печати, когда они будут готовы. Так как такие приложения, работающие в облаке, находятся вне границ брандмауэра пользователя, они могут использовать уведомления об изменениях Microsoft Graph, чтобы узнавать о готовности заданий печати к скачиванию.

>[!NOTE]
>Задания печати нельзя изменить после их перехода в состояние JobFetchable.
Уведомление JobFetchable требуется создавать для каждой очереди принтера. При создании подписки:
* Полю `resource` требуется присвоить значение "print/printers/{printer id}/jobs". 
* Полю `changeType` требуется присвоить значение `updated`. 
* Полю `notificationQueryOptions` требуется присвоить значение `$filter = isFetchable eq true`. 
* Поле `expirationDateTime` не должное превышать [максимальный срок действия](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type). 

Дополнительные сведения см. в разделе [Свойства типа ресурса subscription](/graph/api/resources/subscription?view=graph-rest-v1.0#properties).

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
    "changeType":"updated",
    "resource":"print/printers/{printer id}/jobs",
    "notificationQueryOptions": "$filter = isFetchable eq true", 
    "notificationUrl":"{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}",
    "expirationDateTime":"2020-12-30T22:42:09Z",
    "clientState":"mysecret"
} 
```

### <a name="response"></a>Отклик

Ниже показан пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity", 
    "id": "{Subscription ID}", 
    "resource": "print/printers/{printer ID}/jobs", 
    "applicationId": "{Application ID}", 
    "changeType": "updated", 
    "clientState": "mysecret", 
    "notificationUrl": "{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "notificationQueryOptions": "$filter = isFetchable eq true", 
    "lifecycleNotificationUrl": null, 
    "expirationDateTime": "2020-12-30T22:42:09Z", 
    "creatorId": "{Creator ID}", 
    "includeResourceData": null, 
    "latestSupportedTlsVersion": "v1_2", 
    "encryptionCertificate": null, 
    "encryptionCertificateId": null
}
```


## <a name="renewing-a-notification-subscription"></a>Возобновление подписки на уведомления

В Microsoft Graph срок действия ограничен. Дополнительные сведения см. в разделе о [максимальном сроке действия](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type). Чтобы продолжать получать уведомления, подписку требуется периодически обновлять с помощью [API обновления подписки](/graph/api/subscription-update?view=graph-rest-v1.0&tabs=http). 

## <a name="other-operations-on-notification-subscriptions"></a>Другие операции с подпиской на уведомления 

Приложения могут [получать](/graph/api/subscription-get?view=graph-rest-v1.0&tabs=http) сведения о подписке или [удалять](/graph/api/subscription-delete?view=graph-rest-v1.0&tabs=http) подписку при необходимости. Подробности см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](/graph/api/resources/webhooks?view=graph-rest-v1.0).


## <a name="faqs"></a>Вопросы и ответы
### <a name="how-does-microsoft-graph-validate-notification-urls"></a>Как Microsoft Graph проверяет URL-адреса уведомлений?
Прежде чем создать подписку, Microsoft Graph проверяет конечную точку уведомлений в свойстве **notificationUrl** запроса подписки.
Подробности см. в разделе [Проверка конечной точки уведомлений](./webhooks.md#notification-endpoint-validation).

### <a name="what-are-applications-expected-to-do-after-receiving-a-change-notification"></a>Каковы предполагаемые действия приложений после получения уведомления об изменении?
Приложения должны обрабатывать и подтверждать каждое полученное уведомление об изменении. Подробности см. в разделе [Обработка уведомлений об изменениях](./webhooks.md#processing-the-change-notification).

### <a name="how-can-i-get-a-list-of-active-subscriptions"></a>Как получить список активных подписок?
Сведения о том, как получить список подписок на веб-перехватчики, см. в разделе [Перечисление подписок](/graph/api/subscription-list?view=graph-rest-v1.0&tabs=http).


## <a name="see-also"></a>См. также

- Дополнительные сведения об API облачной печати в Microsoft Graph см. в статье [Обзор API облачной среды универсальной печати](/graph/universal-print-concept-overview). 
- Чтобы отправить предложения и отзывы об API облачной печати в Microsoft Graph, перейдите в [техническое сообщество универсальной печати](https://aka.ms/community/UniversalPrint).
