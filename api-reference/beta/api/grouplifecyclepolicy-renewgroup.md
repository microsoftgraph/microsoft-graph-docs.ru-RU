---
title: 'groupLifecyclePolicy: renewGroup'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
ms.openlocfilehash: 5472927769175912736f66a2d848f103cfb5b8c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833322"
---
# <a name="grouplifecyclepolicy-renewgroup"></a>groupLifecyclePolicy: renewGroup

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.

> **Примечание:** В версии 1.0, [Используйте группы ресурсов следует обновить запросы](/graph/api/group-renew?view=graph-rest-1.0).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).
 

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.ReadWrite.All или Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается |
|Для приложения | Group.ReadWrite.All или Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---------------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json |

## <a name="request-body"></a>Тело запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр | Тип | Описание |
|:---------------|:--------|:----------|
|groupId|GUID| Идентификатор группы для обновления. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
