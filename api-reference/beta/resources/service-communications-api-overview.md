---
title: Работа с API-службами связи в Microsoft Graph
description: Вы можете использовать API сообщений службы в Microsoft Graph для доступа к состояниям здоровья и сообщениям центра сообщений о службы Майкрософт".
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 0c00bf36e3f745614bd3f0e523e75b7229561d78
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58257742"
---
# <a name="working-with-service-communications-api-in-microsoft-graph"></a>Работа с API службы связи в Microsoft Graph
API сообщений службы предоставляет службы здоровья и сообщений центра сообщений, относящихся к облачным службам Майкрософт, которые подписаны вашим клиентом. Вы можете получить текущие и исторические данные о состоянии здоровья службы Майкрософт (например, Exchange Online службы не существует). Вы можете проверить состояние службы, чтобы определить, отслеживается ли проблема и находится ли решение, прежде чем вызывать службу поддержки или тратить время на устранение неполадок. Сообщения центра сообщений позволяет отслеживать предстоящие изменения, в том числе новые функции, обновления и другие важные объявления (например, Exchange Online получает новую функцию).

## <a name="authorization"></a>Авторизация
Microsoft Graph позволяет приложениям получать авторизованный доступ к здравоохранению и изменять сообщения о облачной службе Майкрософт, подписанной клиентом. С соответствующими разрешениями делегирования или приложения [ваше](/graph/permissions-reference#service-communications-permissions)приложение может получать доступ к данным связи от имени подписанного пользователя или без какого-либо подписанного пользователя в клиенте. Как делегированная, так и тип приложения этих разрешений предоставляется только администратором.

Дополнительные сведения о маркерах доступа, регистрации приложений, делегировании и разрешениях на приложения см. в основных сведениях о проверке подлинности [и авторизации.](/graph/auth/auth-concepts)

### <a name="access-service-communications-api-on-behalf-of-signed-in-user"></a>API доступа к службам связи от имени подписанного пользователя

Для доступа к API службы связи от имени подписанного пользователя необходимы делегированные разрешения. Приложения холста, стоящие перед [клиентом, такие](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/homepage) как Центр администрирования Microsoft 365 (доступные только для ролей администратора), могут вызывать API коммуникаций службы, чтобы получить данные о состоянии службы и объявлениях службы для клиента подписанного пользователя _от_ имени подписанного пользователя . Пользователи могут узнать, являются ли их службы, подписав подписку, здоровыми или имеют проблемы. Они также могут узнать о текущих проблемах служб, затрагивающих их клиентов. 

### <a name="access-service-communications-api-without-user"></a>API доступа к службам связи без пользователя

Для доступа к API службы коммуникаций без подписанного пользователя необходимы разрешения приложений. Приложения, которые работают как службы backend, такие как службы мониторинга или оповещения, могут вызывать API сообщений службы с их собственным удостоверением, а не от имени пользователя. Эти службы могут создавать настраиваемые конвейеры мониторинга и оповещения и вызывать API сообщений службы для получения данных о состоянии службы и объявлениях о службах. 


## <a name="common-use-cases-and-required-permissions"></a>Распространенные случаи использования и необходимые разрешения

|Варианты использования|Запросы API| Необходимые разрешения| Поддерживаемые типы разрешений|
|:--------|:--------|:--------|:--------|
| Список обзоров состояния здоровья для клиента | [Список healthOverviews](/graph/api/serviceannouncement-list-healthoverviews?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | Делегированная и приложение | 
| Получить определенные сведения о состоянии здоровья службы для клиента | [Get serviceHealth](/graph/api/servicehealth-get?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | Делегированная и приложение |
| Список всех проблем служб для клиента | [Проблемы со списком](/graph/api/serviceannouncement-list-issues?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | Делегированная и приложение |
| Получить определенную проблему службы для клиента | [Получить проблему](/graph/api/servicehealthissue-get?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | Делегированная и приложение |
| Получите отчет о проверке после инцидента для клиента | [Получить отчет об инциденте](/graph/api/servicehealthissue-incidentreport?view=graph-rest-beta&preserve-view=true)| _ServiceHealth.Read.All_ | Делегированная и приложение |
| Список всех сообщений службы для клиента | [Список сообщений](/graph/api/serviceannouncement-list-messages?view=graph-rest-beta&preserve-view=true) | _ServiceMessage.Read.All_ | Делегированная и приложение |
| Получить определенное сообщение службы для клиента | [Получение сообщения](/graph/api/serviceupdatemessage-get?view=graph-rest-beta&preserve-view=true) | _ServiceMessage.Read.All_ | Делегированная и приложение |
| Обновление состояния сообщения службы для записи в пользователе | Список операций состояния см. в [странице serviceUpdateMessage.](/graph/api/resources/serviceupdatemessage?view=graph-rest-beta&preserve-view=true)| _ServiceMessageViewpoint.Write_ | Delegated |

## <a name="availability-in-national-clouds"></a>Доступность в национальных облаках
Этот API связи службы доступен во всех национальных облачных развертываниях Майкрософт. Вы можете получать данные о состоянии обслуживания и связи для всех клиентов в национальных облаках Майкрософт. Подробные сведения см. [в национальных облачных развертываниях.](/graph/deployments)

|Национальные облачные развертывания|URL-адрес API (частичный)|
|:--------------|:-----------------|
|Глобальная служба Microsoft Graph| https://graph.microsoft.com/beta/admin/serviceAnnouncement/|
|Microsoft Graph для правительства США L4 (GccHigh)|https://graph.microsoft.us/beta/admin/serviceAnnouncement/|
|Microsoft Graph для правительства США L5 (DoD)|https://dod-graph.microsoft.us/beta/admin/serviceAnnouncement/|
|Microsoft Graph для Германии|https://graph.microsoft.de/beta/admin/serviceAnnouncement/|
|Microsoft Graph для Китая под управлением 21Vianet|https://microsoftgraph.chinacloudapi.cn/beta/admin/serviceAnnouncement/|

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия

API сообщений службы может открыть новые способы взаимодействия с пользователями:

- [Обзор доступа к сведениям о работоспособности и взаимодействии служб в Microsoft Graph](/graph/service-communications-concept-overview)
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/en-us/graph/partners).
