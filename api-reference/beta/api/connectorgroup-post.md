---
title: Создание connectorGroup
description: Создание объекта connectorGroup.
ms.localizationpriority: medium
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 04d04de3ff3cf01e9c97e0cbc06c509bb6e5c128
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60934704"
---
# <a name="create-connectorgroup"></a>Создание connectorGroup

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание объекта [connectorGroup.](../resources/connectorgroup.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-request-headers"></a>Необязательные заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Носителер. Обязательный параметр.|
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [connectorGroup.](../resources/connectorgroup.md)
В следующей таблице перечислены свойства, доступные для **connectorGroup.** Свойство **name** — обязательное свойство.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|connectorGroupType|string| Указывает тип гибридного агента. Это свойство заранее заданной системой.|
|id|string| Уникальный идентификатор для этого соединитетеляGroup. Только для чтения. |
|isDefault|логический| Указывает, является ли соединительщикGroup по умолчанию. Соединительщиком по умолчанию может быть только одна группа соединительных групп, и это заранее заданной системой. |
|name|string| Имя, связанное с соединитетелемGroup. |
|регион|string| Регион, в который назначен connectorGroup, и будет оптимизировать трафик. Этот регион можно установить только в **том** случае, если соединители или приложения не назначены соединительгруппе. Доступные регионы: Северная Америка, Европа, Австралия, Азия и Индия. Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` объект [connectorGroup](../resources/connectorgroup.md) в тексте ответа.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup_1"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
Content-type: application/json

{
  "name": "Connector Group Demo"

}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectorgroup-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectorgroup-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectorgroup-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connectorgroup-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
  "name": "Connector Group Demo",
  "connectorGroupType": "applicationProxy",
  "isDefault": true,
  "region": "nam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



