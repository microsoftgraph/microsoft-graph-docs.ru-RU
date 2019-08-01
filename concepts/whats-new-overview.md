---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 5a69232c58469f09e953af9e9d06667509a76568
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049619"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

Знаете ли вы, что некоторые новые возможности Microsoft Graph реализуются на основе распространенных запросов сообщества разработчиков? 

Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версий (`https://graph.microsoft.com/beta`). Возможности предварительной версии могут меняться без уведомления. Не используйте их в приложениях для рабочей среды. 

2. Повышение до **_общедоступного_ статуса (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). В приложениях для рабочей среды следует использовать только возможности со статусом GA.

Давайте рассмотрим, что нового в настоящее время в Microsoft Graph и как вы можете [поделиться своими идеями](#want-to-stay-in-the-loop). Подробные сведения об обновлениях API см. в разделах журнала изменений за [май](changelog.md#may-2019), [июнь](changelog.md#june-2019) и [июль](changelog.md#july-2019).  

## <a name="new-and-generally-available-released-may---july-2019"></a>Новые и общедоступные возможности (выпущенные с мая по июль 2019 г.)

### <a name="calendar-mail-and-personal-contacts"></a>Календарь, почта и личные контакты
Администраторы Exchange могут предоставлять приложению разрешения приложения и [ограничить доступ приложения только к подмножеству почтовых ящиков](auth-limit-mailbox-access.md) вместо доступа ко всем почтовым ящикам в организации, используемого по умолчанию. Такое ограничение доступа будет применено ко всем разрешениям приложения, предоставленным приложению для [календарей](permissions-reference.md#calendars-permissions), [контактов](permissions-reference.md#contacts-permissions), а также [параметров почты и почтового ящика](permissions-reference.md#mail-permissions). См. связанное [объявление в блоге](https://developer.microsoft.com/en-us/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/).

### <a name="example-code-snippets"></a>Примеры фрагментов кода
В дополнение к C# и JavaScript, теперь имеются фрагменты кода Objective-C для всех разделов API в материалах для версий v1.0 и бета. См. пример Objective-C для [получения события](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example).

### <a name="group"></a>Группа
- Используйте функцию [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0), чтобы отображаемое имя или почтовый псевдоним существующей группы Office 365 соответствовали политикам именования.
- Кроме того, перед созданием группы вы можете использовать функцию [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0) для объекта [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), чтобы сначала проверить имена.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-1.0) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-1.0).
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#role-management-permissions) _RoleManagement.Read.Directory_ и _RoleManagement.ReadWrite.Directory_ для управления доступом на основе ролей (RBAC) в каталоге компании:

  - Используйте разрешение на чтение и запись, чтобы сначала [активировать](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0) роль каталога. 
  - Если роль активирована, вы можете использовать разрешение на чтение для [чтения ролей каталога](/graph/api/directoryrole-list?view=graph-rest-1.0), [перечисления участников ролей](/graph/api/directoryrole-list-members?view=graph-rest-1.0) и [перечисления шаблонов для ролей каталогов](/graph/api/directoryroletemplate-list?view=graph-rest-1.0). 
  - Вы также можете использовать разрешение на чтение и запись для [добавления](/graph/api/directoryrole-post-members?view=graph-rest-1.0) и [удаления](/graph/api/directoryrole-delete-member?view=graph-rest-1.0) участников ролей. 

### <a name="mail"></a>Почта
Используйте API [папок поиска почты](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) для поиска сообщений и доступа к результатам поиска по электронной почте Outlook. См. связанное [объявление в блоге](https://developer.microsoft.com/en-us/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/).

### <a name="postman"></a>Postman
В качестве альтернативы песочнице Graph используйте API Microsoft Graph в [коллекции Postman Microsoft Graph](use-postman.md), чтобы изучить поведение API и ускорить разработку приложения.

### <a name="tutorials"></a>Учебники
Воспользуйтесь новым [руководством для создания консольного приложения Java](/graph/tutorials/java), чтобы получить информацию о календаре пользователя.

### <a name="user"></a>Пользователь
Администраторы и пользователи могут [отзывать](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) все выданные маркеры обновления для пользователя. Обычно это используется для того, чтобы запретить доступ к данным организации для приложений на потерянных и украденных устройствах.


## <a name="new-in-preview-released-may---july-2019"></a>Новые предварительные версии (выпущенные с мая по июль 2019 г.)

> [!IMPORTANT]
> Возможности, в том числе API и средства в состоянии _предварительного просмотра_ могут меняться без предварительного уведомления, а некоторые из них могут никогда не быть повышены до состояния общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="calendar"></a>Календарь 
Используйте новый [API мест](/graph/api/resources/place?view=graph-rest-beta), чтобы применять различные типы расположений, например [помещения](/graph/api/resources/room?view=graph-rest-beta) и [список помещений](/graph/api/resources/roomlist?view=graph-rest-beta), настроенные администраторами Exchange Online.

### <a name="devices-and-apps"></a>Устройства и приложения
- Обновления Intune за [май](changelog.md#may-2019) 
- Обновления Intune за [июнь](changelog.md#june-2019)
- Обновления Intune за [июль](changelog.md#july-2019)

### <a name="education"></a>Образование
- Разностный запрос для [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta).
- Разностный запрос и добавления свойств для [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) и [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta).

### <a name="files"></a>Файлы 
Применяйте дату и время окончания срока действия или пароль при [создании ссылки для общего доступа](/graph/api/driveitem-createlink?view=graph-rest-beta) к файлу, папке или другому объекту [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta).

### <a name="group"></a>Группа
Получите [метки конфиденциальности](/graph/api/resources/assignedlabel?view=graph-rest-beta), чтобы обеспечить защиту конфиденциальных данных группы Office 365 и выполнение политик в отношении соответствия требованиям. Эти метки являются объектами [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta), опубликованными администраторами в Центре безопасности и соответствия требованиям Microsoft 365, в рамках возможностей Microsoft Information Protection. 

### <a name="identity-and-access"></a>Удостоверения и доступ
- Получите экземпляр [приложения](/graph/api/resources/applicationtemplate?view=graph-rest-beta) или добавьте экземпляр из коллекции приложений Azure AD в ваш каталог в качестве шаблона.
- Получите журнал всех [событий подготовки](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta) каталога в клиенте.
- Используйте новую функцию [обнаружения](/graph/api/directorydefinition-discover?view=graph-rest-beta) для поиска последней [схемы синхронизации](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta) каталога, чтобы синхронизировать объекты каталога, атрибуты и их типы с приложением.
- Получите сведения об [обнаруженном пользователе или рисках входа в систему](/graph/api/resources/riskdetection?view=graph-rest-beta) в среде Azure AD. Эта функция обнаружения рисков является частью защиты идентификации Azure AD.
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#administrative-units-permissions) _AdministrativeUnit.Read.All_ и _AdministrativeUnit.ReadWrite.All_ для чтения и записи (включая создание, обновление и удаление участников, а также управление ими) ресурсов [административных единиц](/graph/api/resources/administrativeunit?view=graph-rest-beta) соответственно.
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-beta) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-beta).

### <a name="mail"></a>Почта
Используйте более детализированное делегированное разрешение _Mail.ReadBasic_ и разрешение приложений _Mail.ReadBasic.All_, чтобы читать почтовый ящик пользователя, кроме текста сообщений, текста предварительного просмотра, вложений и расширенных свойств, а также без возможности поиска в почтовом ящике. Ранее доступные для [перечисления](/graph/api/user-list-messages?view=graph-rest-beta) и [получения](/graph/api/message-get?view=graph-rest-beta) сообщений теперь они также применимы для ресурса [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) и [изменения уведомлений](webhooks.md) для [сообщения](/graph/api/resources/message?view=graph-rest-beta) и **почтовой папки**.

### <a name="microsoft-graph-toolkit"></a>Набор средств Microsoft Graph
[Набор средств Microsoft Graph](/graph/toolkit/overview) — это набор не зависящих от платформы веб-компонентов и помощников, обеспечивающий удобную проверку подлинности и доступ к данным в Microsoft Graph.  Так как набор средств Microsoft Graph находится в состоянии предварительной версии, используйте компоненты и поставщиков наборов средств только для тех приложений, которые не предназначены для рабочей среды.

### <a name="reports"></a>Отчеты
- Получайте [отчеты о методах проверки подлинности](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta), используемых пользователями в организации, таких как самостоятельное хранение пароля и многофакторная проверка подлинности (MFA).
- Получите дополнительные [данные об использовании почтового ящика](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta) касательно числа и размера удаленных элементов.

### <a name="sites"></a>Сайты
Предоставляйте пользователям возможность [отслеживать](/graph/api/site-follow?view=graph-rest-beta) или [прекращать отслеживание](/graph/api/site-unfollow?view=graph-rest-beta) сайтов SharePoint. 

### <a name="teamwork"></a>Командная работа
- Размещайте [изображения](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta) в [сообщениях в чатах](/graph/api/resources/chatmessage?view=graph-rest-beta) Microsoft Teams.
- Поддерживайте [настройку](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta) способа обнаружения закрытой команды.
- [Устанавливайте](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta), [удаляйте](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta), [обновляйте](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta) и [перечисляйте установленные приложения Microsoft Teams](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta) для пользователя.
- Используйте доступ только для приложения, чтобы читать сообщения канала, а также отвечать на сообщения в каналах и беседах. [Запросите и получите утверждение](teams-protected-apis.md) для такого доступа.


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?
- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Office 365](https://developer.microsoft.com/ru-RU/office/dev-program), получите бесплатную подписку на Office 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/en-us/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).

