---
title: Защищенные API в Microsoft Teams
description: API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 393fcba98a893c9de7b2453281516aa1f1a41065aa2b9a3e106db4dad81937e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192203"
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

Если вы хотите предоставить информацию в дополнение к форме, обратитесь по адресу [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).
