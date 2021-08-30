---
title: Создание externalGroup
description: Создайте новый объект externalGroup.
author: sacampbe-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: bd7a09ae83540ab739bdda97fcdbfc14827a7e25
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697548"
---
# <a name="create-externalgroup"></a>Создание externalGroup
Пространство имен: microsoft.graph.externalConnectors



Создайте новый [объект externalGroup.](../resources/externalconnectors-externalgroup.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | Не поддерживается                               |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                               |
| Для приложений                            | ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All                  |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /connections/{connectionsId}/groups
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта **externalGroup.**

При создании externalGroup можно указать следующие **свойства.**

| Свойство    | Тип   | Описание                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | Уникальный ID внешней группы в подключении. Он должен быть альфа-числом и может иметь длину до 128 символов. Обязательный. |
| displayName | String | Дружеское имя внешней группы. Необязательный параметр.                                                                      |
| description | String | Описание внешней группы. Необязательный параметр.                                                                         |



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` **объект externalGroup** в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_connection"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups
Content-Type: application/json

{
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
