---
title: Создание схемы
description: Создайте схему для Поиск (Майкрософт) подключения.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 98c4c83ff8a8712905ace9fa80ec4fdae0de7180
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467493"
---
# <a name="create-schema"></a>Создание схемы
Пространство имен: microsoft.graph.externalConnectors



Создайте новый [объект схемы.](../resources/externalconnectors-schema.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Неприменимо|
|Делегированные (личная учетная запись Майкрософт)|Неприменимо|
|Приложение| ExternalConnection.ReadWrite.OwnedBy|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /external/connections/{id}/schema
```
В теле запроса поставляем представление JSON объекта [схемы.](../resources/externalconnectors-schema.md)

При регистрации настраиваемой схемы элементов объект должен иметь свойство, к котором должно быть установлено свойство, `schema` `baseType` и должен содержать `microsoft.graph.externalItem` `properties` его. Объект должен содержать по крайней мере одно свойство, не `properties` более 64.

## <a name="response"></a>Отклик

Если заготка включена в запрос, этот метод возвращает код ответа и URL-адрес в загонах ответа, которые можно использовать для получения состояния `Prefer: respond-async` `202 Accepted` `Location` [операции.](../api/externalconnectors-connectionoperation-get.md)

Без заголовка, включенного в запрос, в случае успешного использования этот метод возвращает код ответа и новый объект схемы в `Prefer: respond-async` `201 Created` тексте ответа. [](../resources/externalconnectors-schema.md)

> [!NOTE]
> Создание схемы — это длительный процесс, склонный к выходу времени шлюза. Рекомендуется использовать `Prefer: respond-async` заготку, чтобы избежать ошибок в периодике.

## <a name="examples"></a>Примеры

### <a name="example-register-custom-schema-asynchronously"></a>Пример. Регистрация настраиваемой схемы асинхронно

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async",
  "@odata.type": "microsoft.graph.externalConnectors.schema"
}-->

```http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```
