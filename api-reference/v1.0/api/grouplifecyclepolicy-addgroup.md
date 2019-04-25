---
title: 'groupLifecyclePolicy: addGroup'
description: Добавляет группу к политике жизненного цикла.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: dbd53bc24702cc1025a7546d8bd43058913ec184
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567419"
---
# <a name="grouplifecyclepolicy-addgroup"></a>groupLifecyclePolicy: addGroup

Добавляет группу к политике жизненного цикла.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
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
|groupId|GUID| Идентификатор группы, которую нужно добавить к политике. |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK`. Если к политике добавляется группа, в теле отклика возвращается значение **true**. Если нет, то в теле отклика возвращается значение **false**.

## <a name="example"></a>Пример

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/addGroup
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
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
