---
title: Список сайтов
description: Выведите список всех доступных сайтов в организации или список сайтов, соответствующих указанным критериям фильтра и параметрам запроса.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: f78db6d9ad4d4b2f772ed79451ff16853a514d4e
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66578106"
---
# <a name="list-sites"></a>Список сайтов

Пространство имен: microsoft.graph

Вывод списка всех [доступных сайтов][] в организации.

Также поддерживаются определенные критерии фильтра и параметры запроса, которые описаны ниже.

| Оператор Filter             | Инструкция Select        | Описание
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | Выводит список всех семейств веб-сайтов корневого уровня в организации. Полезно для обнаружения домашнего сайта для каждого географического региона.

Кроме того, можно **[использовать запрос $search][]** к коллекции `/sites` , чтобы найти сайты, соответствующие заданным ключевым словам.

[$search]: site-search.md
[sites]: ../resources/site.md

Дополнительные рекомендации по созданию приложений, использующих обнаружение сайтов в целях сканирования, см. в разделе "Рекомендации по обнаружению файлов и обнаружению изменений [в большом масштабе"](/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="list-all-site-collections"></a>Вывод списка всех семейств веб-сайтов

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается.                              |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | Sites.Read.All, Sites.ReadWrite.All         |

### <a name="discover-the-home-site-for-each-geography"></a>Обнаружение домашнего сайта для каждого географического региона

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Sites.Read.All, Sites.ReadWrite.All         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | Sites.Read.All, Sites.ReadWrite.All         |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /sites
GET /sites?$filter=siteCollection/root ne null
```

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/sites?$select=siteCollection,webUrl&$filter=siteCollection/root%20ne%20null
```

### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Contoso USA",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso-jpn.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Contoso Japan",
      "root": { },
      "siteCollection": {
        "hostname": "contoso-jp.sharepoint.com",
        "dataLocationCode": "JPN",
        "root": { }
      },
      "webUrl": "https://contoso-jp.sharepoint.com"
    }
  ]
}
```

### <a name="request"></a>Запрос

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/sites
```

### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,bf6fb551-d508-4946-a439-b2a6154fc1d9,65a04b8b-1f44-442b-a1fc-9e5852fb946c",
      "name": "Root Site",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso.sharepoint.com,d9ecf079-9b13-4376-ac5d-f242dda55626,746dbcc1-fa2b-4120-b657-2670bae5bb6f",
      "name": "Site A",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com"
      },
      "webUrl": "https://contoso.sharepoint.com/sites/siteA"
    },
    {
      "id": "contoso.sharepoint.com,fd1a778f-263e-4c43-acdf-d5c2519d80eb,c06016db-dfec-4f79-83a1-09c6dbfd7022",
      "name": "Site B",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com"
      },
      "webUrl": "https://contoso.sharepoint.com/sites/siteB"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
  ]
}
-->


