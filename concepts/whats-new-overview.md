---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 5926d13f8971d891d48eb09205162f502999faed
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384473"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.

## <a name="august-2021-new-and-generally-available"></a>Август 2021 г.: новые и общедоступные возможности

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Ежемесячные обновления Intune за сентябрь для версии 1.0. Установите фильтр **Дата** в значение "август 2021" и найдите раздел с таким заголовком.

### <a name="devices-and-apps--service-health-and-communications"></a>Устройства и приложения | Работоспособность и взаимодействие служб
Общедоступная версия [API взаимодействия служб](service-communications-concept-overview.md) в Microsoft Graph для доступа к состоянию работоспособности и записям центра сообщений об облачных службах (Майкрософт).

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Получите коллекцию областей проверки доступа, в которой определены проверяющие и запасные проверяющие для [экземпляра проверки доступа](/graph/api/resources/accessReviewInstance).

## <a name="august-2021-new-in-preview-only"></a>Август 2021 г.: новые возможности только в предварительной версии

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Ежемесячные обновления Intune за сентябрь для бета-версии. Установите фильтр **Дата** в значение "август 2021" и найдите раздел с таким заголовком.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- [Повторно обработайте](/graph/api/accesspackageassignmentrequest-reprocess?view=graph-rest-beta&preserve-view=true) запрос[ на назначение пакета доступа](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true), чтобы автоматически повторить попытку выполнения запроса пользователя на доступ к пакету.
- [Повторно обработайте](/graph/api/accesspackageassignment-reprocess?view=graph-rest-beta&preserve-view=true) запрос[ на назначение пакета доступа](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true), чтобы автоматически проверить назначения пользователя и обеспечить их выполнение.
- [Получите набор требований политики](/graph/api/accesspackage-getapplicablepolicyrequirements?view=graph-rest-beta&preserve-view=true) чтобы создать [запрос назначения для пакета доступа](/graph/api/resources/accesspackageassignmentrequestrequirements?view=graph-rest-beta&preserve-view=true).
- Получите коллекцию ресурсов [проверки доступа и проверяющих](/graph/api/resources/accessreviewreviewer?view=graph-rest-beta&preserve-view=true), где определены проверяющие, с которыми будет установлена связь для [экземпляра проверки доступа](/graph/api/resources/accessReviewInstance?view=graph-rest-beta&preserve-view=true).
- Получите или задайте длительность бездействия, на основе которого будут настраиваться рекомендации, в разделе [параметров расписания проверки доступа](/graph/api/resources/accessReviewScheduleSettings?view=graph-rest-beta&preserve-view=true), используя свойство **recommendationLookBackDuration**.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
Организации могут использовать [политики для применения рекомендованных методик для приложений, использующих методы проверки подлинности приложений](/graph/api/resources/applicationauthmethodpolicy?view=graph-rest-beta&preserve-view=true). Такие политики могут применяться к [приложениям и субъектам-службам](/graph/api/resources/appmanagementpolicy?view=graph-rest-beta&preserve-view=true) или [всем приложениям и субъектам-службам в клиенте](/resources/tenantappmanagementpolicy?view=graph-rest-beta&preserve-view=true).

## <a name="july-2021-new-and-generally-available"></a>Июль 2021 г.: новые и общедоступные возможности

### <a name="cloud-communications--calls"></a>Облачные коммуникации | Звонки
Поддержка ограничения емкости для количества участников, которое приложение может обрабатывать при [ответе](/graph/api/call-answer) на [вызов](/graph/api/resources/call), в организациях, внедряющих [запись звонков на основе политики Teams](/microsoftteams/teams-recording-policy).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Общедоступные поставщики удостоверений с общим базовым типом [identityProviderBase](/graph/api/resources/identityproviderbase):
  - Встроенные поставщики удостоверений для сценариев Azure AD B2B в клиенте Azure AD. Эти поставщики могут поддерживать Azure AD, учетную запись Майкрософт (MSA) или разовые коды доступа, отправляемые по электронной почте.
  - Поставщики социальных удостоверений в клиенте Azure AD B2C, позволяющие пользователям зарегистрироваться и войти в службу с помощью учетной записи социальных сетей, например Microsoft, Google, Facebook, Amazon, LinkedIn или Twitter.
- Не рекомендуется пользование предыдущими API [поставщика удостоверений](/graph/api/resources/identityprovider).

### <a name="users"></a>Пользователи
Позвольте пользователям [менять собственный пароль](/graph/api/user-changepassword) без роли администратора.


## <a name="july-2021-new-in-preview-only"></a>Июль 2021 г.: новые возможности только в предварительной версии

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
Локальное подключение [проверки работоспособности ](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) может выявлять больше возможных типов ошибок проверки работоспособности.
- Учетная запись облачного ПК не найдена в подразделении (`adJoinCheckComputerObjectAlreadyExists`).
- Объект облачного ПК не найден в Azure AD (`azureAdDeviceSyncCheckDeviceNotFound`).
- Превышено время ожидания с момента проверки синхронизации объекта облачного ПК с Azure AD (`azureAdDeviceSyncCheckLongSyncCircle`). 

Подробные сведения и рекомендуемые действия по исправлению см. в [справочных материалах](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true#cloudpconpremisesconnectionhealthcheckerrortype-values).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Ежемесячные обновления Intune за сентябрь для бета-версии. Установите фильтр **Дата** в значение "июль 2021" и найдите раздел с таким заголовком.

### <a name="devices-and-apps--multi-tenant-management"></a>Устройства и приложения | Управление несколькими клиентами
Дебютный выпуск [Microsoft 365 Lighthouse API](managedtenants-concept-overview.md), который позволяет поставщикам управляемых служб удаленно управлять несколькими пользовательскими клиентами в масштабе для обеспечения соответствия требованиям и обнаружения угроз, а также обеспечивать работоспособное и безопасное состояние устройств клиента.

### <a name="education"></a>Образование
- Получите количество ошибок и сообщение о состоянии как часть [состояния синхронизации учебных данных](/graph/api/resources/educationsynchronizationprofilestatus?view=graph-rest-beta&preserve-view=true).
- Получите `extracting` или `validating` как возможные состояния такой синхронизации.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Получите коллекцию ошибок в жизненном цикле [экземпляра проверки доступа](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true).

### <a name="search"></a>Поиск
- Используйте [API Поиска (Майкрософт) для получения сведений о людях](search-concept-person.md), наиболее релевантных для пользователя. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями. 
- Получите доступ к [API индексации соединителей](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true) в подпространстве имен microsoft.graph.externalConnectors.

### <a name="teamwork"></a>Командная работа
- [Подпишитесь на уведомления об изменениях в ресурсе чата](teams-changenotifications-chat.md).
- [Подпишитесь на уведомления об изменениях пользователей в чате](teams-changenotifications-chatmembership.md), в [канале](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) или в [группе](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) (например, ресурсы [conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true)).
- Получайте сведения о событиях, происходящих в чате, канале или команде, путем доступа к ресурсу [eventMessageDetail](/graph/api/resources/EventMessageDetail?view=graph-rest-beta&preserve-view=true) из [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) или [чата](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true). Например, о таких событиях, как добавление участников в канал или чат, или изменение описания команды.


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
