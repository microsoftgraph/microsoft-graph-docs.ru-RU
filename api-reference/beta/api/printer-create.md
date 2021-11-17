---
title: 'принтер: создание'
description: Создает (регистрирует) принтер со службой универсальной печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 328f4d1bb9ada8ceb99be79caa60a9683d15d368
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028096"
---
# <a name="printer-create"></a>принтер: создание

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте (зарегистрируйте) принтер с помощью службы универсальной печати. Это долгосрочная операция, и в качестве таковой возвращается [принтерCreateOperation,](../resources/printercreateoperation.md) который можно использовать для отслеживания и проверки регистрации принтера.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать. Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений| Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/create
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса укажи объект JSON следующими свойствами.

| Параметр      | Тип    |Описание| Обязательный? |
|:---------------|:--------|:----------|:----------|
|displayName|Строка|Имя отображения, которое необходимо назначить принтеру.|Да|
|manufacturer|String|Производитель принтера.|Да|
|model|String|Модель принтера.|Да|
|physicalDeviceId|Строка|UUID физического устройства принтера. Обязательно, если `hasPhysicalDevice` свойство является верным.|Нет|
|hasPhysicalDevice|Логический|True, если на принтере есть физическое выходное устройство, ложное в противном случае. Если значение опущено, значение по умолчанию является верным.|Нет|
|certificateSigningRequest|[printCertificateSigningRequest](../resources/printcertificatesigningrequest.md)|Запрос на подписание сертификата X.509 (CSR) для сертификата, созданного и используемой принтером для идентификации.|Да|
|connectorId|Строка|Id соединителя, выступая в качестве прокси-сервера для принтера.|Нет|

## <a name="response"></a>Отклик
В случае успешного использования этот метод возвращает код отклика и ссылку на связанный `202 Accepted` [принтерCreateOperation](../resources/printercreateoperation.md) в `Operation-Location` загонке.

Чтобы получить состояние текущей регистрации принтера, можно использовать запрос GET на связанный URL-адрес. После успешного завершения регистрации принтера запрос GET на связанный URL-адрес будет содержать созданный объект принтера и зарегистрированный сертификат.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/create
Content-type: application/json

{
  "displayName": "Test Printer",
  "manufacturer": "Test Printer Manufacturer",
  "model": "Test Printer Model",
  "physicalDeviceId": null,
  "hasPhysicalDevice": false,
  "certificateSigningRequest": { 
    "content": "{content}",
    "transportKey": "{sampleTransportKey}"
  },
  "connectorId": null
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-printer-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/beta/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printers: create",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
