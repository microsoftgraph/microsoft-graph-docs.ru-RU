---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 416ba84527957b59ad4f8ff9e6d8c0194d60f245
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35420443"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

Знаете ли вы, что некоторые новые функции в Microsoft Graph реализуются на основе распространенных запросов сообщества разработчиков? 

Давайте рассмотрим стандартный жизненный цикл новой функции, узнаем, что нового в настоящее время в Microsoft Graph, и как вы можете [поделиться своими идеями](#want-to-stay-in-the-loop).

## <a name="life-cycle-of-a-feature"></a>Жизненный цикл функции

Ответственные за службы Microsoft Graph периодически оценивают идеи по функциям и потребности клиентов, а затем выбирают новые сценарии для поддержки. Чтобы создать новую функцию, они могут добавлять или обновлять API REST. Они могут сохранить тот же синтаксис API и расширить поведение функции. Кроме того, они могут предложить более удобные возможности для обучения или разработки.

В большинстве случаев ответственные за службы выпускают новые функции в следующем порядке:

1. Вначале обеспечивается статус **_предварительного_ просмотра**. Это означает, что поведение функции может измениться без предварительного уведомления. Ответственный за службу предоставляет любые связанные дополнения или обновления API REST в конечной точке бета-версии (`https://graph.microsoft.com/beta`). Не используйте функции предварительного просмотра, в том числе API, в приложениях, которые будут использоваться в рабочей среде.

2. Если ответственный за службу получает достаточную обратную связь и считает эту функцию целесообразной, то он продвигает функцию до состояния _общей доступности_. Ответственный за службу также добавляет любые связанные добавления API или обновления к конечной точке v 1.0 (`https://graph.microsoft.com/v1.0`). Эту функцию (включая ее API) в состоянии общей доступности можно использовать в приложениях, которые будут применяться в рабочей среде.

В следующих разделах описаны новые возможности, появившиеся в мае и июне 2019 г. Подробные сведения об обновлениях API см. в разделах журнала изменений за май и [июнь.  

## <a name="new-and-generally-available-released-may---june-2019"></a>Новая и общедоступная версия (выпуск: май–июнь 2019 г.)

### <a name="calendar-mail-and-personal-contacts"></a>Календарь, почта и личные контакты
Администраторы Exchange могут предоставлять приложению разрешения приложения и [ограничить доступ приложения только к подмножеству почтовых ящиков в ](auth-limit-mailbox-access.md), вместо доступа ко всем почтовым ящикам в организации, который используется по умолчанию. Такое ограничение доступа будет применено ко всем разрешениям приложения, предоставленным приложению для [календарей](permissions-reference.md#calendars-permissions), [контактов](permissions-reference.md#contacts-permissions), а также [параметров почты и почтового ящика](permissions-reference.md#mail-permissions). См. связанное объявление в блоге](https://developer.microsoft.com/en-us/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/).

### <a name="example-code-snippets"></a>Примеры фрагментов кода
В дополнение к C# и JavaScript, теперь имеются фрагменты кода Objective-C для всех разделов API в материалах для версий v1.0 и бета. См. пример Objective-C для [получения события](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example).

### <a name="mail"></a>Почта
Используйте API [папок поиска почты](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) для поиска сообщений и доступа к результатам поиска по электронной почте Outlook. См. связанное [объявление в блоге](https://developer.microsoft.com/en-us/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/).

### <a name="postman"></a>Postman
В качестве альтернативы песочнице Graph используйте API Microsoft Graph в коллекции Postman Microsoft Graph](use-postman.md), чтобы изучить поведение API и ускорить разработку приложения.

### <a name="tutorials"></a>Учебники
Воспользуйтесь новым руководством для создания консольного приложения Java](/graph/tutorials/java), чтобы получить информацию о календаре пользователя.

### <a name="user"></a>Пользователь
Администраторы и пользователи могут отзывать](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) все выданные маркеры обновления для пользователя. Обычно это используется для того, чтобы запретить доступ к данным организации для приложений на потерянных и украденных устройствах.


## <a name="new-in-preview-released-may---june-2019"></a>Новое в предварительной версии (выпуск май – июнь, 2019)

> [!IMPORTANT]
> Функции, в том числе API и средства в состоянии _предварительного просмотра_ могут изменяться без предварительного уведомления, при этом некоторые из них могут никогда не быть повышены до состояния общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
- Обновления Intune за [май](changelog.md#may-2019) 
- Обновления Intune за [июнь](changelog.md#june-2019)

### <a name="education"></a>Образование
- Разностный запрос для [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta).
- Разностный запрос и добавления свойств для [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) и [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta).

### <a name="group"></a>Группа
Получите метки конфиденциальности](/graph/api/resources/assignedlabel?view=graph-rest-beta), чтобы обеспечить защиту конфиденциальных данных группы Office 365 и выполнение политик в отношении соответствия требованиям. Эти метки являются объектами [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta), опубликованными администраторами в Центре безопасности и соответствия требованиям Microsoft 365, в рамках возможностей Microsoft Information Protection. 

### <a name="identity-and-access"></a>Удостоверения и доступ
- Получите экземпляр [приложения](/graph/api/resources/applicationtemplate?view=graph-rest-beta) или добавьте экземпляр из коллекции приложений Azure AD в ваш каталог в качестве шаблона.
- Получите список [событий подготовки](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta) в клиенте.
- Получите сведения об [обнаруженном пользователе или рисках входа в систему](/graph/api/resources/riskdetection?view=graph-rest-beta) в среде Azure AD. Эта функциональность обнаружения рисков является частью Azure AD Identity Protection (Защиты идентификации Azure AD).

### <a name="mail"></a>Почта
Используйте [разрешение Mail.ReadBasic](permissions-reference.md#mail-permissions) в API [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) и в [уведомлениях об изменениях](webhooks.md) для [сообщения](/graph/api/resources/message?view=graph-rest-beta) и **mailFolder**.

### <a name="microsoft-graph-toolkit"></a>Набор средств Microsoft Graph
[Набор средств Microsoft Graph — это набор не зависящих от платформы веб-компонентов и помощников, обеспечивающий удобную проверку подлинности и доступ к данным в Microsoft Graph.  Поскольку набор средств Microsoft Graph находится в состоянии предварительной версии, используйте поставщики набора средств и компоненты только для приложений, не предназначенных для рабочей среды.

### <a name="sites"></a>Сайты
Предоставляйте пользователям возможность отслеживать или [прекращать отслеживание](/graph/api/site-unfollow?view=graph-rest-beta) сайтов SharePoint. 

### <a name="teamwork"></a>Командная работа
Размещайте [изображения](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta) в [сообщениях в чатах](/graph/api/resources/chatmessage?view=graph-rest-beta) Microsoft Teams.
Поддерживайте [настройку](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta) способа обнаружения приватной команды.


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?
- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в программе для разработчиков Office 365](https://developer.microsoft.com/ru-RU/office/dev-program), получите бесплатную подписку на Office 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/en-us/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).

