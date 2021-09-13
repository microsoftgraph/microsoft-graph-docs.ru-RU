---
title: Интегрирование аналитики о людях в приложение с помощью Microsoft Graph API
description: Microsoft Graph позволяет получить доступ к полезным сведениям о людях и документах, с которыми они взаимодействуют.
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 4d78275f1a2a7489233d49ce950cd349efe1dea9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032148"
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
