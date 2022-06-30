---
title: Работа с API облачных коммуникаций в Microsoft Graph
description: API облачных коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования функций голоса и видео.
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
ms.localizationpriority: high
ms.openlocfilehash: b8020b413b9d3368bc1b3a7bb0dfb93fe93a18be
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437900"
---
# <a name="working-with-the-cloud-communications-api-in-microsoft-graph"></a>Работа с API облачных коммуникаций в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

API облачных коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования основных возможностей общения в приложениях и службах. Этот API можно использовать для создания и приема звонков, создания и получения координат собраний, а также проверки присутствия пользователей.

API облачных коммуникаций можно использовать для создания служебных приложений (ботов), выполняющих роль участников в звонке, создающих собрания и получающих приглашения на них от имени пользователей, а также для проверки доступности пользователей и их действий.
Этот API предоставляет функции звонков, а также возможность создавать собрания по сети и получать приглашения на них. С помощью этого API можно использовать служебные приложения (боты), при этом боты могут участвовать в звонках VoIP или собраниях Microsoft Teams.

## <a name="authorization"></a>Авторизация

Для доступа к API облачных коммуникаций требуется одно из указанных ниже [разрешений](/graph/permissions-reference#calls-permissions). Эти разрешения должны предоставляться администратором.

| Сценарий                 | Разрешения                                  |
|:------------------------------------|:---------------------------------------------|
| Звонки                 | Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All |
| Собрания                 | OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All |
| Присутствие                 | Presence.Read, Presence.Read.All |
| Записи звонков             | CallRecords.Read.All |

## <a name="common-use-cases"></a>Основные варианты использования

В таблице ниже перечислены некоторые распространенные варианты использования API облачных коммуникаций.

| Варианты использования                         | Ресурсы REST                                 | См. также  |
|:------------------------------------|:---------------------------------------------|:----------|
| Создание приватных и групповых звонков, а также присоединение к ним   | [Звонок](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true)| [Методы звонков](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true#methods)|
|Звонки с интерактивным речевым взаимодействием   |     | [Методы для интерактивного речевого взаимодействия](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta?&preserve-view=true)
| Элементы управления звонком (участник) | [Участник](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true)   ||
|Собрания|[onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)| [Методы для собраний](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true#methods)|
|Присутствие | [presence](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) | [Методы для присутствия](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true#methods) |
| Получение записей звонков | [callRecord](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta&preserve-view=true) | [Подписки веб-перехватчиков](/graph/api/resources/webhooks?view=graph-rest-beta&preserve-view=true) |

## <a name="common-properties"></a>Общие свойства

| Ресурс                | Свойства                             |
|:------------------------------------|:---------------------------------------------|
| call                               | [свойства объекта call](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true#properties)  |
| participant                         | [свойства объекта participant](/graph/api/resources/participant?view=graph-rest-beta?view=graph-rest-v1.0&preserve-view=true#properties) |
| onlineMeeting                            | [свойства объекта onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true#properties)                     |
| presence | [свойства объекта presence](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true#properties) |
| callRecord | [Свойства callRecord](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta&preserve-view=true#properties) |

## <a name="whats-new"></a>Что нового
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="see-also"></a>См. также

- [Примеры API облачных коммуникаций](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [Пакет SDK для передачи сигналов коммуникаций](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [Пакет SDK мультимедиа коммуникаций](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)


