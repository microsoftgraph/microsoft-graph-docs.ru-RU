---
title: 'contentType: addCopyFromContentTypeHub'
description: Добавьте или синхронизируйте копию опубликованного типа контента из концентратора типов контента на целевой сайт или список.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 39b147c1c75b535962eaa70d4120304b4e4634ca
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162332"
---
# <a name="contenttype-addcopyfromcontenttypehub"></a>contentType: addCopyFromContentTypeHub
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавьте или синхронизируйте копию опубликованного типа контента из концентратора типов контента на целевой [сайт](../resources/site.md) или [список.](../resources/list.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись) | Sites.Manage.All, Sites.FullControl.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Sites.Manage.All, Sites.FullControl.All |


## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
POST /sites/{siteId}/contentTypes/addCopyFromContentTypeHub
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON параметров.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|contentTypeId|Строка| ID типа контента в концентраторе типа контента, который должен быть добавлен на целевой сайт или список.|



## <a name="response"></a>Отклик

В случае успеха это действие возвращает код отклика и объект contentType в тексте ответа, если тип контента добавляется синхронно, или код ответа, если тип контента синхронно синхронизирован. `200 OK` [](../resources/contenttype.md) `202 Accepted` В ответе также будет содержаться загон, содержащий расположение `Location` [richLongRunningOperation,](../resources/richLongRunningOperation.md) созданного для обработки копирования и синхронизации. В случае асинхронной операции синхронизация или добавление типа контента может занять до 70 минут.

## <a name="examples"></a>Примеры

### <a name="example-1-synchronous-pull"></a>Пример 1. Синхронная тяга

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "String"
}
```


#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.contentType",
    "id": "String (identifier)",
    "description": "String",
    "group": "String",
    "hidden": "Boolean",
    "isBuiltIn": "Boolean",
    "name": "String"
  }
}
```
### <a name="example-2-asynchronous-pull"></a>Пример 2. Асинхронная тяга

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "String"
}
```


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 202 Accepted
location: https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/operations/{operationId}
```
