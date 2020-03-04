---
title: Работа с API коммуникаций в Microsoft Graph
description: API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования функций голоса и видео.
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 7869ac59f84f266542254fd0c8fc8ea97ee4815d
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394584"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a>Работа с API коммуникаций в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования основных возможностей общения в приложениях и службах. Этот API можно использовать для создания и приема звонков, создания и получения координат собраний, а также проверки присутствия пользователей.

API коммуникаций можно использовать для создания служебных приложений (ботов), выполняющих роль участников в звонке, создающих собрания и получающих приглашения на них от имени пользователей, а также для проверки доступности пользователей и их действий.
Этот API предоставляет функции звонков, а также возможность создавать собрания по сети и получать приглашения на них. С помощью этого API можно использовать служебные приложения (боты), при этом боты могут участвовать в звонках VoIP или собраниях Microsoft Teams.

## <a name="authorization"></a>Авторизация

Для доступа к API коммуникаций требуется одно из указанных ниже [разрешений](/graph/permissions-reference#calls-permissions). Эти разрешения должны предоставляться администратором

| Сценарий                 | Разрешения                                  |
|:------------------------------------|:---------------------------------------------|
| Звонки                 | Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All |
| Собрания                 | OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All |
| Присутствие                 | Presence.Read, Presence.Read.All |
| Записи звонков             | CallRecords.Read.All |

## <a name="common-use-cases"></a>Основные варианты использования

В таблице ниже перечислены некоторые распространенные варианты использования API коммуникаций.

| Варианты использования                         | Ресурсы REST                                 | См. также  |
|:------------------------------------|:---------------------------------------------|:----------|
| Создание приватных и групповых звонков, а также присоединение к ним   | [Звонок](/graph/api/resources/call?view=graph-rest-beta)| [Методы звонков](/graph/api/resources/call?view=graph-rest-beta#methods)|
|Звонки с интерактивным речевым взаимодействием   |     | [Методы для интерактивного речевого взаимодействия](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)
| Элементы управления звонком (участник) | [Участник](/graph/api/resources/participant?view=graph-rest-beta)   ||
|Собрания|[onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta)| [Методы для собраний](/graph/api/resources/onlinemeeting?view=graph-rest-beta#methods)|
|Присутствие | [presence](/graph/api/resources/presence) | [Методы для присутствия](/graph/api/resources/presence#methods) |
| Получение записей звонков | [callRecord](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta) | [Подписки веб-перехватчиков](/graph/api/resources/webhooks?view=graph-rest-beta) |

## <a name="common-properties"></a>Общие свойства

| Ресурс                | Свойства                             |
|:------------------------------------|:---------------------------------------------|
| call                               | [свойства объекта call](/graph/api/resources/call?view=graph-rest-beta#properties)  |
| participant                         | [свойства объекта participant](/graph/api/resources/participant?view=graph-rest-beta#properties) |
| onlineMeeting                            | [свойства объекта onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta#properties)                     |
| presence | [свойства объекта presence](/graph/api/resources/presence#properties) |
| callRecord | [Свойства callRecord](/graph/api/resources/callrecords-callrecord#properties) |

## <a name="see-also"></a>См. также

- [Примеры API коммуникаций](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [Пакет SDK для передачи сигналов коммуникаций](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [Пакет SDK мультимедиа коммуникаций](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)
