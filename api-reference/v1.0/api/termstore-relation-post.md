---
title: Создание связи
description: Создайте новый объект связи.
author: vishriv
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 7e2c77a47f89eadf5140da215a0386917520f644
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/08/2022
ms.locfileid: "62443404"
---
# <a name="create-relation"></a>Создание связи
Пространство имен: microsoft.graph.termStore

Создайте новый [объект связи](../resources/termstore-relation.md) . Они используются для создания закрепленных и повторно используемых отношений между терминами или между термином и набором. Если между термином и набором создается закрепленный или повторно задаваемый термин, то в теле столба **необходимо установить null fromTerm**.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись) |TermStore.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |


## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST sites/{site-id}/termStore/sets/{set-id}/terms/{term-id}/relations
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляют представление JSON объекта [связи](../resources/termstore-relation.md) .

В следующей таблице показаны свойства, необходимые при создании объекта [связи](../resources/termstore-relation.md) .

|Свойство|Тип|Описание|
|:---|:---|:---|
|Отношение|microsoft.graph.termStore.relationType|Тип создаемого отношения. Возможные значения: `pin`, `reuse`.|
|set| [microsoft.graph.termStore.set](../resources/termstore-set.md)| Набор, в котором необходимо создать связь.|
|fromTerm| [microsoft.graph.termStore.term](../resources/termstore-term.md) | Термин, с которым необходимо создать отношения.|



## <a name="response"></a>Отклик

В случае успешного `201 Created` решения этот метод возвращает код ответа и [объект microsoft.graph.termStore.relation](../resources/termstore-relation.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_relation_from_"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/27fd2d26-60d3-485c-9420-0c71f74a0cfd/terms/8861b57a-c777-49e7-826f-47d6afecf80d/relations
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "relationship": "pin",
  "fromTerm" : {
    "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "set" : {
    "id": "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.relation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "052c749c-749c-052c-9c74-2c059c742c05",
  "relationship": "pin",
  "fromTerm" : {
      "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "toTerm" : {
      "id" : "226e8ee3-f4b6-49d7-92d5-ec9d5475eec5"
  },
  "set" : {
      "id" : "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md
[microsoft.graph.termStore.relation]: ../resources/termstore-relation.md


<!--
{
  "type": "#page.annotation",
  "description": "Create a pinned term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Pinned term",
  "suppressions": [
  ]
}
-->


