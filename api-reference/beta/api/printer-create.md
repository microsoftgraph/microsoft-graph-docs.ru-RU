---
title: 'принтер: Create'
description: Создает (регистрирует) принтер с помощью универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: bf100a99d573c186efa64af1692250534a31c50a
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674094"
---
# <a name="printer-create"></a>принтер: Create

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте (Зарегистрируйте) принтер с помощью универсальной службы печати. Это длительно выполняемая операция, которая возвращает объект [принтеркреатеоператион](../resources/printercreateoperation.md) , который можно использовать для отслеживания и проверки регистрации принтера.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать. Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| Printer. Create, Printer. ReadWrite. ALL, Printer. FullControl. ALL |
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
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите объект JSON со следующими свойствами.

| Параметр      | Тип    |Описание| Обязательный? |
|:---------------|:--------|:----------|:----------|
|displayName|String|Отображаемое имя, присваиваемое принтеру.|Да|
|manufacturer|String|Производитель принтера.|Да|
|model|String|Модель принтера.|Да|
|фисикалдевицеид|String|UUID физического устройства принтера. Является обязательным, если `hasPhysicalDevice` свойство имеет значение true.|Нет|
|хасфисикалдевице|Boolean|True, если принтер имеет физическое устройство вывода, в противном случае — значение false. Если этот параметр опущен, значение по умолчанию — true.|Нет|
|цертификатесигнингрекуест|[printCertificateSigningRequest](../resources/printcertificatesigningrequest.md)|Запрос подписи сертификата X. 509 (CSR) для сертификата, созданного и используемого принтером для идентификации.|Да|
|коннекторид|String|Идентификатор соединителя, который выступает в качестве прокси-сервера для принтера.|Нет|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и ссылку на связанный [принтеркреатеоператион](../resources/printercreateoperation.md) в `Operation-Location` заголовке.

Чтобы получить состояние текущей регистрации принтера, можно использовать запрос GET к связанному URL-адресу. После успешного завершения регистрации принтера запрос GET к связанному URL-адресу будет содержать созданный объект Printer и зарегистрированный сертификат.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса. Для получения справки по созданию необходимого запроса подписи сертификата (CSR) обратитесь к [образцу кода создания CSR](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/create
Content-type: application/json
Content-length: 319

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
