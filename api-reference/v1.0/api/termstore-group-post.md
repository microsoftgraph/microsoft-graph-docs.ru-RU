---
title: Создание группы
description: Создание нового группового объекта в магазине терминов.
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: ff08b50016ff40065ec09c462f6f14bd6d8face4
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60947453"
---
# <a name="create-termstore-group"></a>Создание группы termStore
Пространство имен: microsoft.graph.termStore

Создание нового [группового](../resources/termstore-group.md) объекта в магазине терминов.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись) |TermStore.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST sites/{site-id}/termStore/groups
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте описание объекта [group](../resources/termstore-group.md) в формате JSON.

В следующей таблице показаны свойства, необходимые при создании [группового](../resources/termstore-group.md) объекта.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя создаемой группы.|



## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и `201 Created` [объект Microsoft.graph.termStore.group](../resources/termstore-group.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "displayName": "myGroup"
}-->

``` http
POST https://graph.microsoft.com/v1.0/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/groups
Content-Type: application/json

{
  "displayName" : "myGroup"
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
}-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "85825593-5593-8582-9355-828593558285",
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "displayName": "myGroup"  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Create termGroup",
  "suppressions": [
  ]
}
-->


