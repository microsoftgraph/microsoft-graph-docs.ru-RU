---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: ebe9baf44acb273513bb8047740880ec04c205e5
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892767"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Полный список обновлений API см. в разделе [Март](changelog.md#march-2020) и [Февраль](changelog.md#february-2020) журнала изменений API. 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="march-2020-new-and-generally-available"></a>Март 2020: новый и общедоступный

### <a name="identity-and-access"></a>Удостоверение и доступ
Используйте делегированное разрешение `User.ManageIdentities.All`, чтобы разрешить приложению считывать, обновлять и удалять удостоверения, связанные с учетной записью пользователя, к которой имеет доступ зарегистрированный пользователь. Используйте это разрешение на уровне приложения без зарегистрированного пользователя. Это позволяет приложению [определить](/graph/api/user-update?view=graph-rest-1.0), с помощью каких удостоверений пользователь может войти.

### <a name="reports"></a>Отчеты
Используйте Администратор службы Teams и Администратор связи Teams в качестве принятых ролей пользователя, чтобы приложения могли читать отчеты об использовании службы Office 365 от имени пользователя в качестве [форм делегированной пользователем авторизации](reportroot-authorization.md). 

## <a name="march-2020-new-in-preview-only"></a>Март 2020: Новое только в превью

### <a name="calendar"></a>Календарь
- Используйте свойство **calendarGroupId**, чтобы получить группу [календаря](/graph/api/resources/calendargroup?view=graph-rest-beta), в которой создан [календарь](/graph/api/resources/calendar?view=graph-rest-beta).
- Используйте свойство **в черновике**, чтобы идентифицировать [событие](/graph/api/resources/event?view=graph-rest-beta) как собрание, которое пользователь обновил в Outlook, но не отправил для обновления участников.

### <a name="cloud-communications"></a>Облачные коммуникации
- Сторонние партнеры в области устройств видеоконференцсвязи (VTC) могут регистрировать и предоставлять сведения о качестве связи для своих устройств через бот Cloud Video Interop (CVI) с помощью функции [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-beta). Качество связи определяется данными открытого типа о [звуке](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-beta), [видео](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-beta) и [демонстрации экрана](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-beta).
- Для уникальной идентификации участников конференции или [звонка](/graph/api/resources/call?view=graph-rest-beta) от участника к участнику используйте свойство **callChainId**.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [март](changelog.md#march-2020).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте разрешение `Auditlogs.Read.All` для списка [действий входа](/graph/api/resources/signinactivity?view=graph-rest-beta) [пользователя](/graph/api/resources/user?view=graph-rest-beta).
- Используйте разрешение на уровне приложения `PrivilegedAccess.Read.AzureResources` для [управления привилегированными удостоверениями (PIM) ресурсов Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta), чтобы настроить рабочий процесс доступа «точно в срок» для ролей инфраструктуры Azure на уровне группы управления, подписки, группы ресурсов или ресурса.

### <a name="search"></a>Поиск
- Чтобы добавить данные в файле к результатам поиска, просто индексируйте данные как [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta). Тип **externalFile** не рекомендуется.
- Теперь вы можете [обновить](/graph/api/externalitem-update?view=graph-rest-beta) [элемент в индексе](/graph/api/resources/externalitem?view=graph-rest-beta), обновив представление элемента в виде обычного текста (представленное свойством **content**) или контейнер свойств элемента (представленный свойством **properties**). При обновлении любого свойства в контейнере свойств перезаписывается весь контейнер свойств, поэтому убедитесь, что все свойства элемента явным образом включены в обновление.
- Проверьте наличие `HTTP 429` и заголовка ответа `Retry-After` после вызова операции [создания](/graph/api/externalconnection-put-items?view=graph-rest-beta), [обновления](/graph/api/externalitem-update?view=graph-rest-beta) или [удаления](/graph/api/externalitem-delete?view=graph-rest-beta) элемента **externalItem**. Самый быстрый способ выполнить восстановление после [регулирования](throttling.md#best-practices-to-handle-throttling) — отложить запросы с помощью задержки `Retry-After`.

### <a name="teamwork"></a>Командная работа
Используйте разрешение на уровне приложения `ChannelMessage.Read.All` для чтения экземпляров [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) в каналах без зарегистрированного пользователя.

## <a name="february-2020-new-and-generally-available"></a>2020 февраля: новая и общедоступная

### <a name="calendar"></a>Календарь
Просмотрите пример [создания события в общем или делегированном календаре](outlook-create-event-in-shared-delegated-calendar.md), а также действия и свойства, доступные для делегата, приглашенных и владельца календаря во время этого процесса.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Чтобы повысить безопасность при подписке на [уведомления об изменениях пользовательских данных](webhooks.md), [установите Transport Layer Security (TLS) 1.2](https://docs.microsoft.com/configmgr/core/plan-design/security/enable-tls-1-2) или выше на клиентах и серверах сайтов, используемых в процессе уведомления. Новое требование вводится поэтапно, начиная с 15 февраля 2020 года. К 15 мая 2020 года все конечные точки уведомления должны соответствовать новому требованию TLS. [Узнайте о стадиях развертывания](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) и при необходимости воспользуйтесь новым свойством **latestSupportedTlsVersion** в качестве временного решения, чтобы избежать сбоев подписки до выполнения обновления TLS.
- Используйте соответствующие типы [запроса оценки угроз](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0) для отслеживания угроз от [почты](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0), [файла сообщения электронной почты](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0) (. EML-файл), [файлов вложений электронной почты](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0) (текстовых файлов, файлов Word и двоичных файлов) и [URL-адреса](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0).

### <a name="users"></a>Пользователи
[Повторная обработка](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0) всех назначений лицензий на основе группы для [пользователя](/graph/api/resources/user?view=graph-rest-1.0).


## <a name="february-2020-new-in-preview-only"></a>Февраль 2020: новое только в предварительном просмотре

### <a name="calendar"></a>Календарь
Просмотрите [задачи, поддерживаемые API-интерфейсами предварительного просмотра, которые управляют совместным использованием и делегированием календаря](outlook-share-or-delegate-calendar.md).

### <a name="cloud-communications"></a>Коммуникации из облака

- Используйте новую [запись вызова ](/graph/api/resources/callrecord?view=graph-rest-beta) ресурс, чтобы получить метаданные звонков и собрания по сети в Microsoft Teams и Skype для бизнеса в Организации.
- Для участника собрания используйте свойство **инициатора**, чтобы получить идентификационную информацию инициатора [записи](/graph/api/resources/recordinginfo?view=graph-rest-beta), если таковая имеется.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [Февраль](changelog.md#february-2020)

### <a name="groups"></a>Группы
Используйте метод [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta), чтобы назначить лицензии для продуктов, таких как Office 365 или Enterprise Mobility + Security, группе. Поскольку Azure AD обеспечивает назначение лицензий членам группы, для участников, вступающих в группу или покидающих ее, больше не требуется управление лицензиями на индивидуальном уровне.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Установите параметры запроса, утверждения и проверки при создании [политики назначения пакетов доступа](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta).
- Получите доступ к определенным типам [политик для организации](/graph/api/resources/policy-overview?view=graph-rest-beta), используя `/policies`сегмент URL и указав тип политики. Например, организация может применить политику для автоматического выхода пользователя из веб-сеанса после периода бездействия; см. операции CRUD для экземпляров [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta). Это [серьезное изменение](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/), упрощающее обнаружение всех политик путем группировки всех типизированных политик в сегменте `/policies`. Доступ к другим типизированным политикам осуществляется аналогичным образом: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta) и [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta). 
- Используйте уровень приложения и делегированное `Policy.ReadWrite.ApplicationConfiguration`разрешение для операций чтения и записи в [политиках](/graph/api/resources/policy-overview?view=graph-rest-beta) конфигурации приложений, упомянутых в предыдущем пункте.

### <a name="teamwork"></a>Командная работа
- Используйте [уведомления об изменениях,](/graph/api/resources/webhooks?view=graph-rest-beta) всех сообщений канала или всех сообщений в Организации.
- [Отклоните](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta) [запрос на замену смен](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta) другим пользователем в [группе](/graph/api/resources/team?view=graph-rest-beta).

## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Office 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Office 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).

