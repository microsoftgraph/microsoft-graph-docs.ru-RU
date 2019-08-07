---
title: 'Используйте API Microsoft Graph для интеграции функций социальной и рабочей аналитики '
description: Microsoft Graph поддерживает социальные жесты в социальном контексте пользователя и предоставляет доступ к полезным сведениям о пользователях и к социальным данным.
localization_priority: Priority
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 84e0c82173dad6f08d5911f32ef5c384f041ea19
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008091"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-and-workplace-intelligence-in-an-app"></a>Используйте API Microsoft Graph для интеграции функций социальной и рабочей аналитики 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph поддерживает социальные жесты в социальном контексте пользователя и предоставляет доступ к полезным сведениям о пользователях и социальным данным.

## <a name="aggregate-and-extract-specific-information-about-people"></a>Сбор и извлечение определенных сведений о пользователях

Используйте ресурс [person](../resources/person.md) и API службы "Люди" для сбора сведений о пользователе, полученных из его почты, контактов и социальных сетей. Результаты упорядочиваются по релевантности на основании множества отношений общения, совместной работы и бизнес-связей. Вы можете просматривать, сортировать, отбирать, фильтровать или искать сведения о пользователях, основываясь на заданных условиях.

- [Получение списка людей](../api/user-list-people.md)

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a>Помогите пользователям получить наиболее важные документы для работы

Используйте API аналитики для определения наиболее важных документов для пользователя: 

- Список [популярных документов](../api/insights-list-trending.md) пользователя
- Список документов, [используемых](../api/insights-list-used.md) пользователем
- Список документов, [к которым пользователю предоставлен доступ или к которым пользователь предоставил доступ](../api/insights-list-shared.md)

## <a name="manage--mentions"></a>Управление @упоминаниями

Упоминание получателя в сообщении для уведомления и привлечения его внимания является распространенным социальным жестом.
Ресурс [mention](../resources/mention.md) и API упоминаний предоставляют простой механизм для упоминания получателя в [сообщении](../resources/message.md), получения всех сообщений, в которых пользователь отмечен с помощью @упоминания, или получения всех упоминаний в сообщении.

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- Создание упоминаний в новом сообщении

  - [Создание и отправка упоминаний в составе нового сообщения](../api/user-sendmail.md#request-2)
  - [Создание упоминания в составе черновика сообщения](../api/user-post-messages.md#request-2)

- Получение сведений об упоминаниях в сообщении

  - [Получение всех сообщений в почтовом ящике вошедшего пользователя, в которых упоминается пользователь](../api/user-list-messages.md#request-2)
  - [Получение сведений о каждом упоминании в сообщении](../api/message-get.md#request-2)

- [Удаление упоминания](../api/message-delete.md#request-2) в сообщении

