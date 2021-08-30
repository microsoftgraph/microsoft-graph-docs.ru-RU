---
author: swapnil1993
title: 'сайт: getApplicableContentTypesForList'
description: Получите типы контента сайта, которые можно добавить в список.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 94c19b98a01a16f655893661e7d368dc8a902114
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696727"
---
# <a name="site-getapplicablecontenttypesforlist"></a>сайт: getApplicableContentTypesForList
Пространство имен: microsoft.graph



Получите [контент][] [сайтаTypes,][contentType] который можно добавить в список.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/getApplicableContentTypesForList
```

## <a name="function-parameters"></a>Параметры функции
В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.
В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.

|Параметр|Тип|Описание|
|-|-|-|
|listId| String | GUID списка, для которого необходимо извлечь соответствующие типы контента. Обязательный элемент. |

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

Чтобы перечислить только настраиваемые типы контента, используйте `$filter=isBuiltin eq false` .

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы эта функция возвращает код ответа и `200 OK` [коллекцию contentType](../resources/contenttype.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "site_getapplicablecontenttypesforlist"
}
-->
```http
GET https://graph.microsoft.com/v1.0/sites/{siteId}/getApplicableContentTypesForList(listId='listId')
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType",
  "isCollection": true
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
        "id":"0x",
        "description":"",
        "group":"_Hidden",
        "hidden":false,
        "name":"System",
        "base": {
            "name": "System",
            "id": "0x"
        }
    },
    {
        "id":"0x00A7470EADF4194E2E9ED1031B61DA0884",
        "name": "docSet",
        "description": "custom docset",
        "hidden":false,
        "base": {
            "name": "Document Set",
            "id": "0x0120D520"
        },
        "group": "Custom Content Types"
    }
  ]
}
```

[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
