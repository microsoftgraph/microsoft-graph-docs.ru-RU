---
title: Настройка ответов административного поиска для пользователей в организации (предварительная версия)
description: Поиск (Майкрософт) позволяет администраторам связывать поисковые термины со значениями или веб-страницами, относясь к их организациям, и включать их в качестве ответов на поиск.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: ffc0e35f351a0841b8905c73454d1461f7fb7013
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446107"
---
# <a name="set-up-administrative-search-answers-for-users-in-an-organization-preview"></a>Настройка ответов административного поиска для пользователей в организации (предварительная версия)

Поиск (Майкрософт) позволяет администраторам связывать условия поиска со значениями или веб-страницами, которые относятся к их организациям, и включать эти связи в качестве ответов на поиск. Например, пользователи в организации могут получить незнакомую акроним, представляющую внутреннее имя проекта, или имя команды, связанное с веб-страницей группы. Администраторы могут [настраивать](/microsoftsearch/manage-acronyms) аббревиатуры [,](/microsoftsearch/manage-bookmarks) закладки или [QnA](/microsoftsearch/manage-qas) в [](https://admin.microsoft.com/)Центр администрирования Microsoft 365 в разделе поиска & **аналитики**. Это позволяет пользователям использовать поиск для навигации и ознакомления с работой.

Администраторы также могут использовать API поиска (Майкрософт) в Microsoft Graph для программного управления ответами административного [поиска в организации](/graph/api/resources/search-api-answers-overview) . Эти ответы отображаются в результатах поиска (Майкрософт) при активации с помощью аббревиатуры или ключевого слова, определенного в доступных типах ресурсов ответов [поиска:](/graph/api/resources/search-acronym) акроним [,](/graph/api/resources/search-bookmark) закладка и ресурсы [QnA](/graph/api/resources/search-qna) .

При активации с помощью определенного аббревиатуры или ключевого слова эти ответы поиска отображаются в верхней части страницы результатов поиска в организации.

## <a name="example-1-create-a-new-acronym"></a>Пример 1. Создание нового акронима

Следующий запрос создает новый акроним, который будет отображаться на странице результатов поиска при поиске пользователем.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_acronym_from_acronyms"
}-->
```http
POST https://graph.microsoft.com/beta/search/acronyms
Content-Type: application/json

{
  "displayName": "GDPR",
  "standsFor": "General Data Protection Regulation",
  "description": "A European Union (EU) regulation on data protection and privacy in the EU and the European Economic Area (EEA) that enhances individuals' control and rights over their personal data, simplifies the regulatory environment for international business, and addresses the transfer of personal data outside the EU and EEA areas.",
  "webUrl": "http://contoso.com/GDPR",
  "state": "published"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.acronym"
}-->
```http
HTTP/1.1 200 Ok
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

## <a name="example-2-create-a-new-bookmark"></a>Пример 2. Создание новой закладки

Следующий запрос создает новую закладку, которая будет отображаться на странице результатов поиска, когда пользователь выполняет поиск по крайней мере одного из ключевых слов.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_bookmark_from_bookmarks"
}-->
```http
POST https://graph.microsoft.com/beta/search/bookmarks
Content-Type: application/json

{
  "displayName": "Contoso Install Site",
  "webUrl": "http://www.contoso.com/",
  "description": "Try or buy Contoso for Home or Business and view product information",
  "keywords":  {
    "keywords": ["Contoso", "install"],
    "reservedKeywords": ["Contoso"],
    "matchSimilarKeywords": true
  },
  "state": "published"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.bookmark"
}-->
```http
HTTP/1.1 201 CREATED
Location: /733b26d5-af76-4eea-ac69-1a0ce8716897
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

## <a name="next-steps"></a>Дальнейшие действия

- Ознакомьтесь со сценариями и возможностями API поиска: [обзор API поиска (Майкрософт).](/graph/search-concept-overview)
- Узнайте больше об API поиска в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- [Используйте API поиска (Майкрософт) для управления ответами администратора](/graph/api/resources/search-api-answers-overview).
