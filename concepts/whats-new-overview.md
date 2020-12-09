---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 69cc7d0ba5232770bb3b014690991ffefff6df02
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597174"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](changelog.md). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="december-2020-new-and-generally-available"></a>Декабрь 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Облачная коммуникация
Общая доступность ресурса [присутствие](/graph/api/resources/presence), позволяющего получить информацию о присутствии одного или нескольких пользователей.

### <a name="teamwork"></a>Командная работа
- Общая доступность [API для управления установкой приложения Teams](/graph/api/resources/teamsappinstallation), в том числе управления установкой приложений, а также добавления, удаления или обновления приложения в команде или в личной области пользователя.
- [Получение чата между пользователем и приложением Teams](/graph/api/userscopeteamsappinstallation-get-chat).

## <a name="december-2020-new-in-preview-only"></a>Декабрь 2020 г.: новые возможности только в предварительной версии

### <a name="identity-and-access"></a>Удостоверение и доступ
Получение или настройка метаданных версии и создания для [соглашения](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) [об условиях использования](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true), [файла соглашения](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true)и отношения [agreementfilelocalization](/graph/api/resources/agreementfilelocalization?view=graph-rest-beta&preserve-view=true) в Azure AD

## <a name="november-2020-new-and-generally-available"></a>Ноябрь 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Облачная коммуникация
- Общая доступность свойства **роль** типа [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo), разделяющего участников [виртуального собрания](/graph/api/resources/onlinemeeting) на участников и докладчиков.
- Общая доступность свойства **lobbyBypassSettings** и его [значений](/graph/api/resources/lobbybypasssettings#lobbybypassscope-values) для допуска пользователей к виртуальному собранию.
- Общая доступность свойства **isEntryExitAnnounced** для настройки параметров объявления пользователей, присоединяющихся к виртуальному собранию или покидающих его.
- Общая доступность свойства **allowedPresenters** для разрешения отдельным пользователям выступать на собрании.

### <a name="search"></a>Поиск
- Общая доступность [API запросов](/graph/api/resources/search-api-overview) Поиска (Майкрософт), поддерживающих поиск данных следующих типов:
  - [Сообщения Outlook](/graph/search-concept-messages)
  - [События календаря Outlook](/graph/search-concept-events)
  - [Ресурсы OneDrive и SharePoint](/graph/search-concept-files).

### <a name="teamwork"></a>Командная работа

- Общая доступность разрешений с согласием для конкретных ресурсов (RSC). Разрешения RSC позволяют владельцам команд предоставлять детальные разрешения рабочим приложениям на доступ и/или изменение конкретных данных команды, например на чтение параметров команды или изменение названий каналов, описаний и других параметров.
- Общая доступность API, применяемых к [каналу](/graph/api/resources/channel) или сообщениям в канале. API включают:
  - [Создание](/graph/api/conversationmember-add) или [удаление](/graph/api/conversationmember-delete) участника беседы из канала.
  - [Обновление роли участника](/graph/api/conversationmember-update) в канале.
  - Получение конкретного сообщения или всех сообщений в канале.
  - Получение конкретного ответа или всех ответов в канале.
  - [Отслеживание новых или обновленных сообщений в канале](/graph/api/chatmessage-delta).


## <a name="november-2020-new-in-preview-only"></a>Ноябрь 2020 г.: новые возможности только в предварительной версии

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
Дебют [API облачного ПК](/graph/api/resources/virtualendpoint?view=graph-rest-beta&preserve-view=true), позволяющего организациям выполнять подготовку виртуальных компьютеров для сотрудников и управлять этими компьютерами. Используйте его в сочетании с API Intune для управления физическими и виртуальными конечными точками.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
[Подписка на уведомления об изменениях](webhooks.md) в [определении задачи печати](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [ноябрь](changelog.md#november-2020) для бета-версии.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Указание URL-адресов для отправки маркеров входа пользователей и URI для кодов авторизации и маркеров доступа в свойстве **spa** [приложения](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true).
- Настройка внешнего вида и удобства использования экранов входа в Azure Active Directory посредством [свойств бренда организации](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true). Организации могут выполнять настройку на основе региональных параметров для отдельных пользователей.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Дебютное представление интерфейса [API проверки доступа в целях предоставления членства в группе](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) для регулярной проверки доступа пользователей. Интерфейс позволяет обеспечивать постоянный доступ только нужным пользователям и эффективно управлять членством в группе.

### <a name="search"></a>Поиск
Вы можете объединять числовые или строковые результаты поиска, импортированные [соединителями Microsoft Graph](/microsoftsearch/connectors-overview), которые настроены в качестве уточняемых в [схеме](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true). Ознакомьтесь с дополнительными сведениями об [уточнении результатов поиска с помощью агрегирования](search-concept-aggregation.md).


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Microsoft 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Microsoft 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).
