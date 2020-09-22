---
title: Создание Екстерналграуп
description: Создание нового объекта Екстерналграуп.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: fb836591b86972144f3ff632f807f7e1d4c0e82c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193952"
---
# <a name="create-externalgroup"></a>Создание Екстерналграуп

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [екстерналграуп](../resources/externalgroup.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке убывания привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается                               |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                               |
| Приложение                            | ExternalItem.ReadWrite.All                  |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionId}/groups
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [екстерналграуп](../resources/externalgroup.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [екстерналграуп](../resources/externalgroup.md).

| Свойство    | Тип   | Описание                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | Уникальный идентификатор внешней группы в подключении. Он должен состоять из буквенно-цифровых символов и иметь длину до 128 символов. |
| displayName | String | Понятное имя внешней группы. Необязательно.                                                                      |
| description | String | Описание внешней группы. Необязательный параметр.                                                                         |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [екстерналграуп](../resources/externalgroup.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_connection"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroup"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
