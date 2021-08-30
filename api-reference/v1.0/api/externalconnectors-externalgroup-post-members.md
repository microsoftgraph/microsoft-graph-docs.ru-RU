---
title: Создание удостоверений
description: Создание нового участника в качестве ресурса удостоверений в externalGroup.
author: sacampbe
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 42ac3ef6dd3aa12d1116c09694c74957c34077e3
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697547"
---
# <a name="create-identity"></a>Создание удостоверений
Пространство имен: microsoft.graph.externalConnectors



Создание ресурса [удостоверений](../resources/externalconnectors-identity.md) для нового участника в [externalGroup.](../resources/externalconnectors-externalgroup.md)

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
POST /connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем JSON-представление объекта **удостоверений.**

Следующие свойства можно указать при создании ресурса **удостоверений** для участника **в externalGroup.**

| Свойство       | Тип                    | Описание                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| id             | String                  | Уникальный `id` член. Это будет **objectId** в случае Azure Active Directory пользователей или групп и **externalGroupId** в случае внешних групп. Обязательное.                                    |
| type           | microsoft.graph.externalConnectors.identityType | Тип участника, добавленного во внешнюю группу. Возможные значения: `user` , `group` , `externalGroup` . Обязательный. |


## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` объект **удостоверения** в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a>Пример 1. Добавление Azure Active Directory пользователя в качестве участника

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_aad_user_identity_from_group"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user"
}
```

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.identity"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user"
}
```

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a>Пример 2. Добавление Azure Active Directory группы в качестве участника

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_aad_group_identity_from_group"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group"
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.identity"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group"
}
```

### <a name="example-3-add-another-external-group-as-a-member"></a>Пример 3. Добавление другой внешней группы в качестве участника

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_external_group_identity_from_group"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "1431b9c38ee647f6a",
  "type": "externalGroup",
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.identity"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "14m1b9c38qe647f6a",
  "type": "externalGroup"
}
```
