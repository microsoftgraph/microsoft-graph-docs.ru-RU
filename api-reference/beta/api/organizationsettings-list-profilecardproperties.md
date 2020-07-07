---
title: Список Профилекардпропертиес
description: Получение списка объектов профилекардпроперти.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4aa23e69308d8c13cc9ceb25bcc1398c9cbb1012
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051135"
---
# <a name="list-profilecardproperties"></a>Список Профилекардпропертиес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение коллекции ресурсов [профилекардпроперти](../resources/profilecardproperty.md) Организации. Каждый ресурс идентифицируется по свойству **директорипропертинаме** .

## <a name="permissions"></a>Разрешения

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | User. Read, User. Read. ALL                    |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | Не поддерживается.                              |

>**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль администратора клиента или роль глобального администратора.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает некоторые параметры запроса OData для настройки ответа. Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя          |Описание                  |
|:--------------|:----------------------------|
| Авторизация | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [профилекардпроперти](../resources/profilecardproperty.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "directoryPropertyName": "CustomAttribute1",
      "annotations": [
        {
          "displayName": "Cost Center",
          "localizations": [
            {
              "languageTag": "ru-RU",
              "displayName": "центр затрат"
            }
          ]
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List profileCardProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
