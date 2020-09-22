---
title: Создание отношения
description: Создание объекта связи.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8008abbfa10bbc0c7267384c66afc7c7c1c1c328
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055724"
---
# <a name="create-relation"></a>Создание отношения
Пространство имен: Microsoft. Graph. банка

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание объекта [связи](../resources/termstore-relation.md) . Они используются для создания закрепленных и ресуед связей между терминами или между термином и набором. При создании закрепленного/повторно используемого термина между термином и set значение Фромтерм в тексте POST должно иметь значение null.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
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
POST /termStore/sets/{setId}/terms/{termId}/relations
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [relation](../resources/termstore-relation.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [отношения](../resources/termstore-relation.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|Отношение|релатионтипе|Тип создаваемого отношения. Возможные значения: `pin`, `reuse`.|
|set| [Microsoft. Graph. банка. Set](../resources/termstore-set.md)| Набор, в котором необходимо создать связь.
|фромтерм| [Microsoft. Graph. Банк. Term](../resources/termstore-term.md) | Термин, с которым необходимо создать связь.



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [relation](../resources/termstore-relation.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

``` http
POST https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}/relations
Content-Type: application/json
Content-length: 89

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
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termstore.relation"
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


