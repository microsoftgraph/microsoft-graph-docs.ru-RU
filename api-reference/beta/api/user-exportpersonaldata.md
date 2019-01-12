---
title: 'пользователь: exportPersonalData'
description: Отправляет запрос операции данные политики, внесенные администратором компании для экспорта данных организации пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7f112d065b75da7dc525e667df78b0264be37d55
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934193"
---
# <a name="user-exportpersonaldata"></a>пользователь: exportPersonalData

Отправляет запрос операции данные политики, сделанных с администратора компании для экспорта данных организации пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  User.Export.All и User.Read.All  |
|Делегированные (личная учетная запись Майкрософт) |  Неприменимо  |
|Application | User.Export.All и User.Read.All |

>**Примечание:** Экспорт может выполняться только администратором компании при использовании делегированных разрешений.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание |
|:---------------|:----------|
| Authorization  | Bearer {token}|

## <a name="request-body"></a>Тело запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание |
|:---------------|:--------|:----------|
|storageLocation|Строка|Это URL-адрес подписи (SAS) общий доступ к учетной записи хранилища Azure, для которых следует экспортировать данные.|

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. Он не возвращает все действия в теле ответа. Ответ содержит следующие заголовки.

| Имя       | Описание |
|:---------------|:----------|
| Расположение  | URL-адрес, чтобы проверить состояние запроса. |
| Повтор после  | Период времени в секундах. Лиц, ответственных за запрос должен ожидать это время после отправки запроса для проверки состояния. |


## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a>Ответ

```
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
