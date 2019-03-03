---
title: 'Тииндикатор: Делететииндикаторсбекстерналид'
description: Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов, а запрос содержит внешние идентификаторы, а не идентификаторы.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 82cdd0d9688e778982244a06a2a2e5d558d25807
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366947"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a>Тииндикатор: Делететииндикаторсбекстерналид

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе вместо нескольких запросов, если запрос содержит внешние идентификаторы, а не идентификаторы.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения  | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Среатиндикаторс. ReadWrite. Овнедби |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Среатиндикаторс. ReadWrite. Овнедби |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {code} |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|value|Коллекция строк| `externalIds` Коллекция объектов **тииндикатор** , которые необходимо удалить. |

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект коллекции [ресултинфо](../resources/resultinfo.md) в тексте отклика.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicatorsbyexternalid"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId
Content-type: application/json

{
  "value": [
    "externalId-value1",
    "externalId-value2"
  ]
}
```

### <a name="response"></a>Ответ

Ниже приведен пример ответа.

> [!NOTE]
> Объект Response, показанный здесь, может быть укорочен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "value": [
    {
      "code": "code-value",
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
