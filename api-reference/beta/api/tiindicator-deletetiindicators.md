---
title: 'Тииндикатор: Делететииндикаторс'
description: Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 49475f15520f02cc36bb1bf37af9a5849a8ee245
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544679"
---
# <a name="tiindicator-deletetiindicators"></a>Тииндикатор: Делететииндикаторс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | ThreatIndicators.ReadWrite.OwnedBy |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | ThreatIndicators.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {code} |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|значение|Коллекция строк| Коллекция Тииндикатор `id`s, которую необходимо удалить. |

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод `200, OK` возвращает код отклика и объект коллекции [ресултинфо](../resources/resultinfo.md) в тексте отклика.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicators"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators
Content-type: application/json

{
  "value": [
    "id-value1",
    "id-value2"
  ]
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

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
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
