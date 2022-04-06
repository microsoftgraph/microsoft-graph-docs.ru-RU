---
title: Защищенные API в Microsoft Teams
description: API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API.
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: f8c4fd35982d6fa36b49209255217989d121aac7
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516147"
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

Чтобы запросить доступ к этим защищенным API, заполните следующую [форму запроса](https://forms.office.com/r/v3qjyzBCxD). Обычно мы проверяем запросы доступа по средам и развертываем утверждения по пятницам и понедельникам, кроме недель, на которые приходятся важнейшие праздники в США. Запросы, отправленные в такие недели, будут обработаны в следующую непраздничную неделю. Чтобы проверить, утвержден ли ваш запрос, протестируйте доступ к приложению в следующий понедельник. Если у нас возникнут дополнительные вопросы о запросе, мы свяжемся по электронной почте, указанной в форме. 

