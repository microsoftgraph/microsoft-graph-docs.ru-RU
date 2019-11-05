---
title: Обзор предыдущих выпусков Microsoft Graph
description: Новые возможности в предыдущих выпусках Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 9cb240474a6df6344c6c4b4ad66f099ff354deb8
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37968491"
---
# <a name="highlights-of-earlier-releases"></a>Обзор предыдущих выпусков

## <a name="september-2019-new-and-generally-available"></a>Сентябрь 2019 г.: новые и общедоступные возможности

### <a name="calendar-mail-and-group"></a>Календарь, почта и группа
[Получение необработанного содержимого файла или содержимого MIME элемента](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment), добавленного в качестве [вложения](/graph/api/resources/attachment?view=graph-rest-1.0) в [событие](/graph/api/resources/event?view=graph-rest-1.0), [сообщение](/graph/api/resources/message?view=graph-rest-1.0) или [запись](/graph/api/resources/post?view=graph-rest-1.0) группы.

### <a name="calendar-mail-outlook-task-personal-contact"></a>Календарь, почта, задача Outlook, личный контакт
Преобразование идентификатора элемента Outlook в поддерживаемые [форматы](/graph/api/user-translateexchangeids?view=graph-rest-1.0#exchangeidformat-values), включая стандартный и неизменяемый формат идентификаторов Microsoft Graph, с помощью функции [translateExchangeId](/graph/api/user-translateexchangeids?view=graph-rest-1.0). 

Преобразование формата идентификатора поддерживают следующие ресурсы:

- [attachment](/graph/api/resources/attachment?view=graph-rest-1.0)
- [contact](/graph/api/resources/contact?view=graph-rest-1.0)
- [event](/graph/api/resources/event?view=graph-rest-1.0)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0)
- [message](/graph/api/resources/message?view=graph-rest-1.0)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0)

### <a name="mail"></a>Почта
[Получение содержимого MIME сообщения](outlook-get-mime-message.md)

### <a name="microsoft-graph-toolkit"></a>Набор средств Microsoft Graph
Использование [набора средств Microsoft Graph](toolkit/overview.md) с целью разработки приложений для рабочей среды, обеспечивающих согласованный внешний вид и функции Microsoft 365, и экономии времени при проверке подлинности и доступе к данным из Microsoft Graph.

## <a name="september-2019-new-in-preview"></a>Сентябрь 2019 г.: новые возможности в предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [сентябрь](changelog.md#september-2019)

### <a name="files"></a>Файлы
- Улучшенная поддержка синхронизации:

  - Определение операций, которые могут влиять на двоичное содержимое объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta), с помощью нового свойства **pendingOperations**.
  - [Восстановление](/graph/api/driveitem-restore?view=graph-rest-beta) удаленного объекта **driveItem**. 
- Использование защищенного алгоритма хэширования (SHA-256) для улучшения безопасности и целостности данных ресурса [file](/graph/api/resources/file?view=graph-rest-beta).
- Получение или настройка ориентации ресурса [photo](/graph/api/resources/photo?view=graph-rest-beta). Настройка поддерживается в OneDrive персональный.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Использование нового свойства **identities** и получение удостоверений, которые может применять [пользователь](/graph/api/resources/user?view=graph-rest-beta) для входа в учетную запись. Удостоверения могут предоставляться организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт.
- Добавочные улучшения для [синхронизации удостоверений](/graph/api/resources/synchronization-overview?view=graph-rest-beta) в облачном приложении для клиента:

  - Сохранение параметров для [задания синхронизации](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)
  - Указание причины применения [карантина](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta) для задания синхронизации

### <a name="teamwork"></a>Командная работа
Использование канала **Общий** в [команде](/graph/api/resources/team?view=graph-rest-beta) или настройка [параметров участников](/graph/api/resources/teammembersettings?view=graph-rest-beta), чтобы разрешить участникам команд создавать закрытые каналы в **команде**.

### <a name="users"></a>Пользователи
- Получение или обновление удостоверений, с помощью которых [пользователь](/graph/api/resources/user?view=graph-rest-beta) может войти в учетную запись. Эти удостоверения могут предоставляться бизнес-организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт.
- Получение или обновление параметров предпочитаемого пользователем формата даты и времени [для почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-beta).


## <a name="august-2019-new-and-generally-available"></a>Август 2019 г.: новые и общедоступные возможности 

### <a name="reports"></a>Отчеты
- Получите дополнительные [данные об использовании почтового ящика](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0) касательно числа и размера удаленных элементов.
- Отслеживайте идентификаторы групп Office 365 при [получении сведений о действиях групп](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0).
- Отслеживайте имя субъекта-владельца при получении [сведений об использовании хранилища OneDrive учетной записью](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0) и [сведений об использовании сайта SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0).
- Узнайте число активных и неактивных пользователей в Office 365 при [получении отчета о количестве пользователей в отдельных службах Office 365](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0).

### <a name="security"></a>Безопасность
- Используйте новую [надстройку Microsoft Graph Security API для Splunk](https://aka.ms/graphsecuritysplunkaddon), чтобы передавать оповещения системы безопасности и аналитику из различных продуктов партнеров в Splunk, облегчая сопоставление их данных по безопасности в режиме реального времени. Дополнительные сведения см. в [объявлении](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972). 
- [Ознакомьтесь со списком других решений и соединителей](security-integration.md), разработанных корпорацией Майкрософт или партнерами Майкрософт, которые подключаются к API безопасности и позволяют работать с данными в едином формате.


## <a name="august-2019-new-in-preview"></a>Август 2019 г.: новые возможности предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [август](changelog.md#august-2019)

### <a name="education"></a>Образование
- Свяжите [преподавателя](/graph/api/resources/educationuser?view=graph-rest-beta) или [задание](/graph/api/resources/educationassignment?view=graph-rest-beta) с [рубрикой оценивания](/graph/api/resources/educationrubric?view=graph-rest-beta), чтобы задать определенные показатели качества и уровни заданий. К примерам показателей качеств относятся орфография и грамматика, а к примерам уровней — "хорошо" и "неудовлетворительно". Кроме того, вы можете связать с рубрикой баллы и веса. Дополнительные сведения см. в [обзоре образовательных рубрик](education-rubric-overview.md).
- Оцените задание и представьте результаты в виде [отзыва](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta), [числовой оценки](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta) или [рубрики](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta).

### <a name="files"></a>Файлы
До этого момента вы могли [отслеживать](/graph/api/driveitem-follow?view=graph-rest-beta) объект [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) для удобного доступа или упрощения таких действий, как перемещение, копирование и сохранение в определенном формате. Теперь вы можете использовать действие [отмены отслеживания](/graph/api/driveitem-unfollow?view=graph-rest-beta), чтобы прекратить отслеживание таких элементов диска.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Поставщики управления доступом на основе ролей (RBAC) могут [управлять ролями](/graph/api/resources/rolemanagement?view=graph-rest-beta) в Azure Active Directory, [определяя действия ролей](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta), которые могут выполняться с определенными ресурсами, и [назначая роли](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta) пользователям в соответствии с этими определениями, чтобы предоставить им доступ к этим ресурсам.
- Администраторы могут [просматривать обзоры доступа](/graph/api/accessreview-list?view=graph-rest-beta), чтобы эффективно проверять членство в группах, доступ к корпоративным приложениям и назначения ролей. Регулярные проверки доступа позволяют гарантировать, что только уполномоченные люди получают постоянный доступ к ресурсам определенными способами.

### <a name="social-and-workplace-intelligence"></a>Социальная и рабочая аналитика
Пользователи могли использовать приложение [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights-preview) Office 365 для получения аналитических сведений о распределении рабочего времени, совместной работе и балансе между трудовой и личной жизнью. Теперь с помощью [API аналитики](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-gain-insights-into-their-work-patterns) можно интегрировать данные о времени, потраченном на рабочие задачи (например, звонки, чаты и электронную почту), чтобы повысить продуктивность пользователя и улучшить его самочувствие. 


## <a name="july-2019-new-and-generally-available"></a>Июль 2019 г.: новые и общедоступные возможности 

### <a name="example-code-snippets"></a>Примеры фрагментов кода
Теперь имеются фрагменты кода Objective-C для всех статей по API в справочных материалах для версии 1.0 и бета-версии. См. пример Objective-C для [получения события](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example).

### <a name="group"></a>Группа
- Используйте функцию [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0), чтобы отображаемое имя или почтовый псевдоним существующей группы Office 365 соответствовали политикам именования.
- Кроме того, перед созданием группы вы можете использовать функцию [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0) для объекта [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), чтобы сначала проверить имена.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-1.0) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-1.0).
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#role-management-permissions) _RoleManagement.Read.Directory_ и _RoleManagement.ReadWrite.Directory_ для управления доступом на основе ролей (RBAC) в каталоге компании:

  - Используйте разрешение на чтение и запись, чтобы сначала [активировать](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0) роль каталога. 
  - Если роль активирована, вы можете использовать разрешение на чтение для [чтения ролей каталога](/graph/api/directoryrole-list?view=graph-rest-1.0), [перечисления участников ролей](/graph/api/directoryrole-list-members?view=graph-rest-1.0) и [перечисления шаблонов для ролей каталогов](/graph/api/directoryroletemplate-list?view=graph-rest-1.0). 
  - Вы также можете использовать разрешение на чтение и запись для [добавления](/graph/api/directoryrole-post-members?view=graph-rest-1.0) и [удаления](/graph/api/directoryrole-delete-member?view=graph-rest-1.0) участников ролей.


## <a name="july-2019-new-in-preview"></a>Июль 2019 г.: новые возможности предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="calendar"></a>Календарь 
Используйте новый [API мест](/graph/api/resources/place?view=graph-rest-beta), чтобы применять различные типы расположений, например [помещения](/graph/api/resources/room?view=graph-rest-beta) и [список помещений](/graph/api/resources/roomlist?view=graph-rest-beta), настроенные администраторами Exchange Online.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [июль](changelog.md#july-2019)

### <a name="files"></a>Файлы 
Применяйте дату и время окончания срока действия или пароль при [создании ссылки для общего доступа](/graph/api/driveitem-createlink?view=graph-rest-beta) к файлу, папке или другому объекту [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте [новое разрешение приложений](/graph/permissions-reference?#accessreviews-permissions) _AccessReview.ReadWrite.Membership_ для операций CRUD при [проверках доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta). 
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#administrative-units-permissions) _AdministrativeUnit.Read.All_ и _AdministrativeUnit.ReadWrite.All_ для чтения и записи (включая создание, обновление и удаление участников, а также управление ими) ресурсов [административных единиц](/graph/api/resources/administrativeunit?view=graph-rest-beta) соответственно.
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-beta) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-beta).
- Используйте новую функцию [обнаружения](/graph/api/directorydefinition-discover?view=graph-rest-beta) для поиска последней [схемы синхронизации](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta) каталога, чтобы синхронизировать объекты каталога, атрибуты и их типы с приложением.
- Используйте [политику развертывания функций](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta), чтобы помочь администраторам клиента выполнить пилотное развертывание функций для определенных групп перед включением их для всей организации.

### <a name="mail"></a>Почта
Используйте более детализированное разрешение приложений _Mail.ReadBasic.All_, чтобы читать почтовый ящик пользователя, кроме текста сообщений, текста предварительного просмотра, вложений и расширенных свойств, а также без возможности поиска в почтовом ящике. Теперь его можно применять в [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) и [отслеживании изменений](delta-query-overview.md) для [сообщения](/graph/api/resources/message?view=graph-rest-beta) и объекта **mailFolder**.

### <a name="reports"></a>Отчеты
- Получите дополнительные [данные об использовании почтового ящика](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta) касательно числа и размера удаленных элементов.

### <a name="teamwork"></a>Командная работа
- [Устанавливайте](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta), [удаляйте](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta), [обновляйте](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta) и [перечисляйте установленные приложения Microsoft Teams](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta) для пользователя.
- Используйте доступ только для приложения, чтобы читать сообщения канала, а также отвечать на сообщения в каналах и беседах. [Запросите и получите утверждение](teams-protected-apis.md) для такого доступа.

## <a name="may---june-2019-new-and-generally-available"></a>Май–июнь 2019 г.: новые и общедоступные возможности

### <a name="calendar-mail-and-personal-contacts"></a>Календарь, почта и личные контакты
Администраторы Exchange могут предоставлять приложению разрешения приложения и [ограничить доступ приложения только к подмножеству почтовых ящиков](auth-limit-mailbox-access.md) вместо доступа ко всем почтовым ящикам в организации, используемого по умолчанию. Такое ограничение доступа будет применено ко всем разрешениям приложения, предоставленным приложению для [календарей](permissions-reference.md#calendars-permissions), [контактов](permissions-reference.md#contacts-permissions), а также [параметров почты и почтового ящика](permissions-reference.md#mail-permissions). См. связанное [объявление в блоге](https://developer.microsoft.com/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/).

### <a name="mail"></a>Почта
Используйте API [папок поиска почты](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) для поиска сообщений и доступа к результатам поиска по электронной почте Outlook. См. связанное [объявление в блоге](https://developer.microsoft.com/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/).

### <a name="postman"></a>Postman
В качестве альтернативы песочнице Graph используйте API Microsoft Graph в [коллекции Postman Microsoft Graph](use-postman.md), чтобы изучить поведение API и ускорить разработку приложения.

### <a name="tutorials"></a>Учебники
Воспользуйтесь новым [руководством для создания консольного приложения Java](/graph/tutorials/java), чтобы получить информацию о календаре пользователя.

### <a name="user"></a>Пользователь
Администраторы и пользователи могут [отзывать](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) все выданные маркеры обновления для пользователя. Обычно это используется для того, чтобы запретить доступ к данным организации для приложений на потерянных и украденных устройствах.


## <a name="may---june-2019-new-in-preview"></a>Май–июнь 2019 г.: новые возможности в предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
- Обновления Intune за [май](changelog.md#may-2019) 
- Обновления Intune за [июнь](changelog.md#june-2019)

### <a name="education"></a>Образование
- Разностный запрос для [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta).
- Разностный запрос и добавления свойств для [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) и [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta).

### <a name="group"></a>Группа
Получите [метки конфиденциальности](/graph/api/resources/assignedlabel?view=graph-rest-beta), чтобы обеспечить защиту конфиденциальных данных группы Office 365 и выполнение политик в отношении соответствия требованиям. Эти метки являются объектами [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta), опубликованными администраторами в Центре безопасности и соответствия требованиям Microsoft 365, в рамках возможностей Microsoft Information Protection. 

### <a name="identity-and-access"></a>Удостоверения и доступ
- Получите экземпляр [приложения](/graph/api/resources/applicationtemplate?view=graph-rest-beta) или добавьте экземпляр из коллекции приложений Azure AD в ваш каталог в качестве шаблона.
- Получите журнал всех [событий подготовки](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta) каталога в клиенте.
- Получите сведения об [обнаруженном пользователе или рисках входа в систему](/graph/api/resources/riskdetection?view=graph-rest-beta) в среде Azure AD. Эта функциональность обнаружения рисков является частью Azure AD Identity Protection (Защиты идентификации Azure AD).

### <a name="mail"></a>Почта
Используйте более детализированное делегированное разрешение _Mail.ReadBasic_, чтобы читать почтовый ящик пользователя, кроме текста сообщений, текста предварительного просмотра, вложений и расширенных свойств, а также без возможности поиска в почтовом ящике. Доступно для методов чтения [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) и [отслеживания изменений](delta-query-overview.md) для [сообщения](/graph/api/resources/message?view=graph-rest-beta) и объекта **mailFolder**.

### <a name="microsoft-graph-toolkit"></a>Набор средств Microsoft Graph
[Набор средств Microsoft Graph](/graph/toolkit/overview) — это набор не зависящих от платформы веб-компонентов и помощников, обеспечивающий удобную проверку подлинности и доступ к данным в Microsoft Graph.  Так как набор средств Microsoft Graph находится в состоянии предварительной версии, используйте компоненты и поставщиков наборов средств только для тех приложений, которые не предназначены для рабочей среды.

### <a name="reports"></a>Отчеты
- Получайте [отчеты о методах проверки подлинности](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta), используемых пользователями в организации, таких как самостоятельное хранение пароля и многофакторная проверка подлинности (MFA).

### <a name="sites"></a>Сайты
Предоставляйте пользователям возможность [отслеживать](/graph/api/site-follow?view=graph-rest-beta) или [прекращать отслеживание](/graph/api/site-unfollow?view=graph-rest-beta) сайтов SharePoint. 

### <a name="teamwork"></a>Командная работа
- Размещайте [изображения](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta) в [сообщениях в чатах](/graph/api/resources/chatmessage?view=graph-rest-beta) Microsoft Teams.
- Поддерживайте [настройку](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta) способа обнаружения закрытой команды.


## <a name="january---april-2019-new-and-generally-available"></a>Январь–апрель 2019 г.: новые и общедоступные возможности

[Подключение к данным Microsoft Graph](data-connect-concept-overview.md)

### <a name="calendar"></a>Календарь
[Получение сведений о доступности](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>Удостоверения и доступ
[Поставщики удостоверений](/graph/api/resources/identityprovider?view=graph-rest-1.0)
[Руководство по улучшенной проверке подлинности](/graph/auth)
[Миграция приложений из Azure AD Graph в Microsoft Graph](migrate-azure-ad-graph-overview.md)

### <a name="sdks"></a>Пакеты SDK
[Руководство по пакетам SDK](/sdks/sdks-overview.md) Фрагменты API ([пример](/graph/api/user-get?view=graph-rest-1.0&tabs=cs#sdk-sample-code))

### <a name="security"></a>Система безопасности
[Оценка безопасности клиента](/graph/api/resources/securescore?view=graph-rest-1.0)

## <a name="january---april-2019-new-in-preview"></a>Январь–апрель 2019 г.: новые возможности в предварительной версии

### <a name="calendar-group-mail-to-do-tasks"></a>Календарь, группа, почта, задачи To-Do
[Получение необработанного контента или содержимого MIME вложений](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment) для события, сообщения, задачи Outlook или записи в группе

### <a name="change-notifications"></a>Уведомления об изменениях
[Уменьшение числа пропущенных уведомлений об изменениях для ресурсов Outlook](webhooks-outlook-authz.md)

### <a name="devices-and-apps"></a>Устройства и приложения
- Обновления Intune за [январь](changelog.md#january-2019) 
- Обновления Intune за [февраль](changelog.md#february-2019)
- Обновления Intune за [март](changelog.md#march-2019)
- Обновления Intune за [апрель](changelog.md#april-2019)

### <a name="files"></a>Файлы
[Приглашение к совместному использованию](/graph/api/driveitem-invite?view=graph-rest-beta) включает истечение срока его действия и пароль

### <a name="financials"></a>Финансовые показатели
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>Удостоверения и доступ
[Проверки доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta) поддерживают разрешения для приложений [Журналы аудита и входа](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta)
[Настраиваемые вход и регистрация в Azure AD B2C](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta)
[Рискованный пользователь](/graph/api/resources/riskyuser?view=graph-rest-beta) и [журнал](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta)

### <a name="mail"></a>Почта
[Получение содержимого MIME сообщений](outlook-get-mime-message.md)

### <a name="reports"></a>Отчеты
[Отчеты о входе в приложение](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta)

### <a name="security"></a>Система безопасности
[Действия по обеспечению безопасности](/graph/api/resources/securityaction?view=graph-rest-beta)
[Индикаторы угроз](/graph/api/resources/tiindicator?view=graph-rest-beta)

### <a name="teamwork"></a>Командная работа
[Личные чаты](/graph/api/resources/chat?view=graph-rest-beta)
[Управление сменами](/graph/api/resources/shift?view=graph-rest-beta)

## <a name="see-also"></a>См. также
- Ознакомьтесь [с текущими новыми возможностями](whats-new-overview.md) в Microsoft Graph.
- Периодически просматривайте [блог разработчика, посвященный Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).