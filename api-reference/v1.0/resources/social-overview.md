---
title: Интегрирование аналитики о людях в приложение с помощью Microsoft Graph API
description: Microsoft Graph позволяет получить доступ к полезным сведениям о людях и документах, с которыми они взаимодействуют.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 983ca1e7b11e488cec38abc2b54c7e241d4a0719
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353898"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-intelligence-in-an-app"></a>Интегрирование аналитики о людях в приложение с помощью Microsoft Graph API

Microsoft Graph позволяет получить доступ к полезным сведениям о людях и документах, с которыми они взаимодействуют.

## <a name="aggregate-and-extract-specific-information-about-people"></a>Сбор и извлечение определенных сведений о пользователях

Функция: люди

Можно использовать ресурс [person](../resources/person.md) и API службы "Люди" для сбора сведений о пользователе, полученных из его почты, контактов и социальных сетей. Результаты упорядочиваются по релевантности на основании множества шаблонов общения и совместной работы, а также его бизнес-связями. Вы можете просматривать, сортировать, отбирать, фильтровать или искать сведения о пользователях, основываясь на заданных условиях.

Со сценариями и примерами можно ознакомиться в статье [Получение сведений о релевантных людях](/graph/people-example).

Чтобы использовать API, ознакомьтесь со следующими материалами:

- [Получение списка людей](../api/user-list-people.md)


## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a>Помощь пользователям в получении наиболее важных документов для работы

Функция: аналитика на основе документов

Используйте API аналитики для определения наиболее важных документов для пользователя:

- Список [популярных документов](../api/insights-list-trending.md) пользователя
- Список документов, [используемых](../api/insights-list-used.md) пользователем
- Список документов, [к которым пользователю предоставлен доступ или к которым пользователь предоставил доступ](../api/insights-list-shared.md)

## <a name="whats-new"></a>Что нового
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.