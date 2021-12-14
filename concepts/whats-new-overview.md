---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 499fb9829c0f5b5eddc6f8b124fbf3d6375b5c12
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424577"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.


## <a name="december-2021-new-and-generally-available"></a>Декабрь 2021 г.: новые и общедоступные возможности

### <a name="cloud-communications--presence"></a>Облачные коммуникации | Присутствие
[Подпишитесь на уведомления об изменениях](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&preserve-view=true) в состоянии [присутствия](/graph/api/resources/presence) указанного пользователя. Всегда указывайте сертификат шифрования в запросе подписки, так как это [подробные уведомления, которые включают зашифрованные данные ресурсов](webhooks-with-resource-data.md).

## <a name="december-2021-new-in-preview-only"></a>Декабрь 2021 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--presence"></a>Облачные коммуникации | Присутствие
- Используйте действие [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true), чтобы задать предпочтительное состояние доступности и активности для пользователя. Присутствие пользователя становится предпочтительным.
- Используйте действие [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true), чтобы очистить предпочтительное состояние доступности и активности для пользователя.
- Используйте `Presence.ReadWrite` в качестве делегированного разрешения с действиями [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true), [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true), [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) или [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true).
- Используйте `Presence.ReadWrite.All` в качестве разрешения приложения с действиями [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true), [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true), [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) или [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
- [Получите](/graph/api/application-get?view=graph-rest-beta&preserve-view=true) сведения о сертификате [приложения](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) с помощью свойства **certification**. Свойство задается только в том случае, если приложение сертифицировано по [программе Соответствия требованиям приложений Microsoft 365](/microsoft-365-app-certification/docs/enterprise-app-certification-guide).  
- [Включите](/graph/api/permissiongrantpolicy-post-includes?view=graph-rest-beta&preserve-view=true) или [исключите](/graph/api/permissiongrantpolicy-post-excludes?view=graph-rest-beta&preserve-view=true) сертификацию как [условие](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true) в [политике предоставления разрешений](/graph/api/resources/permissiongrantpolicy?view=graph-rest-beta&preserve-view=true) посредством свойства **certifiedClientApplicationsOnly** в [permissionGrantConditionSet](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true).

### <a name="search--index"></a>Поиск | Индекс
Используйте операцию [обновления](/graph/api/externalconnectors-schema-update?view=graph-rest-beta&preserve-view=true), чтобы обновить свойства элементов в схеме [подключения](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true), включая их псевдонимы и метки.


## <a name="november-2021-new-and-generally-available"></a>Ноябрь 2021 г.: новые и общедоступные возможности

### <a name="files"></a>Файлы
Узнайте состояние диска на определенный момент времени, указав соответствующую метку времени, зашифрованную в виде URL-адреса. См. [пример](/graph/api/driveitem-delta#example-4-retrieving-delta-results-using-a-timestamp).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход
- Запустите [кампании](/graph/api/resources/authenticationMethodsRegistrationCampaign) и [заставьте пользователей регистрироваться](/graph/api/resources/registrationEnforcement) во время регистрации, чтобы настроить целевые методы проверки подлинности.
-  Настройте [поставщика удостоверений Apple](/graph/api/resources/applemanagedidentityprovider) в клиенте Azure AD B2C.

## <a name="november-2021-new-in-preview-only"></a>Ноябрь 2021 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Онлайн-собрание
Автоматический допуск новых типов участников в собрания по сети в обход "зала ожидания" собрания.
- Только пользователи, которых приглашает организатор.
- Только участники из одной компании.

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
- Определите [конфигурацию](/graph/api/resources/cloudPcDomainJoinConfiguration?view=graph-rest-beta&preserve-view=true) того, как подготовленное устройство с облачным компьютером может присоединиться к Azure Active Directory (Azure AD): только в облаке и присоединиться только к Azure AD, или в гибридной системе и присоединиться к локальной службе Active Directory и Azure AD.
- Получите [ресурс образа коллекции](/graph/api/resources/cloudPcGalleryImage?view=graph-rest-beta&preserve-view=true) текущей организации, который можно использовать для подготовки облачного компьютера к работе.

### <a name="devices-and-apps--device-updates"></a>Устройства и приложения | Обновления устройств
- Используйте [параметры мер безопасности](/graph/api/resources/windowsupdates-safeguardSettings?view=graph-rest-beta&preserve-view=true), чтобы отказаться от защиты от вероятных проблем при развертывании.
- Поддержка [состояния развертывания](/graph/api/resources/windowsupdates-deploymentState?view=graph-rest-beta&preserve-view=true) при невозможности развертывания из-за того, что содержимое больше не может быть развернуто, например после окончания обслуживания.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
- Определите и назначьте [настраиваемые атрибуты безопасности](/graph/api/resources/custom-security-attributes-overview?view=graph-rest-beta&preserve-view=true) объектам Azure AD. Используйте эти атрибуты для хранения информации, классификации объектов или применения детального контроля доступа к определенным ресурсам Azure. Используйте эти атрибуты вместе с [контролем доступа на основе атрибутов Azure](/azure/role-based-access-control/conditions-overview) (Azure ABAC).
- [Создайте группу в административной единице](/graph/api/administrativeunit-post-members?view=graph-rest-beta&preserve-view=true).

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
[Отчеты об использовании Microsoft 365](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true) в типе вывода JSON больше не строго типизированы и имеют тип `Edm.Stream`. Подробности см. в статье [Изменение свойств OData в API отчетов об использовании Microsoft 365 в Microsoft Graph](https://devblogs.microsoft.com/microsoft365dev/odata-property-changes-to-microsoft-365-usage-reports-api-in-microsoft-graph/).

### <a name="teamwork"></a>Teamwork
Отметьте чат как [прочитанный](/graph/api/chat-markChatReadForUser?view=graph-rest-beta&preserve-view=true) или [непрочитанный](/graph/api/chat-markchatunreadforuser?view=graph-rest-beta&preserve-view=true) для пользователя.



## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на сайте [сообщества Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Впервые в состоянии **_предварительной версии_**. Все связанные обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Microsoft 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Microsoft 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](https://developer.microsoft.com/graph/changelog/).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).
