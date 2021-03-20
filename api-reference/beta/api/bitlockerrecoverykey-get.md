---
title: Get bitlockerRecoveryKey
description: Извлечение свойств и связей объекта bitlockerRecoveryKey.
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d55f1889a8134196760b133827bee2ec8c82b20e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944423"
---
# <a name="get-bitlockerrecoverykey"></a>Get bitlockerRecoveryKey
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение свойств и связей [объекта bitlockerRecoveryKey.](../resources/bitlockerrecoverykey.md) 

По умолчанию эта операция не возвращает ключевое **свойство,** которое представляет фактический ключ восстановления. Чтобы включить **ключевое** свойство в ответ, используйте параметр `$select` запроса OData. В том числе параметр запроса запускает аудит Azure AD операции и `$select` создает журнал аудита. Журнал аудита [Azure AD](/azure/active-directory/reports-monitoring/concept-audit-logs) можно найти в категории KeyManagement.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|BitLocker.ReadBasic.All, BitLocker.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Не поддерживается|

>**Примечание:** Для делегирования разрешений, позволяющих приложениям получать ресурсы BitLockerRecoveryKey от имени подписанного пользователя, администратор клиента должен назначить пользователю одну из следующих ролей, либо пользователь должен быть зарегистрированным владельцем устройства, на которое изначально был подписан ключ BitLocker:  
* Глобальный администратор
* Администратор облачных устройств
* Администратор службы поддержки
* администратор службы Intune;
* Администратор безопасности
* Читатель безопасности
* Глобальный читатель

## <a name="http-request"></a>HTTP-запрос
Чтобы получить указанный ключ BitLocker без возврата свойства **ключа:**
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'
```

Чтобы получить указанный ключ BitLocker, включая его **ключевое** свойство:
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'?$select=key
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметр `$select` запроса OData для возврата **свойства ключа.** Подробные сведения [см. в примере 2](#example-2). Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|ocp-client-name|Имя клиентского приложения, которое выполняет вызов API. Обязательный.|
|ocp-client-version|Версия клиентского приложения с вызовом API. Обязательно.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) в теле ответа.

## <a name="examples"></a>Примеры

### <a name="example-1"></a>Пример 1
Получите ключ BitLocker, указав **ключевой id.** В этом примере свойство **ключа не** возвращается.

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey_3"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
Ниже приведен пример ответа.

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

### <a name="example-2"></a>Пример 2
Получите ключ BitLocker с **свойством ключа,** указав **ключевой id.**

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey_4"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4?$select=key
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
Ниже приведен пример ответа.

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
