---
title: Использование API Microsoft Graph для интеграции функций социальной и рабочей аналитики в приложении
description: Microsoft Graph обеспечивает доступ к полезным социальным и рабочим данным для пользователей, а также поддерживает социальные жесты в социальном контексте пользователя.
localization_priority: Priority
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 74beb2a66f103342f6dbc5e5977200751a309c08
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450671"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-and-workplace-intelligence-in-an-app"></a>Использование API Microsoft Graph для интеграции функций социальной и рабочей аналитики в приложении

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph обеспечивает доступ к социальным и рабочим данным для пользователей, а также поддерживает жесты в социальном контексте пользователя.

## <a name="aggregate-and-extract-specific-information-about-people"></a>Сбор и извлечение определенных сведений о пользователях

Используйте ресурс [person](../resources/person.md) и API службы "Люди" для сбора сведений о пользователе, полученных из его почты, контактов и социальных сетей. Результаты упорядочиваются по релевантности на основании множества отношений общения, совместной работы и бизнес-связей. Вы можете просматривать, сортировать, отбирать, фильтровать или искать сведения о пользователях, основываясь на заданных условиях.

- [Получение списка людей](../api/user-list-people.md)

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a>Помогите пользователям получить наиболее важные документы для работы

Используйте API аналитики для определения наиболее важных документов для пользователя:

- Список [популярных документов](../api/insights-list-trending.md) пользователя
- Список документов, [используемых](../api/insights-list-used.md) пользователем
- Список документов, [к которым пользователю предоставлен доступ или к которым пользователь предоставил доступ](../api/insights-list-shared.md)

## <a name="help-users-gain-insights-into-their-work-patterns"></a>Помощь пользователям в получении аналитики рабочих закономерностей

Используйте API аналитики, чтобы получить статистику о действиях и соответствующие параметры для пользователя:

- [settings](../resources/settings.md). Чтобы API аналитики возвращал результаты для пользователя, в параметрах аналитики текущего пользователя должна отображаться действительная лицензия MyAnalytics, должно быть выбрано использование MyAnalytics и должен применяться облачный почтовый ящик с поддержкой Graph.
- [activityStatistics](../resources/activitystatistics.md). Получение данных за последнюю полную неделю (или указанный промежуток времени) для действий в Office 365, выполнявшихся пользователем, включая количество часов, потраченное на [звонки](callactivitystatistics.md), [чаты (мгновенные сообщения)](chatactivitystatistics.md), [письма](emailactivitystatistics.md) и [собрания](meetingactivitystatistics.md) в течение и вне рабочего времени, а также часы, доступные для [сосредоточенной работы](focusactivitystatistics.md).

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
