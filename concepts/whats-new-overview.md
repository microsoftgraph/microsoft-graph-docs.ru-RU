---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 0742ac1f35e10cfbed09ca164d4cb2af6a1c8484
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229369"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Полный список обновлений API см. в разделах [Апрель](changelog.md#april-2020) и [Март](changelog.md#march-2020) журнала изменений API. 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="april-2020-new-and-generally-available"></a>Апрель 2020 г.: новые и общедоступные возможности

### <a name="calendar"></a>Календарь
- [Делитесь календарями или делегируйте их](outlook-share-or-delegate-calendar.md) программным способом, соответствующим пользовательскому интерфейсу Outlook. Поддерживается отслеживание разрешений текущего пользователя и состояния общего доступа к календарю, а также следующие возможности:
  - Для каждого [календаря](/graph/api/resources/calendar?view=graph-rest-1.0) теперь можно управлять [разрешениями](/graph/api/resources/calendarpermission?view=graph-rest-1.0) каждого пользователя, которому предоставлен доступ к календарю. 
  - Для каждого [почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-1.0) теперь можно указать, кто получает сообщения о собраниях и ответы на эти сообщения: делегат, владелец почтового ящика или и тот, и другой. 
- [Создание или обновление события в виде собрания по сети](outlook-calendar-online-meetings.md):
  - В каждом **календаре** можно указать разрешенных и используемых по умолчанию поставщиков собраний по сети.
  - Можно создать или обновить [мероприятие](/graph/api/resources/event?view=graph-rest-1.0), доступное по сети, и предоставить участникам сведения для присоединения к собранию по сети. 
  - В частности, можно использовать **onlineMeetingProvider** и **onlineMeeting** — это новые свойства **мероприятий**, с помощью которых можно задать или указать Microsoft Teams в качестве поставщика собраний по сети. Это временное решение [известной проблемы](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) со свойством **onlineMeetingUrl**.

## <a name="april-2020-new-in-preview-only"></a>Апрель 2020 г.: новые возможности только в предварительной версии

### <a name="identity-and-access"></a>Удостоверение и доступ
Чтобы управлять ролями и назначать доступ к ресурсам в провайдерах управления доступом на основе ролей (RBAC), таких как Microsoft Intune, используйте [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-beta). Ресурс **unifiedRoleAssignmentMultiple** поддерживает определение одной роли в массиве областей и назначение роли для нескольких субъектов (например, пользователей). 


## <a name="march-2020-new-and-generally-available"></a>Март 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Облачные коммуникации
- Получите функцию маршрутизации вызовов и контекст входящих [вызовов](/graph/api/resources/call?view=graph-rest-1.0).
- [Обновите состояние записи](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0) звонка.
- Укажите информацию о записи для [участника](/graph/api/resources/participant?view=graph-rest-1.0), включая инициатора и состояние записи.
- Для уникальной идентификации участников конференции или [звонка](/graph/api/resources/call?view=graph-rest-1.0) от участника к участнику используйте свойство **callChainId**.
- Определите как часть [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0) код страны и тип конечной точки (например, Skype для бизнеса или Skype для бизнеса VoIP) участника.
- Сторонние партнеры в области устройств видеоконференцсвязи (VTC) могут регистрировать и предоставлять сведения о качестве связи для своих устройств через бот Cloud Video Interop (CVI) с помощью функции [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0). Качество связи определяется данными открытого типа о [звуке](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-1.0), [видео](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-1.0) и [демонстрации экрана](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-1.0).

### <a name="files"></a>Файлы
- [Удаленные элементы](/graph/api/resources/remoteitem?view=graph-rest-1.0), к которым пользователю предоставлен общий доступ, добавленные в хранилище OneDrive пользователя или возвращенные как результаты поиска, могут содержать метаданные для изображения или видео.
- [Отслеживайте](/graph/api/driveitem-follow?view=graph-rest-1.0) объект [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) для удобного доступа или упрощения таких действий, как перемещение, копирование и сохранение в определенном формате. Используйте [отмену отслеживания](/graph/api/driveitem-unfollow?view=graph-rest-1.0), чтобы прекратить отслеживание элемента диска.
- [Предоставьте](/graph/api/permission-grant?view=graph-rest-1.0) пользователям разрешение на доступ к ссылке для общего доступа, чтобы поделиться соответствующим элементом диска.

### <a name="identity-and-access"></a>Удостоверение и доступ
- [Отслеживайте изменения](/graph/api/orgcontact-delta?view=graph-rest-1.0) в [контактах организации](/graph/api/resources/orgcontact?view=graph-rest-1.0).
- Используйте свойство **riskEventTypes_v2**, чтобы получить типы событий риска, связанные с [входом](/graph/api/resources/signin?view=graph-rest-1.0).
- Используйте делегированное разрешение `User.ManageIdentities.All`, чтобы разрешить приложению считывать, обновлять и удалять удостоверения, связанные с учетной записью пользователя, к которой имеет доступ зарегистрированный пользователь. Используйте это разрешение на уровне приложения без зарегистрированного пользователя. Это позволяет приложению [определить](/graph/api/user-update?view=graph-rest-1.0), с помощью каких удостоверений пользователь может войти.

### <a name="reports"></a>Отчеты
Используйте Администратор службы Teams и Администратор связи Teams в качестве принятых ролей пользователя, чтобы приложения могли читать отчеты об использовании службы Office 365 от имени пользователя в качестве [форм делегированной пользователем авторизации](reportroot-authorization.md). 

### <a name="sites"></a>Сайты
- Предоставляйте пользователям возможность [отслеживать](/graph/api/site-follow?view=graph-rest-1.0) или [прекращать отслеживание](/graph/api/site-unfollow?view=graph-rest-1.0) сайтов SharePoint. 
- [Подпишитесь на уведомления об изменениях](/graph/api/resources/subscription?view=graph-rest-1.0) в [списке](/graph/api/resources/list?view=graph-rest-1.0) SharePoint.

## <a name="march-2020-new-in-preview-only"></a>Март 2020: Новое только в превью

### <a name="calendar"></a>Календарь
- Используйте свойство **calendarGroupId**, чтобы получить группу [календаря](/graph/api/resources/calendargroup?view=graph-rest-beta), в которой создан [календарь](/graph/api/resources/calendar?view=graph-rest-beta).
- Используйте свойство **в черновике**, чтобы идентифицировать [событие](/graph/api/resources/event?view=graph-rest-beta) как собрание, которое пользователь обновил в Outlook, но не отправил для обновления участников.

### <a name="cloud-communications"></a>Облачные коммуникации
- Используйте [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta), чтобы получить экземпляр [онлайн-собрания](/graph/api/resources/onlinemeeting?view=graph-rest-beta) с помощью внешнего настраиваемого идентификатора или создать его, если он еще не существует.
- Вы можете использовать свойство **externalId**, чтобы определить онлайн-собрание с помощью внешнего настраиваемого идентификатора.
- Используйте необязательный заголовок HTTP-запроса `Accept-Language`, чтобы [создать](/graph/api/application-post-onlinemeetings?view=graph-rest-beta) или [получить](/graph/api/onlinemeeting-get?view=graph-rest-beta) экземпляр онлайн-собрания. При успешном выполнении операции отображается содержимое свойства **joinInformation** на указанном языке и вариант локали.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [март](changelog.md#march-2020).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте разрешение `Auditlogs.Read.All` для списка [действий входа](/graph/api/resources/signinactivity?view=graph-rest-beta) [пользователя](/graph/api/resources/user?view=graph-rest-beta).
- Используйте разрешение на уровне приложения `PrivilegedAccess.Read.AzureResources` для [управления привилегированными удостоверениями (PIM) ресурсов Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta), чтобы настроить рабочий процесс доступа «точно в срок» для ролей инфраструктуры Azure на уровне группы управления, подписки, группы ресурсов или ресурса.
- Используйте объект [identitySecurityDefaultsEnforcementPolicy](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta), чтобы [получить](/graph/api/identitysecuritydefaultsenforcementpolicy-get?view=graph-rest-beta) или [обновить](/graph/api/identitysecuritydefaultsenforcementpolicy-update?view=graph-rest-beta) предварительно настроенные параметры безопасности по умолчанию, которые защищают организации от распространенных атак.
- Используйте сегмент `identity` при вызове API условного доступа. Например, чтобы [получить](/graph/api/conditionalaccesspolicy-get?view=graph-rest-beta) [политику условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta): `GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}`.
- Используйте свойство **authenticationRequirement**, чтобы получить наивысший уровень проверки подлинности, необходимый для успешного выполнения всех действий [входа](/graph/api/resources/signin?view=graph-rest-beta).
- Используйте разбивку на страницы при [перечислении событий подготовки](/graph/api/provisioningobjectsummary-list?view=graph-rest-beta) в вашем клиенте.

### <a name="search"></a>Поиск
- Чтобы добавить данные в файле к результатам поиска, просто индексируйте данные как [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta). Тип **externalFile** не рекомендуется.
- [Обновите](/graph/api/externalitem-update?view=graph-rest-beta) [элемент в индексе](/graph/api/resources/externalitem?view=graph-rest-beta), обновив представление элемента в виде обычного текста (представленное свойством **content**) или контейнер свойств элемента (представленный свойством **properties**). При обновлении любого свойства в контейнере свойств перезаписывается весь контейнер свойств, поэтому убедитесь, что все свойства элемента явным образом включены в обновление.
- Проверьте наличие `HTTP 429` и заголовка ответа `Retry-After` после вызова операции [создания](/graph/api/externalconnection-put-items?view=graph-rest-beta), [обновления](/graph/api/externalitem-update?view=graph-rest-beta) или [удаления](/graph/api/externalitem-delete?view=graph-rest-beta) элемента **externalItem**. Самый быстрый способ выполнить восстановление после [регулирования](throttling.md#best-practices-to-handle-throttling) — отложить запросы с помощью задержки `Retry-After`.

### <a name="teamwork"></a>Командная работа
Используйте разрешение на уровне приложения `ChannelMessage.Read.All` для чтения экземпляров [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) в каналах без зарегистрированного пользователя.

### <a name="universal-print"></a>Универсальная печать
Появление [API универсальной печати](universal-print-concept-overview.md), позволяющего пользователям печатать в Интернете или из приложения. API позволяет ИТ-администраторам управлять доступом пользователей и групп к принтерам в облаке Microsoft 365, а также удаленным общим доступом к принтерам для поддерживания доступности, отслеживать состояние принтеров и создавать отчеты о заархивированных заданиях печати и использовании. 

Обратите внимание, что с марта 2020 г. _служба_ универсальной печати доступна в закрытой предварительной версии. Дополнительные сведения об участии см. в статье [Представляем универсальную печать: облачное решение для печати](https://aka.ms/announcinguniversalprint).


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

