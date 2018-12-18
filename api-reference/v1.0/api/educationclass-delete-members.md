---
title: Удаление учащегося
description: Удаляет educationUser из educationClass.
author: mmast-msft
ms.openlocfilehash: a887b3286a0c9cbdbb7d12f0bdaa26131332346f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303817"
---
# <a name="remove-a-student"></a>Удаление учащегося

Удаляет [educationUser](../resources/educationuser.md) из [educationClass](../resources/educationclass.md).

>**Примечание.** Преподаватели _и_ учащиеся включены в коллекцию **members** курса. Перед вызовом этого API нужно проверить, не представляет ли удаляемый объект **educationUser** преподавателя.  Для этого необходимо получить список преподавателей путем вызова [educationclass_list_teachers](educationclass-list-teachers.md) и проверить, не возвращается ли в этом списке ИД удаляемого пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Не поддерживается.  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | EduRoster.ReadWrite.All | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.


## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/{member-id}
```

##### <a name="response"></a>Ответ
Ниже приведен пример ответа. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
