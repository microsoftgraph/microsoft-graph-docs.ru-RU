---
title: ПереЧисление сайтов
description: ПереЧислите доступные [сайты] [] в Организации, которые совпадают с предоставленными критериями фильтра и параметрами запроса.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0bcf6023779178ea2c5d8e6ccb24adafad4bb7d7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330123"
---
# <a name="enumerate-sites"></a>ПереЧисление сайтов

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список доступных [сайтов][] в Организации, которые отвечают предоставленным условиям фильтра и параметрам запроса.

В настоящее время поддерживаются только следующие параметры запросов:

| Оператор Filter             | Оператор SELECT        | Описание
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | ПереЧисление всех семейств сайтов корневого уровня в Организации. Полезен для обнаружения домашнего сайта для каждого из географических регионов.

Кроме того, вы можете использовать **[поисковый][]** запрос в семействе "" "" "" "" "" "" "" "" "" "" "

[выполнять]: site-search.md
[сайтов]: ../resources/site.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)
|:--------------------------------------|:-------------------------------------
|Делегированные (рабочая или учебная учетная запись)     | Sites.Read.All, Sites.ReadWrite.All
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.
|Для приложений                            | Sites.Read.All, Sites.ReadWrite.All

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a>Пример

#### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": []
}
-->
