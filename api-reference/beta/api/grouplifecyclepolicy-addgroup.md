---
title: 'groupLifecyclePolicy: addGroup'
description: Добавляет группу к политике жизненного цикла.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8deeafa852b69af919fb79b43acaa5b588bdcd35
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316701"
---
# <a name="grouplifecyclepolicy-addgroup"></a>groupLifecyclePolicy: addGroup

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавляет определенные группы в политику жизненного цикла. Это действие ограничивает политику жизненного цикла группы набором групп только в том случае, если установлено свойство **managedGroupTypes** [groupLifecyclePolicy.](../resources/grouplifecyclepolicy.md) `Selected`

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается |
|Для приложений | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---------------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр | Тип | Описание |
|:---------------|:--------|:----------|
|groupId|String| Идентификатор группы, добавляемой в политику. |

Когда **установлено свойство managedGroupTypes** [groupLifecyclePolicy,](../resources/grouplifecyclepolicy.md) в список можно добавить до `Selected` 500 групп. Если вам нужно добавить более 500 групп, необходимо установить свойство **managedGroupTypes** [groupLifecyclePolicy.](../resources/grouplifecyclepolicy.md) `All`

На каждый запрос можно добавить только одну группу.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK`. Если группа добавлена в политику, в теле ответа возвращается `true` значение. В противном `false` случае в теле ответа возвращается значение.

## <a name="example"></a>Пример

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a>Отклик
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


