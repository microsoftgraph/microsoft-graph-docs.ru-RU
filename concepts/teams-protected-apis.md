---
title: Защищенные API в Microsoft Teams
description: API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: cf8f977d2a8d8e9e9704118718ac0c8da9b6ae77
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036321"
---
# <a name="protected-apis-in-microsoft-teams"></a>Защищенные API в Microsoft Teams

API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API. Перед использованием этих API необходимо выполнить дополнительные проверки, кроме проверки разрешений и согласия.

В настоящий момент защищенными являются следующие API:
* [Перечисление сообщений в каналах](/graph/api/channel-list-messages?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Получение сообщений в каналах](/graph/api/channel-get-message?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Перечисление ответов на сообщение](/graph/api/channel-list-messagereplies?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Получение ответа на сообщение](/graph/api/channel-get-messagereply?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Перечисление сообщений в чате](/graph/api/chatmessage-list?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)
* [Получение сообщения в чате](/graph/api/chatmessage-get?view=graph-rest-beta) с использованием [разрешений приложения](auth/auth-concepts.md#microsoft-graph-permissions)

>[!NOTE]
>[Отправка сообщения](/graph/api/channel-post-messages?view=graph-rest-beta) не является защищенным API.

Чтобы запросить доступ к этим защищенным API, заполните следующую [форму запроса](http://aka.ms/teamsgraph/requestaccess). Мы просматриваем запросы на доступ каждую среду и выпускаем утверждения каждую пятницу.
Если вы хотите предоставить информацию в дополнение к форме, обратитесь по адресу [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).
