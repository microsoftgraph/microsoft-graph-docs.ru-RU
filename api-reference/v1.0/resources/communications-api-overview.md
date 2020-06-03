---
title: Работа с API коммуникаций в Microsoft Graph
description: API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования функций голоса и видео.
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: b0337dfe620318482f3cc400512d5c381bf123a9
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491884"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a>Работа с API коммуникаций в Microsoft Graph

API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования основных возможностей общения в приложениях и службах. Этот API можно использовать для создания и приема звонков, а также для создания и получения координат собраний.

API коммуникаций можно использовать для создания служебных приложений (ботов), выполняющих роль участников в звонке, а также создающих собрания и получающих приглашения на них от имени пользователей.
Этот API предоставляет функции звонков, а также возможность создавать собрания по сети и получать приглашения на них. С помощью этого API можно использовать служебные приложения (боты), при этом боты могут участвовать в звонках VoIP или собраниях Microsoft Teams.

## <a name="authorization"></a>Авторизация

Для доступа к API коммуникаций требуется одно из указанных ниже [разрешений](https://docs.microsoft.com/graph/permissions-reference#calls-permissions). Эти разрешения должны предоставляться администратором

| Сценарий                 | Разрешения                                  |
|:------------------------------------|:---------------------------------------------|
| Звонки                 | Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All |
| Собрания                 | OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All |
| Записи звонков             | CallRecords.Read.All |

## <a name="common-use-cases"></a>Основные варианты использования

В таблице ниже перечислены некоторые распространенные варианты использования API коммуникаций.

| Варианты использования                         | Ресурсы REST                                 | См. также  |
|:------------------------------------|:---------------------------------------------|:----------|
| Создание приватных и групповых звонков, а также присоединение к ним   | [Звонок](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0)| [Методы звонков](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#methods)| 
|Звонки с интерактивным речевым взаимодействием   |     | [Методы для интерактивного речевого взаимодействия](https://docs.microsoft.com/graph/api/resources/calls-api-ivr-overview?view=graph-rest-v1.0)
| Элементы управления звонком (участник) | [Участник](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0)   ||
|Собрания|[onlineMeeting](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0)| [Методы для собраний](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#methods)|
| Получение записей звонков | [callRecord](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) | [Подписки веб-перехватчиков](/graph/api/resources/webhooks?view=graph-rest-1.0) |

## <a name="common-properties"></a>Общие свойства

| Ресурс                | Свойства                             |
|:------------------------------------|:---------------------------------------------|
| call                               | [свойства объекта call](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#properties)  |
| participant                         | [свойства объекта participant](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0#properties) |
| onlineMeeting                            | [свойства объекта onlineMeeting](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#properties)                     |
| callRecord | [Свойства callRecord](/graph/api/resources/callrecords-callrecord#properties) |

## <a name="whats-new"></a>Новые возможности
Узнайте о [последних новых возможностях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="see-also"></a>См. также

- [Примеры API коммуникаций](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [Пакет SDK для передачи сигналов коммуникаций](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)
- [Пакет SDK мультимедиа коммуникаций](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media)
