---
title: Тип ресурса group
description: 'Представляет группу Azure Active Directory (Azure AD), которая может быть группой Microsoft 365 или группой безопасности. '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 027f3df4ef061d4b620d9eaa177327d2edce9140
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944207"
---
# <a name="group-resource-type"></a>Тип ресурса group

Пространство имен: microsoft.graph

Представляет группу Azure Active Directory (Azure AD), которая может быть группой Microsoft 365 или группой безопасности.

Наследуется от [directoryObject](directoryobject.md).

Чтобы повысить производительность, операции [create](../api/group-post-groups.md), [get](../api/group-get.md) и [list](../api/group-list.md) возвращают только подмножество часто используемых свойств по умолчанию. Эти свойства _по умолчанию_ указаны в разделе [Свойства](#properties). Чтобы получить любые свойства, которые не возвращаются по умолчанию, укажите их в параметре запроса OData `$select`.

Этот ресурс поддерживает:

- добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);
- подписку на [уведомления об изменениях](/graph/webhooks);
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/user-delta.md)).


## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:------ |:----------- |:----------- |
| **Управление группами** |||
| [Создание группы](../api/group-post-groups.md) | [group](group.md) | Создание группы. Это может быть группа Microsoft 365, группа безопасности или динамическая группа. |
| [Получение группы](../api/group-get.md) | [group](group.md) | Считывание свойств объекта group. |
| [Список групп](../api/group-list.md) | Коллекция [group](group.md) | Список объектов group и их свойств. |
| [Обновление группы](../api/group-update.md) | Нет | Обновление свойств объекта group. |
| [Удаление группы](../api/group-delete.md) | Нет | Удаление объекта group. |
| [delta](../api/group-delta.md) | Коллекция group | Получение добавочных изменений для групп. |
| [Добавление члена](../api/group-post-members.md) | Нет | Добавление пользователя или группы в данную группу путем помещения в свойство навигации **members** (поддерживается только для групп безопасности, в том числе с включенной поддержкой почты). |
| [Добавление владельца](../api/group-post-owners.md) | Нет | Добавление владельца группы путем помещения в свойство навигации **owners** (поддерживается только для групп безопасности, в том числе с включенной поддержкой почты). |
| [Создание параметра](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) | Создание параметра объекта на базе groupSettingTemplate. POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне. В случае этой операции могут использоваться только шаблоны специально для групп. |
| [Удаление параметра](../api/groupsetting-delete.md) | Нет | Удаление объекта setting. |
| [Получение параметра](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Считывание свойств определенного объекта setting. |
| [Перечисление groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md)  | Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md) | Перечисление политик жизненного цикла для групп. |
| [Перечисление участников](../api/group-list-members.md) | Коллекция [directoryObject](directoryobject.md) | Получение пользователей и групп, являющихся непосредственными участниками этой группы, из свойства навигации **members**. |
| [Список владельцев](../api/group-list-owners.md) | Коллекция [directoryObject](directoryobject.md) | Получение владельцев группы из свойства навигации **owners**. |
| [Перечисление параметров](../api/groupsetting-list.md) | Коллекция объектов [groupSetting](groupsetting.md) | Перечисление свойств всех объектов setting. |
| [Перечисление транзитивных участников](../api/group-list-transitivemembers.md) | Коллекция [directoryObject](directoryobject.md) | Получение пользователей, групп и устройств, являющихся участниками, включая вложенных участников этой группы. |
| [Перечисление транзитивных свойств memberOf](../api/group-list-transitivememberof.md) | Коллекция [directoryObject](directoryobject.md) | Перечисление групп, в которых состоит эта группа. Эта операция является транзитивной и включает группы, в которых эта группа является вложенным элементом. |
| [Удаление участника](../api/group-delete-members.md) | Нет | Удаление участника из группы Microsoft 365 или группы безопасности (в том числе с включенной поддержкой почты) с помощью свойства навигации **members**. Вы можете удалять пользователей или другие группы. |
| [Удаление владельца](../api/group-delete-owners.md) | Нет | Удаление владельца из группы Microsoft 365 или группы безопасности (в том числе с включенной поддержкой почты) с помощью свойства навигации **owners**. |
| [Обновление параметра](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Обновление объекта setting. |
| [assignLicense](../api/group-assignlicense.md) | [group](group.md) | Добавление или удаление подписок группы. Вы также можете включать и отключать отдельные планы, связанные с подпиской. |
| [checkMemberGroups](../api/group-checkmembergroups.md) | Коллекция String | Проверка данной группы на членство в списке групп. Это транзитивная функция. |
| [checkMemberObjects](../api/group-checkmemberobjects.md) | Коллекция String | Проверка участия в списке группы, роли каталога или объектах административных единиц. Это транзитивная функция. |
| [getMemberGroups](../api/group-getmembergroups.md) | Коллекция String | Возврат всех групп, в которых состоит эта группа. Это транзитивная функция. |
| [getMemberObjects](../api/group-getmemberobjects.md) | Коллекция String | Возврат всех групп, в которых состоит эта группа. Это транзитивная функция. |
| [renew](../api/group-renew.md) | Boolean | Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой. |
| [validateProperties](../api/group-validateproperties.md) | JSON | Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования. |
| **Назначение ролей приложений** |||
| [Перечисление appRoleAssignments](../api/group-list-approleassignments.md) | Коллекция [appRoleAssignment](approleassignment.md) | Получение приложений и ролей приложений, назначенных группе. |
| [Добавление объекта appRoleAssignment](../api/group-post-approleassignments.md) | [appRoleAssignment](approleassignment.md) | Назначение роли приложения группе. |
| [Удаление объекта appRoleAssignment](../api/group-delete-approleassignments.md) | Нет. | Удаление назначения роли приложения из группы. |
| **Calendar** |||
| [Создание события](../api/group-post-events.md) | [event](event.md) | Создание объекта event путем публикации в коллекции объектов event. |
| [Получение события](../api/group-get-event.md) | [event](event.md) | Считывание свойств объекта event. |
| [Перечисление событий](../api/group-list-events.md) | Коллекция [event](event.md) | Получение коллекции объектов event. |
| [Обновление события](../api/group-update-event.md) | Нет | Обновление свойств объекта event. |
| [Удаление события](../api/group-delete-event.md) | Нет | Удаление объекта event. |
| [Список calendarView](../api/group-list-calendarview.md) | Коллекция [event](event.md) | Получение коллекции событий за указанный интервал времени.|
| **Беседы** |||
| [Создание беседы](../api/group-post-conversations.md) | [conversation](conversation.md) | Создание беседы путем публикации в коллекции объектов conversation. |
| [Получение беседы](../api/group-get-conversation.md) | [conversation](conversation.md) | Считывание свойств объекта conversation. |
| [Перечисление бесед](../api/group-list-conversations.md) | Коллекция [conversation](conversation.md) | Получение коллекции объектов conversation. |
| [Удаление беседы](../api/group-delete-conversation.md) | Нет | Удаление объекта conversation. |
| [Создание цепочки](../api/group-post-threads.md) | [conversationThread](conversationthread.md) | Создание цепочки беседы. |
| [Получение цепочки](../api/group-get-thread.md) | [conversationThread](conversationthread.md) | Считывание свойств объекта thread. |
| [Перечисление цепочек](../api/group-list-threads.md) | Коллекция [conversationThread](conversationthread.md) | Получение всех цепочек группы. |
| [Обновление цепочки](../api/group-update-thread.md) | Нет | Обновление свойств объекта thread. |
| [Удаление цепочки](../api/group-delete-thread.md) | Нет | Удаление объекта thread. |
| [Вывод acceptedSenders](../api/group-list-acceptedsenders.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка пользователей или групп, включенных в список утвержденных отправителей для этой группы. |
| [Добавление acceptedSender](../api/group-post-acceptedsenders.md) | [directoryObject](directoryobject.md) | Добавление User или Group в коллекцию acceptedSenders. |
| [Удаление acceptedSender](../api/group-delete-acceptedsenders.md) | [directoryObject](directoryobject.md) | Удаление User или Group из коллекции acceptedSenders. |
| [Список rejectedSenders](../api/group-list-rejectedsenders.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка пользователей или групп, включенных в список запрещенных отправителей для этой группы. |
| [Добавление rejectedSender](../api/group-post-rejectedsenders.md)  | [directoryObject](directoryobject.md) | Добавление User или Group в коллекцию rejectedSenders. |
| [Удаление rejectedSender](../api/group-delete-rejectedsenders.md) | [directoryObject](directoryobject.md) | Удаление нового объекта User или Group из коллекции объектов rejectedSender. |
| [Создание параметра](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) | Создание параметра объекта на базе groupSettingTemplate. POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне. В случае этой операции могут использоваться только шаблоны специально для групп. |
| [Получение параметра](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Считывание свойств определенного объекта setting. |
| [Перечисление параметров](../api/groupsetting-list.md) | Коллекция объектов [groupSetting](groupsetting.md) | Перечисление свойств всех объектов setting. |
| [Обновление параметра](../api/groupsetting-update.md) | Нет | Обновление объекта параметра. |
| [Удаление параметра](../api/groupsetting-delete.md) | Нет | Удаление объекта параметра. |
| [Получение шаблона параметров](../api/groupsettingtemplate-get.md) | Нет | Чтение свойств шаблона параметров. |
| [Перечисление шаблонов параметров](../api/groupsettingtemplate-list.md) | Нет | Перечисление свойств всех шаблонов параметров. |
| **Открытые расширения** |||
| [Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) | Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс. |
| [Получение открытого расширения](../api/opentypeextension-get.md) | Коллекция объектов [openTypeExtension](opentypeextension.md) | Получение открытого расширения, определяемого именем расширения. |
| **Расширения схемы** |||
| [Добавление значений расширений для схемы](/graph/extensibility-schema-groups) | Нет | Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных. |
| **Другие ресурсы групп** |||
| [Перечисление фотографий](../api/group-list-photos.md) | Коллекция объектов [profilePhoto](photo.md) | Получение коллекции фотографий профиля для группы. |
| [Перечисление планов](../api/plannergroup-list-plans.md) | Коллекция объектов [plannerPlan](plannerplan.md) | Получение планов, принадлежащих группе. |
| **Параметры пользователя** |||
| [addFavorite](../api/group-addfavorite.md) | Нет | Добавление группы в список избранных групп вошедшего пользователя. Поддерживается только для групп Microsoft 365. |
| [removeFavorite](../api/group-removefavorite.md) | Нет | Удаление группы из списка избранных групп вошедшего пользователя. Поддерживается только для групп Microsoft 365. |
| [Перечисление memberOf](../api/group-list-memberof.md) | Коллекция [directoryObject](directoryobject.md) | Получение групп и административных единиц, непосредственным участником которых является пользователь, из свойства навигации **memberOf**. |
| [subscribeByMail](../api/group-subscribebymail.md) | Нет | Задает для свойства isSubscribedByMail значение `true`. Позволяет вошедшему пользователю получать беседы по электронной почте. Поддерживается только для групп Microsoft 365. |
| [unsubscribeByMail](../api/group-unsubscribebymail.md) | Нет | Задает для свойства isSubscribedByMail значение `false`. Отключает получение бесед по электронной почте для вошедшего пользователя. Поддерживается только для групп Microsoft 365. |
| [resetUnseenCount](../api/group-resetunseencount.md) | Нет | Сброс значений unseenCount до 0 для всех записей, которые вошедший пользователь не просматривал со времени последнего посещения. Поддерживается только для групп Microsoft 365. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowExternalSenders|Логический| Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу. Значение по умолчанию — `false`. <br><br>Возвращается только с помощью оператора `$select`. Поддерживается только для API получения группы (`GET /groups/{ID}`). |
|assignedLabels|Коллекция [assignedLabel](assignedlabel.md)|Список пар меток конфиденциальности (идентификатор метки, имя метки), связанных с группой Microsoft 365. <br><br>Возвращается только с помощью оператора `$select`. Только для чтения.|
|assignedLicenses|Коллекция [assignedLicense](assignedlicense.md)|Лицензии, назначенные группе. <br><br>Возвращается только с помощью оператора `$select`. Только для чтения.|
|autoSubscribeNewMembers|Логический|Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте. Это свойство можно задать в запросе PATCH для группы. Не задавайте его в первоначальном запросе POST, создающем группу. Значение по умолчанию — `false`. <br><br>Возвращается только с помощью оператора `$select`. Поддерживается только для API получения группы (`GET /groups/{ID}`).|
|classification|String|Описывает классификацию для группы (например, незначительное, среднее или значительное влияние на бизнес). Допустимые значения для этого свойства определяются созданием значения [setting](groupsetting.md) ClassificationList на базе [определения шаблона](groupsettingtemplate.md).<br><br>Возвращается по умолчанию.|
|createdDateTime|DateTimeOffset| Метка времени создания группы. Значение не может изменяться и заполняется автоматически, когда создается группа. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. <br><br>Возвращается по умолчанию. Только для чтения. |
|deletedDateTime|DateTimeOffset| При удалении некоторых объектов Azure Active Directory (пользователя, группы, приложения) сначала имеет место логическое удаление, а это свойство обновляется в соответствии с датой и временем удаления объекта. В противном случае это свойство имеет значение `null`. При восстановлении объекта это свойство обновляется до `null`. |
|description|String|Необязательное описание для группы. <br><br>Возвращается по умолчанию.|
|displayName|String|Отображаемое имя для группы. Это свойство необходимо при создании группы и не может быть удалено во время обновления. <br><br>Возвращается по умолчанию. Поддерживает `$filter` и `$orderby`. |
|expirationDateTime|DateTimeOffset| Метка времени завершения срока действия группы. Значение не может изменяться и заполняется автоматически, когда создается группа. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. <br><br>Возвращается по умолчанию. Только для чтения. |
|groupTypes|Коллекция String| Задает тип группы и участие в ней.  <br><br>Если коллекция содержит объект `Unified`, эта группа является группой Microsoft 365. В противном случае она является группой безопасности или группой рассылки. Дополнительные сведения см. в статье [Обзор групп](groups-overview.md).<br><br>Если коллекция включает объект `DynamicMembership`, в этой группе используется динамическое участие. В противном случае участие является статическим.  <br><br>Возвращается по умолчанию. Поддерживает `$filter`.|
|hasMembersWithLicenseErrors|Логический|Указывает, есть ли в этой группе участники с ошибками лицензий после группового назначения лицензий. <br><br>Это свойство никогда не возвращается при использовании операции GET. Его можно использовать в качестве аргумента $filter для получения групп, включающих участников с ошибками лицензии (т. е. фильтру для этого свойства присвоено значчение true). См. [пример](../api/group-list.md).|
|hideFromAddressLists |Логический |Значение true указывает, что группа не отображается в определенных частях пользовательского интерфейса Outlook: в **адресной книге**, в списках адресов для выбора получателей сообщений и в диалоговом окне **Обзор групп** для поиска групп. В противном случае используется значение false. Значение по умолчанию — `false`. <br><br>Возвращается только с помощью оператора `$select`. Поддерживается только для API получения группы (`GET /groups/{ID}`).|
|hideFromOutlookClients |Логический |Значение true указывает, что группа не отображается в клиентах Outlook, например Outlook для Windows и Outlook в Интернете. В противном случае используется значение false. Значение по умолчанию — `false`. <br><br>Возвращается только с помощью оператора `$select`. Поддерживается только для API получения группы (`GET /groups/{ID}`).|
|id|String|Уникальный идентификатор группы. <br><br>Возвращается по умолчанию. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
|isSubscribedByMail|Логический|Указывает, подписан ли вошедший пользователь на получение бесед по электронной почте. Значение по умолчанию — `true`. <br><br>Возвращается только с помощью оператора `$select`. Поддерживается только для API получения группы (`GET /groups/{ID}`). |
|licenseProcessingState|String|Указывает состояние назначения лицензии группы для всех участников группы. Значение по умолчанию — `false`. Только для чтения. Возможные значения: `QueuedForProcessing`, `ProcessingInProgress` и `ProcessingComplete`.<br><br>Возвращается только с помощью оператора `$select`. Только для чтения.|
|mail|String|SMTP-адрес группы, например "serviceadmins@contoso.onmicrosoft.com". <br><br>Возвращается по умолчанию. Только для чтения. Поддерживает `$filter`.|
|mailEnabled|Boolean|Указывает, включена ли для этой группы поддержка почты. <br><br>Возвращается по умолчанию.|
|membershipRule|String|Правило, определяющее участников этой группы, если группа является динамической (groupTypes содержит `DynamicMembership`). Дополнительные сведения о синтаксисе правила участия см. в [здесь](/azure/active-directory/users-groups-roles/groups-dynamic-membership). <br><br>Возвращается по умолчанию. |
|membershipRuleProcessingState|String|Указывает, включена или приостановлена динамическая обработка участия. Возможные значения: `On` или `Paused`. <br><br>Возвращается по умолчанию. |
|onPremisesSamAccountName|String|Содержит локальный параметр **SAM account name**, синхронизированный из локального каталога. Свойство заполняется только для клиентов, синхронизирующих свой локальный каталог с Azure Active Directory через Azure AD Connect.<br><br>Возвращается по умолчанию. Только для чтения. |
|onPremisesSecurityIdentifier|String|Содержит локальный идентификатор безопасности (SID) для локальной группы, синхронизированной с облаком. <br><br>Возвращается по умолчанию. Только для чтения. |
|onPremisesSyncEnabled|Boolean|Значение `true` указывает, что эта группа синхронизируется из локального каталога. Значение `false` указывает, что эта группа ранее синхронизировалась из локального каталога, но синхронизация больше не выполняется. Значение **null** указывает, что этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). <br><br>Возвращается по умолчанию. Только для чтения. Поддерживает `$filter`.|
|preferredDataLocation|String|Предпочитаемое расположение данных для группы. Дополнительные сведения см. в статье [OneDrive Online с поддержкой нескольких регионов](/sharepoint/dev/solution-guidance/multigeo-introduction). <br><br>Возвращается по умолчанию.|
|preferredLanguage|String|Предпочитаемый язык для группы Microsoft 365. Он должен быть представлен в формате ISO 639-1, например "ru-RU". <br><br>Возвращается по умолчанию. |
|proxyAddresses|Коллекция String| Адреса электронной почты для группы, ведущие в один почтовый ящик группы. Пример: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`. Для фильтрации выражений по многозначным свойствам требуется оператор **any**. <br><br>Возвращается по умолчанию. Только для чтения. Значение null не допускается. Поддерживает `$filter`. |
|renewedDateTime|DateTimeOffset| Метка времени последнего обновления группы. Не может изменяться непосредственно. Обновляется только при выполнении [действия обновления](../api/group-renew.md). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. <br><br>Возвращается по умолчанию. Только для чтения.|
|resourceBehaviorOptions|Коллекция объектов string|Определяет поведение группы, которое может быть задано для группы Microsoft 365 во время ее создания. Это можно сделать только в рамках операции создания (POST). Возможные значения: `AllowOnlyMembersToPost`, `HideGroupInOutlook`, `SubscribeNewGroupMembers`, `WelcomeEmailDisabled`. Дополнительные сведения см. в статье [Настройка вариантов поведения и подготовки групп Microsoft 365](/graph/group-set-options).|
|resourceProvisioningOptions|Коллекция объектов string|Определяет ресурсы группы, которые были подготовлены в рамках создания групп Microsoft 365 и обычно не являются частью процесса создания группы по умолчанию. Возможное значение: `Team`. Дополнительные сведения см. в статье [Настройка вариантов поведения и подготовки групп Microsoft 365](/graph/group-set-options).|
|securityEnabled|Логический|Указывает, является ли эта группа группой безопасности. <br><br>Возвращается по умолчанию. Поддерживает `$filter`.|
|securityIdentifier|String|Идентификатор безопасности группы, используемый в сценариях Windows. <br><br>Возвращается по умолчанию.|
|theme|String|Указывает цветовую тему группы Microsoft 365. Возможные значения: `Teal`, `Purple`, `Green`, `Blue`, `Pink`, `Orange` или `Red`. <br><br>Возвращается по умолчанию. |
|unseenCount|Int32|Количество бесед с новыми сообщениями, полученными с момента последнего посещения группы вошедшим в систему пользователем. <br><br>Возвращается только с помощью оператора `$select`. Поддерживается только для API получения группы (`GET /groups/{ID}`). |
|visibility|String| Указывает политику присоединения к группе и видимость содержимого для групп. Возможные значения: `Private`, `Public` или `Hiddenmembership`. `Hiddenmembership` задается только для Групп Microsoft 365 при их создании. Обновление невозможно выполнить позже. Другие значения видимости можно обновлять после создания группы.<br> Если при создании группы в Microsoft Graph не задается значение видимости, группа безопасности по умолчанию создается как `Private`, а группа Microsoft 365 —`Public`. Дополнительные сведения см. в разделе [Параметры видимости группы](#group-visibility-options). <br><br>Возвращается по умолчанию.|


### <a name="group-visibility-options"></a>Параметры видимости группы

|Значение|Описание|
|:----|-----------|
| Public | К группе может присоединиться любой пользователь без необходимости разрешения владельца.<br>Любой пользователь может просматривать содержимое группы.|
| Private | Чтобы присоединиться к группе, требуется разрешение владельца.<br>Пользователи, не являющиеся участниками группы, не могут просматривать ее содержимое.|
| Hiddenmembership | Чтобы присоединиться к группе, требуется разрешение владельца.<br>Пользователи, не являющиеся участниками группы, не могут просматривать ее содержимое.<br>Пользователи, не являющиеся участниками группы, не могут просматривать ее участников.<br>Администраторы (глобальные, организации, пользователей и службы поддержки) могут просматривать список участников группы.<br>Группа отображается в глобальной адресной книге (глобальном списке адресов).|


## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|acceptedSenders|Коллекция [directoryObject](directoryobject.md)|Список пользователей или групп, которым разрешено создавать записи или события календаря в этой группе. Если этот список не пуст, то добавлять записи разрешено только перечисленным в нем пользователям и группам.|
|appRoleAssignments|Коллекция [appRoleAssignment](approleassignment.md)|Представляет роли группе, предоставленные пользователю для приложения. |
|calendar|[calendar](calendar.md)|Календарь группы. Только для чтения.|
|calendarView|Коллекция [event](event.md)|Представление календаря. Только для чтения.|
|conversations|Коллекция [conversation](conversation.md)|Беседы группы.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Пользователь или приложение, создавшие группу. ПРИМЕЧАНИЕ. Это значение не задается, если пользователь является администратором. Только для чтения.|
|drive|[drive](drive.md)|Используемый по умолчанию диск группы. Только для чтения.|
|drives|Коллекция [drive](drive.md)|Диск группы. Только для чтения.|
|events|Коллекция [event](event.md)|События в календаре группы.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для группы. Только для чтения. Допускается значение null.|
|groupLifecyclePolicies|Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)|Коллекция политик жизненного цикла для этой группы. Только для чтения. Допускается значение null.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Группы, в которых состоит эта группа. Методы HTTP: GET (поддерживается для всех групп). Только для чтения. Допускается значение null.|
|members|Коллекция [directoryObject](directoryobject.md)| Пользователи и группы, состоящие в этой группе. Методы HTTP:GET (поддерживается для всех групп), POST (поддерживается для групп Microsoft 365 и групп безопасности, в том числе с включенной поддержкой почты), DELETE (поддерживается для групп Microsoft 365 и групп безопасности). Допускается значение null.|
|membersWithLicenseErrors|Коллекция [User](user.md)|Список участников группы с ошибками лицензий после группового назначения лицензий. Только для чтения.|
|onenote|[Onenote](onenote.md)| Только для чтения.|
|owners|Коллекция [directoryObject](directoryobject.md)|Владельцы группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект. Максимальное количество владельцев: 100. Методы HTTP:GET (поддерживается для всех групп), POST (поддерживается для групп Microsoft 365 и групп безопасности, в том числе с включенной поддержкой почты), DELETE (поддерживается для групп Microsoft 365 и групп безопасности). Допускается значение null.|
|permissionGrants|[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)|Разрешение, предоставленное группе для определенного приложения.|
|photo;|[profilePhoto](profilephoto.md)| Фотография профиля группы. |
|photos|Коллекция объектов [profilePhoto](profilephoto.md)| Фотографии профиля, принадлежащие группе. Только для чтения. Допускается значение null.|
|planner|[plannerGroup](plannergroup.md)| Точка входа в ресурс Planner, который может существовать для единой группы.|
|rejectedSenders|Коллекция [directoryObject](directoryobject.md)|Список пользователей или групп, которым запрещено создавать записи или события календаря в этой группе. Допускается значение null.|
|settings|Коллекция объектов [groupSetting](groupsetting.md)| Только для чтения. Допускается значение null.|
|sites|Коллекция объектов [site](site.md)|Список сайтов SharePoint в этой группе. Для доступа к сайту по умолчанию используйте путь /sites/root.|
|threads|Коллекция [conversationThread](conversationthread.md)| Цепочки бесед группы. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "drives",
    "events",
    "extensions",
    "groupLifecyclePolicies",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "photos",
    "planner",
    "rejectedSenders",
    "settings",
    "sites",
    "threads",

    "allowExternalSenders",
    "assignedLicenses",
    "autoSubscribeNewMembers",
    "hasMembersWithLicenseErrors",
    "isSubscribedByMail",
    "licenseProcessingState",
    "unseenCount"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "acceptedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "conversations",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "rejectedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "allowExternalSenders": false,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "autoSubscribeNewMembers": true,
  "classification": "string",
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "hasMembersWithLicenseErrors": "Boolean",
  "hideFromAddressLists": false,
  "hideFromOutlookClients": false,
  "id": "string (identifier)",
  "isSubscribedByMail": true,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "string",
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "resourceBehaviorOptions": ["String"],
  "resourceProvisioningOptions": ["String"],
  "securityEnabled": true,
  "securityIdentifier": "String",
  "unseenCount": 1024,
  "visibility": "string",
  "acceptedSenders": [ { "@odata.type": "microsoft.graph.directoryObject"} ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "conversations": [ { "@odata.type": "microsoft.graph.conversation" }],
  "createdOnBehalfOf": { "@odata.type": "microsoft.graph.directoryObject" },
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "events": [ { "@odata.type": "microsoft.graph.event" }],
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "members": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "membersWithLicenseErrors": [{"@odata.type": "microsoft.graph.user"}],
  "owners": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "rejectedSenders": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "sites": [ { "@odata.type": "microsoft.graph.site" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
