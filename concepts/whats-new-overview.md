---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: ae6cd9109faf46aa9ab2b55c0015f846f494a619
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119786"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Полный список обновлений API см. в [декабрьском](changelog.md#december-2019) и [ноябрьском](changelog.md#november-2019) разделах журнала изменений API. 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="january-2020-new-and-generally-available"></a>Январь 2020 г.: новые и общедоступные возможности

### <a name="security"></a>Безопасность
В рамках управления оповещениями используйте метод [обновления оповещений](/graph/api/alert-update?view=graph-rest-1.0) и обновляйте поле **комментариев** как `Closed in IPC` или `Closed in MCAS`.

## <a name="december-2019-new-and-generally-available"></a>Декабрь 2019 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Коммуникации из облака
API коммуникаций из облака имеет общедоступное состояние, API ресурсов [call](/graph/api/resources/call?view=graph-rest-1.0) и [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-1.0) [доступны в версии 1.0](/graph/api/resources/communications-api-overview?view=graph-rest-1.0).

### <a name="education"></a>Образование
Используйте свойство **classSettings**, чтобы управлять параметрами для конкретного класса, например включением отправки еженедельных дайджестов заданий.  Это свойство доступно в ресурсе [team](/graph/api/resources/team?view=graph-rest-1.0), когда команда представляет собой [группу обучения](/graph/api/resources/educationclass?view=graph-rest-1.0).

### <a name="identity-and-access"></a>Удостоверение и доступ 
[При попытке получить объекты-контейнеры с ограниченными разрешениями часть данных возвращается](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects). В качестве примера можно привести экземпляр [группы](/graph/api/resources/group?view=graph-rest-1.0), связанный с [пользователем](/graph/api/resources/user?view=graph-rest-1.0), другую **группу** и [устройство](/graph/api/resources/device?view=graph-rest-1.0). Приложение, у которого есть только разрешения User.Read.All и Group.Read.All, при попытке получить доступ к этому экземпляру **группы** получит объекты **user** и **group**, а также ограниченные данные для объекта **device** (только тип данных и ИД объекта), не включающие значения свойств.

### <a name="people-and-workplace-intelligence"></a>Люди и рабочая аналитика
API аналитики имеет общедоступное состояние. Используйте этот API в рабочих приложениях для определения наиболее релевантных документов, которые:

- [касаются](/graph/api/insights-list-trending?view=graph-rest-1.0) пользователя;
- [используются](/graph/api/insights-list-used?view=graph-rest-1.0) пользователем;
- [к которым предоставлен доступ](/graph/api/insights-list-shared?view=graph-rest-1.0) пользователю или пользователем.

### <a name="reports"></a>Отчеты
Чтобы получать отчеты об использовании Office 365 с помощью разрешений, делегированных пользователем, администраторам необходимо назначить пользователю роль администратора Azure AD с ограниченными правами. Это может быть одна из следующих ролей: администратор организации, администратор Exchange, администратор SharePoint, администратор Lync, глобальный читатель или читатель отчетов. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](reportroot-authorization.md).

### <a name="toolkit"></a>Набор средств
Выпущен набор средств Microsoft Graph версии 1.1. Список улучшений и исправлений ошибок см. в [разделе за декабрь 2019 г.](changelog.md#december-2019) журнала изменений.

## <a name="december-2019-new-in-preview"></a>Декабрь 2019 г.: новые возможности в предварительной версии

### <a name="cloud-communications"></a>Коммуникации из облака
- Чтобы получить сведения о доступности и текущей активности одного или нескольких пользователей, используйте новый ресурс [presence](/graph/api/resources/presence?view=graph-rest-beta).
- [Удалите](/graph/api/onlinemeeting-delete?view=graph-rest-beta) экземпляр [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta).
- Ознакомьтесь с [разделом за декабрь 2019 г.](changelog.md#december-2019) журнала изменений, чтобы переименовать или удалить несколько элементов ресурсов [call](/graph/api/resources/call?view=graph-rest-beta) и [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta) и обеспечить соответствие версии v1 этих ресурсов.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [декабрь](changelog.md#december-2019)

### <a name="identity-and-access"></a>Удостоверение и доступ 
- Исправлено поведение отношений **appRoleAssignments** и **appRoleAssignedTo** в [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta).
- Используйте [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta) в [функции управления правами в Azure AD](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta) для запроса добавления ресурса к [каталогу](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta), чтобы роли этого ресурса можно было использовать в [пакете для доступа](/graph/api/resources/accesspackage?view=graph-rest-beta).
- Используйте [API оценки угроз](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta), чтобы дать администраторам возможность сообщать о подозрительной почте, URL-адресах фишинга, вложениях электронной почты и других файлах. Вывод, сделанный при сканировании потока, может побудить их изменить политику организации соответствующим образом.

### <a name="teamwork"></a>Командная работа
- [Настройка уведомлений об изменениях, включающих данные](webhooks-with-resource-data.md) для ресурсов [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) в каналах и чатах Microsoft Teams.
- [Подписка на уведомления](/graph/api/resources/subscription?view=graph-rest-beta) о новых и измененных [сообщениях канала или чата](/graph/api/resources/chatmessage?view=graph-rest-beta).
- Используйте ресурс [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta), чтобы включить указание доступности пользователя для назначения смен в [графике](/graph/api/resources/schedule?view=graph-rest-beta). Настройте эту возможность в [параметрах](/graph/api/resources/usersettings?view=graph-rest-beta) пользователя.


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

