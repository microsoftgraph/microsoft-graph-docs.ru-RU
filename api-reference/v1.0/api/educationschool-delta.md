---
title: 'educationSchool: delta'
description: Создайте новые или обновленные школы, не выполняя полное чтение всей школьной коллекции.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3604a9296d7419d20e1b2b9016a2dc724b65c222
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232278"
---
# <a name="educationschool-delta"></a>educationSchool: delta

Пространство имен: microsoft.graph

Создайте новые или обновленные школы, не выполняя полное чтение всей школьной коллекции. Подробные [сведения см. в запросе Use Delta.](/graph/delta-query-overview)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | EduRoster.ReadBasic                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | EduRoster.Read.All, EduRoster.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/delta
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию educationSchool](../resources/educationschool.md) в тексте ответа. Отклик также содержит URL-адрес `nextLink` или `deltaLink`.

- Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных. Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.
- Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса. Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях в ресурсе в будущем.

Подробные сведения см. в [материале Использование запроса delta.](/graph/delta-query-overview) Например, запросы см. [в рублях Получить дополнительные изменения для пользователей.](/graph/delta-query-users)

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/schools/delta
```

### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationSchool)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationSchool)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/schools/delta?$skiptoken=VwhMSQw1l1O5v2F1ZPm...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSchool",
      "id": "String (identifier)",
      "displayName": "String",
      "description": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "principalEmail": "String",
      "principalName": "String",
      "externalPrincipalId": "String",
      "lowestGrade": "String",
      "highestGrade": "String",
      "schoolNumber": "String",
      "externalId": "String",
      "phone": "String",
      "fax": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress"
      }
    }
  ]
}
```
