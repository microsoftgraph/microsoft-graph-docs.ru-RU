---
title: Набор обновлений
description: Обновление свойств объекта набора.
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: b36db1756c104ddc41a2483b3403f04c989b61b3
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58515026"
---
# <a name="update-set"></a>Набор обновлений
Пространство имен: microsoft.graph.termStore

Обновление свойств объекта [набора.](../resources/termstore-set.md)

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
PATCH sites/{site-id}/termStore/sets/{set-id}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса устроим представление JSON [установленного](../resources/termstore-set.md) объекта.

В следующей таблице показаны свойства, которые можно изменить для за [наборного](../resources/termstore-set.md) объекта.

|Свойство|Тип|Описание|
|:---|:---|:---|
|локализованные имена|[коллекция microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md)|Имя набора.|
|description|Строка|Описание набора.|
|properties|[коллекция microsoft.graph.keyValue](../resources/keyvalue.md)|Свойства набора.|



## <a name="response"></a>Отклик

В случае успешного решения этот метод возвращает код отклика и обновленный `200 OK` [объект microsoft.graph.termStore.set](../resources/termstore-set.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_set"
} -->

``` http
PATCH https://graph.microsoft.com/v1.0/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/sets/3607e9f9-e9f9-3607-f9e9-0736f9e90736
Content-Type: application/json
Content-length: 288

{
  "description": "mySet"
}
```

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
  "description": "mySet",    
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update termSet",
  "suppressions": [
  ]
}
-->


