---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 5e56d74e35bf55caade6c0137619d0d24ecc7323
ms.sourcegitcommit: cea768f767cf27a938b72bb26892d70e3dedaf2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/08/2020
ms.locfileid: "41865853"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Полный список обновлений API см. в [декабрьском](changelog.md#december-2019) и [ноябрьском](changelog.md#november-2019) разделах журнала изменений API. 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="february-2020-new-and-generally-available"></a>2020 февраля: новая и общедоступная

### <a name="calendar"></a>Календарь
Просмотрите пример [создания события в общем или делегированном календаре](outlook-create-event-in-shared-delegated-calendar.md), а также действия и свойства, доступные для делегата, приглашенных и владельца календаря во время этого процесса.

### <a name="security"></a>Безопасность
Чтобы повысить безопасность при подписке на [уведомления об изменениях пользовательских данных](webhooks.md), [установите Transport Layer Security (TLS) 1.2](https://docs.microsoft.com/configmgr/core/plan-design/security/enable-tls-1-2) или выше на клиентах и серверах сайтов, используемых в процессе уведомления. Новое требование вводится поэтапно, начиная с 15 февраля 2020 года. К 15 мая 2020 года все конечные точки уведомления должны соответствовать новому требованию TLS. [Узнайте о стадиях развертывания](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) и при необходимости воспользуйтесь новым свойством **latestSupportedTlsVersion** в качестве временного решения, чтобы избежать сбоев подписки до выполнения обновления TLS.

## <a name="february-2020-new-in-preview"></a>Февраль 2020: новое в предварительной версии

### <a name="calendar"></a>Календарь
Просмотрите [задачи, поддерживаемые API-интерфейсами предварительного просмотра, которые управляют совместным использованием и делегированием календаря](outlook-share-or-delegate-calendar.md).


## <a name="january-2020-new-and-generally-available"></a>Январь 2020 г.: новые и общедоступные возможности

### <a name="security"></a>Безопасность
В рамках управления оповещениями используйте метод [обновления оповещений](/graph/api/alert-update?view=graph-rest-1.0) и обновляйте поле **комментариев** как `Closed in IPC` или `Closed in MCAS`.

### <a name="teamwork"></a>Командная работа
Используйте свойство навигации **primaryChannel** [группы](/graph/api/resources/team?view=graph-rest-1.0) для доступа к каналу по умолчанию **General**.

### <a name="users"></a>Пользователи
Чтобы получить доступ к одному или нескольким удостоверениям, которые [пользователь](/graph/api/resources/user?view=graph-rest-1.0) может использовать для входа в учетную запись пользователя Azure AD, используйте свойство **удостоверения **. Удостоверения могут предоставляться поставщиками услуг Майкрософт, организаций или социальных удостоверений, таких как Facebook, Google или Microsoft. Это свойство позволяет пользователю входить в учетную запись пользователя с помощью любого из этих удостоверений.

## <a name="january-2020-new-in-preview"></a>Январь 2020: Новое в предварительной версии

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [Январь](changelog.md#january-2020).

<!--
### Identity and access
Access specific types of [policies for an organization](/graph/api/resources/policy-overview?view=graph-rest-beta) using the `/policies` URL segment and specifying the policy type. For example, an organization can enforce a policy to automatically sign a user out from a web session after a period of inactivity; see CRUD operations for instances of [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta). This is a [breaking change](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/) to make it easier to discover all policies, by grouping all typed policies under the `/policies` segment. Access other typed policies in a similar approach: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta), and [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta).
-->


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

