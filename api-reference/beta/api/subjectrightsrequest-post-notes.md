---
title: Создание authoredNote
description: Создание нового объекта authoredNote.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 811e0063b44e942aaeb13cf4069780b4635636d9
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60447047"
---
# <a name="create-authorednote"></a>Создание authoredNote
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [объекта authoredNote.](../resources/authorednote.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|SubjectRightsRequest.ReadWrite.All*|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается|

>[!IMPORTANT]
>Разрешения, отмеченные звездочкой (*), в настоящее время недоступны. Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues#compliance).

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [authoredNote.](../resources/authorednote.md)

В следующей таблице показаны свойства, необходимые при создании [authoredNote.](../resources/authorednote.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|content|[microsoft.graph.itemBody](../resources/itembody.md)|Содержимое заметки для запроса|


## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект authoredNote](../resources/authorednote.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_authorednote_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
Content-Type: application/json
Content-length: 203

{
"content": 
  {
    "content": "String",
    "contentType": "text"
  }
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authoredNote"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "String (identifier)",
    "createdDateTime": "String (timestamp)",
    "author": { "@odata.type": "microsoft.graph.identitySet"},
    "content": {
          "@odata.type": "microsoft.graph.itemBody"
    }

}
```

