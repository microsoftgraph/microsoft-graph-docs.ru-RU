---
title: Защищенные API в Microsoft Teams
description: API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API.
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 03ad082f9bed728222f09c88de5d42b517f1fd2c
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687454"
---
# <a name="protected-apis-in-microsoft-teams"></a>Защищенные API в Microsoft Teams

API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API. Перед использованием этих API необходимо выполнить дополнительные проверки, кроме проверки разрешений и согласия.


В настоящий момент защищенными являются следующие API:
* [Перечисление сообщений в каналах](/graph/api/channel-list-messages) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Получение изменений для объектов chatMessages в канале](/graph/api/chatmessage-delta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Получение сообщений в каналах](/graph/api/chatmessage-get) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Создание подписки на новые сообщения в каналах](/graph/api/subscription-post-subscriptions) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Перечисление ответов на сообщение](/graph/api/chatmessage-list-replies) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Получение ответа на сообщение](/graph/api/chatmessage-get) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* (Перечисление чатов с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions) не существует, с доступом или без доступа через защищенные API)
* [Перечисление сообщений в чате](/graph/api/chat-list-messages) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Получение сообщения в чате](/graph/api/chatmessage-get) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Создание подписки на новые сообщения в чатах](/graph/api/subscription-post-subscriptions) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Перечисление всего размещенного содержимого](/graph/api/chatmessage-list-hostedcontents) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Получение размещенного содержимого](/graph/api/chatmessagehostedcontent-get) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)

>[!NOTE]
>[Отправка сообщения](/graph/api/channel-post-messages) не является защищенным API.

Чтобы запросить доступ к этим защищенным API, заполните следующую [форму запроса](https://aka.ms/teamsgraph/requestaccess). Мы проверяем запросы доступа каждую среду и развертываем утверждения каждую пятницу, кроме недель, на которые приходятся основные праздничные каникулы в США. Отправки в эти недели обрабатываются в следующую непраздничную неделю. 
