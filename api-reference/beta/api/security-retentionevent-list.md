---
title: Перечисление retentionEvents
description: Получение списка объектов retentionEvent и их свойств.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9357bc4668f0b275a4c69025063e2542b4156f40
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447827"
---
# <a name="list-retentionevents"></a>Перечисление retentionEvents
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [retentionEvent](../resources/security-retentionevent.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|RecordsManagement.Read.All, RecordsManagement.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|RecordsManagement.Read.All, RecordsManagement.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/triggers/retentionEvents
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры расширенного запроса OData для настройки ответа. Например, чтобы получить тип события, используйте `$expand=retentionEventType`. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения `200 OK` этот метод возвращает код отклика и коллекцию объектов [microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md)  в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "list_retentionevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/triggers/retentionEvents
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.retentionEvent)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.security.retentionEvent",
      "id": "fcdbfb58-d0c6-85dd-d011-4e0ff9a6805d",
      "displayName": "String",
      "description": "String",
      "eventQueries": [
        {
          "@odata.type": "microsoft.graph.security.eventQueries"
        }
      ],
      "eventTriggerDateTime": "String (timestamp)",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "String (timestamp)",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "eventPropagationResults": [
        {
          "@odata.type": "microsoft.graph.security.eventPropagationResult"
        }
      ],
      "eventStatus": {
        "@odata.type": "microsoft.graph.security.retentionEventStatus"
      },
      "lastStatusUpdateDateTime": "String (timestamp)"
    }
  ]
}
```
