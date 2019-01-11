---
title: 'пользователь: exportPersonalData'
description: Отправляет запрос операции данные политики, внесенные администратором компании для экспорта данных организации пользователя.
localization_priority: Normal
ms.openlocfilehash: db20b0cb7eb11358298ce5b9fc59357a18fcb9be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869687"
---
# <a name="user-exportpersonaldata"></a>пользователь: exportPersonalData

Запрос данных политики операции от администратора компании или приложения для экспорта данных организации пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  User.Export.All User.Read.All  |
|Делегированные (личная учетная запись Майкрософт) |  Неприменимо  |
|Application | User.Export.All User.Read.All |

>**Примечание:** Экспорт может выполняться только администратором компании при использовании делегированы разрешения.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Authorization  | Bearer {token}|

## <a name="request-body"></a>Тело запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|storageLocation|Строка|Это URL-адрес подписи (SAS) общий доступ к учетной записи хранилища Azure, для которых следует экспортировать данные.|

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. Он не возвращает все действия в теле ответа. Ответ содержит следующие заголовки ответа.

| Имя       | Описание|
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
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a>Ответ

```
{
  Location: https://graph.microsoft.com/v1.0/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
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
