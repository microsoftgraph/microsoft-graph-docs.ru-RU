---
title: Update groupLifecyclePolicy
description: Обновляет свойства объекта groupLifecyclePolicyтип ресурса groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4f8379ac39ebd3b55fd6fc8528be14fc740c1ce8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941704"
---
# <a name="update-grouplifecyclepolicy"></a>Update groupLifecyclePolicy

Обновляет свойства объекта groupLifecyclePolicy[тип ресурса groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).

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
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a>Необязательные заголовки запросов
| Имя | Описание |
|:-----------|:-----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

В теле запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в тело запроса, остаются прежними или повторно вычисляются с учетом измененных значений других свойств. Для наилучших результатов не следует включать существующие значения, которые не изменились.

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|alternateNotificationEmails|String| Список адресов электронной почты для отправки уведомлений о группах без владельцев. Можно указать несколько адресов электронной почты, разделив их точкой с запятой. |
|groupLifetimeInDays|Int32| Количество дней до истечения срока действия группы. После продления группа будет оставаться активной в течение указанного количества дней. |
|managedGroupTypes|String| Тип группы, к которому применяется политика истечения срока действия. Возможные значения — **All**, **Selected** и **None**. |

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле ответа.
## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a>Отклик
Примечание. Представленный здесь объект отклика может быть усечен для краткости. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
