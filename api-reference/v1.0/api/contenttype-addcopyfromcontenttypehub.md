---
title: 'contentType: addCopyFromContentTypeHub'
description: Добавьте или синхронизируйте копию опубликованного типа контента из концентратора типов контента на целевой сайт или список.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: c19aa0813e8bf7a5fa59fd87e9023a1ea605318c
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191882"
---
# <a name="contenttype-addcopyfromcontenttypehub"></a>contentType: addCopyFromContentTypeHub
Пространство имен: microsoft.graph

Добавьте или синхронизируйте копию опубликованного типа контента из концентратора типов контента на целевой [сайт](../resources/site.md) или [список](../resources/list.md).

Этот метод является частью изменений в типе публикации контента, чтобы оптимизировать синхронизацию опубликованных типов контента с сайтами и списками, эффективно переходя от "принудительного везде" к "извлечению по мере необходимости". Этот метод позволяет пользователям извлекать типы контента непосредственно из центра типов контента на сайт или в список. Дополнительные сведения см. в разделе [contentType: getCompatibleHubContentTypes](contenttype-getcompatiblehubcontenttypes.md) и записи блога о обновлениях продукта [Syntex — август 2021 г](https://techcommunity.microsoft.com/t5/sharepoint-syntex-blog/syntex-product-updates-august-2021/ba-p/2606438).

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
В тексте запроса добавьте представление параметров в формате JSON.

В следующей таблице показан параметр, который можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|contentTypeId|Строка| Идентификатор типа контента в центре типов контента, который будет добавлен на целевой сайт или в список.|



## <a name="response"></a>Ответ

`200 OK` В случае успешного выполнения это действие возвращает код отклика и объект [contentType](../resources/contenttype.md) `202 Accepted` в тексте ответа, если тип контента добавляется синхронно, или код ответа, если тип контента будет синхронно синхронизирован. Ответ также будет содержать `Location` заголовок, содержащий расположение [объекта richLongRunningOperation](../resources/richlongrunningoperation.md) , созданного для обработки операции копирования и синхронизации. В случае асинхронной операции синхронизация или добавление типа контента может занять до 70 минут.

## <a name="examples"></a>Примеры

### <a name="example-1-synchronous-pull"></a>Пример 1. Синхронное извлечение

В следующем примере тип контента добавляется или синхронно синхронизируется на основе определенных внутренних условий.

#### <a name="request"></a>Запрос

Ниже приведен пример синхронной операции.

<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/sites/root/lists/Documents/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "0x0101"
}
```

#### <a name="response"></a>Ответ

Ниже приведен пример отклика.

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
    "@odata.type": "#microsoft.graph.contentType",
    "id": "0x0101",
    "description": "Document content type",
    "group": "Document Content Types",
    "hidden": false,
    "isBuiltIn": true,
    "name": "Document"
}
```

### <a name="example-2-asynchronous-pull"></a>Пример 2. Асинхронное извлечение

В следующем примере тип контента добавляется или синхронно синхронно, так как внутренние условия синхронной операции не выполняются.

#### <a name="request"></a>Запрос

Ниже приведен пример асинхронной операции.

<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/sites/root/lists/Documents/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "0x0101"
}
```


#### <a name="response"></a>Ответ

Ниже приведен пример отклика.

<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 202 Accepted
location: https://graph.microsoft.com/v1.0/sites/root/lists/Documents/operations/contentTypeCopy,0x0101
```
