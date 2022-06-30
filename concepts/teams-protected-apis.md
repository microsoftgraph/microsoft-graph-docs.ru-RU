---
title: Защищенные API в Microsoft Teams
description: API-интерфейсы Microsoft Teams в Microsoft Graph, которые получают доступ к конфиденциальным данным, считаются защищенными API-интерфейсами и требуют дополнительной проверки, прежде чем вы сможете их использовать.
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 8f9387d33d440a7ac8d90fc9be9e671b790c9e17
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556299"
---
# <a name="protected-apis-in-microsoft-teams"></a>Защищенные API в Microsoft Teams

API Microsoft Teams в Microsoft Graph, получающие доступ к конфиденциальным данным, считается защищенными API. Эти API требуют, чтобы у вас была дополнительная проверка помимо разрешений и согласия, прежде чем вы сможете их использовать.

Сейчас защищены следующие API, и все они используют [разрешения приложения Microsoft Graph](auth/auth-concepts.md#microsoft-graph-permissions):

* [Перечисление сообщений в каналах](/graph/api/channel-list-messages)
* [Получить chatMessages в дельте канала](/graph/api/chatmessage-delta)
* [Получить сообщение канала](/graph/api/chatmessage-get)
* [Создать подписку на новые сообщения канала](/graph/api/subscription-post-subscriptions)
* [Перечисление ответов на сообщение](/graph/api/chatmessage-list-replies)
* [Получение ответа на сообщение](/graph/api/chatmessage-get)
* (Список чатов не существует, с защищенным доступом к API или без него)
* [Список сообщений в чате](/graph/api/chat-list-messages)
* [Получение сообщения в чате](/graph/api/chatmessage-get)
* [Создать подписку на новые сообщения чата](/graph/api/subscription-post-subscriptions)
* [Список всего размещенного содержимого](/graph/api/chatmessage-list-hostedcontents)
* [Получить размещенное содержимое](/graph/api/chatmessagehostedcontent-get)

> [!NOTE]
> [Отправка сообщения](/graph/api/channel-post-messages) не является защищенным API.

## <a name="request-access-to-protected-apis"></a>Запросить доступ к защищенным API

Чтобы запросить доступ к этим защищенным API, заполните следующую [форму запроса](https://forms.office.com/r/v3qjyzBCxD). Обычно мы проверяем запросы на доступ каждую среду и развертываем утверждения каждую пятницу или понедельник, за исключением основных праздничных недель. Заявки в течение этих недель обрабатываются на следующей непраздничной неделе.

Чтобы проверить, утвержден ли ваш запрос, протестируйте доступ к приложению в следующий понедельник. Если у нас возникнут дополнительные вопросы о запросе, мы свяжемся по электронной почте, указанной в форме.

## <a name="see-also"></a>См. также

* [Обзор API Microsoft Teams](teams-concept-overview.md)