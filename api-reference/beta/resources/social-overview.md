---
title: Интегрирование социальной аналитики в приложение с помощью Microsoft Graph API
description: Microsoft Graph поддерживает социальные жесты в социальном контексте пользователя и предоставляет доступ к полезным сведениям о пользователях и социальным данным.
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: 45482d2e47c97b6c09302ab60ff9c031cef1e92a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345718"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a>Интегрирование социальной аналитики в приложение с помощью Microsoft Graph API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph поддерживает социальные жесты в социальном контексте пользователя и предоставляет доступ к полезным сведениям о пользователях и социальным данным.

## <a name="aggregate-and-extract-specific-information-about-people"></a>Сбор и извлечение определенных сведений о пользователях

Используйте ресурс [person](../resources/person.md) и API службы "Люди" для сбора сведений о пользователе, полученных из его почты, контактов и социальных сетей. Результаты упорядочиваются по релевантности на основании множества отношений общения, совместной работы и бизнес-связей. Вы можете просматривать, сортировать, отбирать, фильтровать или искать сведения о пользователях, основываясь на заданных условиях.

- [Получение списка людей](../api/user-list-people.md)

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

## <a name="access-social-data-around-and-about-a-user"></a>Доступ к социальным данным о пользователе

Office Graph собирает отношения между различными объектами в Office 365. С помощью Office Graph можно получать социальную аналитику по отдельным пользователям в Office 365.

- Перечисление [популярных](../api/insights-list-trending.md) элементов, связанных с пользователем
- Перечисление пользователей, [работавших](../api/user-list-people.md) с пользователем
