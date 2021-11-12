---
title: Создание набора
description: Создайте новый объект набора.
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: 781cca8fce8b83b00be65cc1063cd290318bbd55
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60940260"
---
# <a name="create-set"></a>Создание набора
Пространство имен: microsoft.graph.termStore

Создайте новый [объект набора.](../resources/termstore-set.md)

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
POST sites/{site-id}/termStore/sets
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса устроим представление JSON [установленного](../resources/termstore-set.md) объекта.

В следующей таблице показаны свойства, необходимые при создании [задатки](../resources/termstore-set.md) объекта.

|Свойство|Тип|Описание|
|:---|:---|:---|
|локализованные имена|[коллекция microsoft.graph.termstore.localizedName](../resources/termstore-localizedname.md)|Имя создаемого набора.|
|parentGroup|[microsoft.graph.termstore.group](../resources/termstore-group.md)|termstore-group, в которой необходимо создать набор.|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект microsoft.graph.termStore.set](../resources/termstore-set.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
``` http
POST https://graph.microsoft.com/v1.0/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/sets
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.termStore.set",
  "parentGroup":{
      "id": "fc733b51-10f1-40fd-b784-dc6d1e42804b"
   },
   "localizedNames" : [
      {
        "languageTag" : "en-US",
        "name" : "Department"
      }
  ]
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termstore.set"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
  "localizedNames" : [
      {
        "languageTag" : "en-US",
        "name" : "Department"
      }
  ]
}
```


[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Create termSet",
  "suppressions": [
  ]
}
-->


