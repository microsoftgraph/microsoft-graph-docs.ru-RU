---
title: Настройка ответов на административный поиск для пользователей в организации (предварительный просмотр)
description: Microsoft Search позволяет администраторам связывать термины поиска со значениями или веб-страницами, определенными для их организаций, и включать эти ассоциации в качестве ответов на поиск.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 542f1c3dc3d280ba72c3c64d032c19594c6bc29c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337915"
---
# <a name="set-up-administrative-search-answers-for-users-in-an-organization-preview"></a>Настройка ответов на административный поиск для пользователей в организации (предварительный просмотр)

Microsoft Search позволяет администраторам связывать термины поиска со значениями или веб-страницами, определенными для их организаций, и включать эти ассоциации в качестве ответов на поиск. Например, пользователи в организации могут иметь незнакомую аббревиатуру, представляюную внутреннее имя проекта, или имя команды, связанное с веб-страницей группы. Администраторы могут настроить аббревиатуры [, закладки](/microsoftsearch/manage-acronyms) или [QnA](/microsoftsearch/manage-qas) в центре администрирования [Microsoft 365](https://admin.microsoft.com/) в поисковой &**.**[](/microsoftsearch/manage-bookmarks) Это позволяет пользователям использовать поиск для навигации и ознакомления с их работой.

Администраторы также могут использовать API поиска в Microsoft Graph для программного управления ответами на административный поиск в организации. Эти ответы отображаются в результатах поиска Майкрософт, когда срабатывает аббревиатура или ключевое слово, определенное в доступных типах ресурсов ответов [поиска:](/graph/api/resources/search-acronym) аббревиатуре [,](/graph/api/resources/search-bookmark) закладке и [ресурсах QnA](/graph/api/resources/search-qna) .

При запуске определенной аббревиатуры или ключевого слова эти ответы поиска будут отображаться в верхней части страницы результатов поиска в организации.

## <a name="example-create-a-new-acronym"></a>Пример. Создание новой аббревиатуры

В следующем запросе создается новая аббревиатура, которая будет отображаться на странице результатов поиска при поиске пользователем.

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

## <a name="example-create-a-new-bookmark"></a>Пример: создание новой закладки

В следующем запросе создается новая закладка, которая будет отображаться на странице результатов поиска при поиске по крайней мере одного из ключевых слов пользователя.

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
- Ознакомьтесь со сценариями и возможностями [API поиска: обзор API поиска Майкрософт](/graph/search-concept-overview).
- Узнайте больше об API поиска в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- [Управление ответами на административный поиск](search-concept-answers.md).
