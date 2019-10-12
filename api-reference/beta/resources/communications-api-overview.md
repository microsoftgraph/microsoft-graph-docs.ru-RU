---
title: Работа с API коммуникаций в Microsoft Graph
description: API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования функций голоса и видео.
author: VinodRavichandran
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: d5bcd46cb89a5d911c9286ef5c2093460949a3a1
ms.sourcegitcommit: 99cbeac2ca652632d2946c4740133c9b82c8e992
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/12/2019
ms.locfileid: "37477082"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a>Работа с API коммуникаций в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования основных возможностей общения в приложениях и службах. Этот API можно использовать для создания и приема звонков, создания и получения координат собраний, а также проверки присутствия пользователей.

API коммуникаций можно использовать для создания служебных приложений (ботов), выполняющих роль участников в звонке, а также создающих собрания и получающих приглашения на них от имени пользователей. <!-- and to check presence availability and activity of users. -->
Этот API предоставляет функции звонков, а также возможность создавать собрания по сети и получать приглашения на них. С помощью этого API можно использовать служебные приложения (боты), при этом боты могут участвовать в звонках VoIP или собраниях Microsoft Teams.

## <a name="authorization"></a>Авторизация

Для доступа к API коммуникаций требуется одно из указанных ниже [разрешений](https://docs.microsoft.com/ru-RU/graph/permissions-reference#calls-permissions). Эти разрешения должны предоставляться администратором

| Сценарий                 | Разрешения                                  |
|:------------------------------------|:---------------------------------------------|
| Звонки                 | Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All |
| Собрания                 | OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All |

## <a name="common-use-cases"></a>Основные варианты использования

В таблице ниже перечислены некоторые распространенные варианты использования API коммуникаций.

| Варианты использования                         | Ресурсы REST                                 | См. также  |
|:------------------------------------|:---------------------------------------------|:----------|
| Создание приватных и групповых звонков, а также присоединение к ним   | [Звонок](https://docs.microsoft.com/en-us/graph/api/resources/call?view=graph-rest-beta)| [Методы звонков](https://docs.microsoft.com/en-us/graph/api/resources/call?view=graph-rest-beta#methods)| 
|Звонки с интерактивным речевым взаимодействием   |     | [Методы для интерактивного речевого взаимодействия](https://docs.microsoft.com/en-us/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)
| Элементы управления звонком (участник) | [Участник](https://docs.microsoft.com/en-us/graph/api/resources/participant?view=graph-rest-beta)   ||
|Собрания|[onlineMeeting](https://docs.microsoft.com/en-us/graph/api/resources/onlinemeeting?view=graph-rest-beta)| [Методы для собраний](https://docs.microsoft.com/en-us/graph/api/resources/onlinemeeting?view=graph-rest-beta#methods)|

## <a name="common-properties"></a>Общие свойства

| Ресурс                | Свойства                             |
|:------------------------------------|:---------------------------------------------|
| call                               | [свойства объекта call](https://docs.microsoft.com/en-us/graph/api/resources/call?view=graph-rest-beta#properties)  |
| participant                         | [свойства объекта participant](https://docs.microsoft.com/en-us/graph/api/resources/participant?view=graph-rest-beta#properties) |
| onlineMeeting                            | [свойства объекта onlineMeeting](https://docs.microsoft.com/en-us/graph/api/resources/onlinemeeting?view=graph-rest-beta#properties)                     |

## <a name="see-also"></a>См. также

- [Примеры API коммуникаций](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [Пакет SDK для передачи сигналов коммуникаций](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [Пакет SDK мультимедиа коммуникаций](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)
