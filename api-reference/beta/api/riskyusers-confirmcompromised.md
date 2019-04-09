---
title: Подтверждение riskyUsers скомпрометированных атак
description: Подтвердите, что объект riskyUsers скомпрометирован.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: beca64415a2d03898d57cd9cda2fb248121c424b
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2019
ms.locfileid: "31559977"
---
# <a name="confirm-riskyusers-compromised"></a>Подтверждение riskyUsers скомпрометированных атак

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>**Примечание:** Для API riskyUsers требуется лицензия Azure AD Premium P2.

Подтвердите, что объект [рискюсер](../resources/riskyuser.md) скомпрометирован. При этом уровень риска целевого пользователя будет установлен в значение High (высокий).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Идентитирискюсер. ReadWrite. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Идентитирискюсер. ReadWrite. ALL |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Workbook-Session-Id  | Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.|

## <a name="request-body"></a>Текст запроса
Укажите идентификаторы пользователя, которые нужно отклонить в теле запроса.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
