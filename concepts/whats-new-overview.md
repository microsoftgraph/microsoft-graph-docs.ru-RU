---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: a3adfca811e6b4c770ebe97d3279f4568db8d3ed
ms.sourcegitcommit: cfcd58f09bc44de0a32ecf4c627267035902a07e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/27/2019
ms.locfileid: "37278616"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

Знаете ли вы, что некоторые новые возможности Microsoft Graph реализуются на основе распространенных запросов сообщества разработчиков? 

Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 

Ниже представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробные сведения об обновлениях API см. в разделах журнала изменений API за [август](changelog.md#august-2019) и [сентябрь](changelog.md#september-2019). 

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

## <a name="september-2019-new-in-preview"></a>Сентябрь 2019 г.: новые возможности в предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [сентябрь](changelog.md#september-2019)

### <a name="identity-and-access"></a>Удостоверение и доступ
Добавочные улучшения для [синхронизации удостоверений](/graph/api/resources/synchronization-overview?view=graph-rest-beta) в облачном приложении для клиента:

- Чтобы сохранять параметры для [задания синхронизации](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)
- Чтобы указать причину применения [карантина](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta) для задания синхронизации

### <a name="teamwork"></a>Командная работа
Программная поддержка канала **Общий** в [команде](/graph/api/resources/team?view=graph-rest-beta) и настройки [параметров участников](/graph/api/resources/teammembersettings?view=graph-rest-beta), чтобы разрешить участникам команд создавать закрытые каналы в **команде**.

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


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?
- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Office 365](https://developer.microsoft.com/ru-RU/office/dev-program), получите бесплатную подписку на Office 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).

