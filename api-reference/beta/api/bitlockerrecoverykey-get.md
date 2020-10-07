---
title: Получение Битлоккеррековерикэй
description: Получение свойств и связей объекта Битлоккеррековерикэй.
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5652a3ae5c2f0a5a02ea5ea193b06ffd6ab98257
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372378"
---
# <a name="get-bitlockerrecoverykey"></a>Получение Битлоккеррековерикэй
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств и связей объекта [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) . 

По умолчанию эта операция не возвращает свойство **Key** , представляющее фактический ключ восстановления. Чтобы включить свойство **Key** в ответ, используйте `$select` параметр запроса OData. Включение `$select` параметра запроса инициирует аудит Azure AD для операции и создает журнал аудита. Журнал [аудита Azure AD](/azure/active-directory/reports-monitoring/concept-audit-logs) можно найти в категории кэйманажемент.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|BitLocker. ReadBasic. ALL, BitLocker. Read. ALL|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Не поддерживается|

>**Примечание:** Для делегированных разрешений, позволяющих приложениям получать ресурсы Битлоккеррековерикэй от имени вошедшего пользователя, администратору клиента должен быть назначен один из следующих ролей, либо пользователь должен быть **зарегистрированным владельцем** устройства, с которого была создана резервная копия ключа BitLocker: 
* глобальный администратор;
* Администратор облачных устройств
* Администратор службы поддержки
* администратор службы Intune;
* Администратор безопасности
* Читатель безопасности
* Глобальный читатель

## <a name="http-request"></a>HTTP-запрос
Чтобы получить указанный ключ BitLocker, не возвращая свойство **Key** :
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'
```

Получение указанного ключа BitLocker, включая его свойство **ключа** :
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'?$select=key
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает `$select` параметр запроса OData для возврата свойства **Key** . Подробнее: [Пример 2](#example-2). Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|OCP — имя клиента|Имя клиентского приложения, выполняющего вызов API. Обязательное.|
|OCP — Client – Version|Версия клиентского приложения, выполняющего вызов API. Обязательно.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1"></a>Пример 1
Получите ключ BitLocker, указав **идентификатор ключа**. В этом примере не возвращается свойство **Key** .

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "2020-06-15T13:45:30.0000000Z",
    "volumeType": 1,
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
  }
}
```

### <a name="example-2"></a>Пример 2
Получите ключ BitLocker с помощью **ключевого** свойства, указав **идентификатор ключа**.

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4?$select=key
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "String (timestamp)",
    "volumeType": 1,
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
    "key": "123456-231453-873456-213546-654678-765689-123456-324565"
  }
}
```
