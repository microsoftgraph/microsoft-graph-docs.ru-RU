---
title: 'принтер: Create'
description: Создает (регистрирует) принтер с помощью универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1b36a856a73d78b479270138868285a852d6d187
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007196"
---
# <a name="printer-create"></a>принтер: Create

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте (Зарегистрируйте) принтер с помощью универсальной службы печати. Это длительно выполняемая операция, которая возвращает объект [принтеркреатеоператион](../resources/printercreateoperation.md) , который можно использовать для отслеживания и проверки регистрации принтера.

## <a name="permissions"></a>Разрешения
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированное (рабочая или учебная учетная запись)| User.Read.All |
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/create
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {token}. Required. |
| Content-Type  | application/json. Required.|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите объект JSON со следующими свойствами.

| Параметр      | Тип    |Описание| Обязательный? |
|:---------------|:--------|:----------|:----------|
|displayName|String|Отображаемое имя, присваиваемое принтеру.|Да|
|manufacturer|String|Производитель принтера.|Да|
|model|String|Модель принтера.|Да|
|фисикалдевицеид|String|UUID физического устройства принтера. Является обязательным, если `hasPhysicalDevice` свойство имеет значение true.|Нет|
|хасфисикалдевице|Boolean|True, если принтер имеет физическое устройство вывода, в противном случае — значение false. Если этот параметр опущен, значение по умолчанию — true.|Нет|
|цертификатесигнингрекуест|[принтцертификатесигнингрекуест](../resources/printcertificatesigningrequest.md)|Запрос подписи сертификата X. 509 (CSR) для сертификата, созданного и используемого принтером для идентификации.|Да|
|коннекторид|String|Идентификатор соединителя, который выступает в качестве прокси-сервера для принтера.|Нет|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и ссылку на связанный [принтеркреатеоператион](../resources/printercreateoperation.md) в `Operation-Location` заголовке.

Чтобы получить состояние текущей регистрации принтера, можно использовать запрос GET к связанному URL-адресу. После успешного завершения регистрации принтера запрос GET к связанному URL-адресу будет содержать созданный объект Printer и зарегистрированный сертификат.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса. Для получения справки по созданию необходимого запроса подписи сертификата (CSR) обратитесь к [образцу кода создания CSR](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).

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
