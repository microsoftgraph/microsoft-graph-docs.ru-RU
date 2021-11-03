---
title: Get bitlockerRecoveryKey
description: Извлечение свойств и связей объекта bitlockerRecoveryKey.
author: hafowler
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 557333d36b9a61243dddb844148a81e31b19bddd
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695876"
---
# <a name="get-bitlockerrecoverykey"></a>Get bitlockerRecoveryKey
Пространство имен: microsoft.graph

Извлечение свойств и связей [объекта bitlockerRecoveryKey.](../resources/bitlockerrecoverykey.md) 

По умолчанию эта операция не возвращает ключевое **свойство,** которое представляет фактический ключ восстановления. Чтобы включить **ключевое** свойство в ответ, используйте параметр `$select` запроса OData. В том числе параметр запроса запускает аудит Azure AD операции и `$select` создает журнал аудита. Дополнительные сведения о журналах аудита для ключей восстановления bitlocker см. в фильтре категорий KeyManagement журналов аудита [Azure AD.](/azure/active-directory/reports-monitoring/concept-audit-logs)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|BitLockerKey.ReadBasic.All, BitLockerKey.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Не поддерживается|

Для делегирования разрешений вызывающее пользователь должен быть зарегистрированным владельцем устройства, на которое изначально был восстановлен ключ восстановления BitLocker, или он должен быть в одной из следующих ролей [каталога:](/azure/active-directory/roles/permissions-reference)
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
GET /informationProtection/bitlocker/recoveryKeys/{bitlockeryRecoveryKeyId}
```

Чтобы получить указанный ключ BitLocker, включая его **ключевое** свойство:
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/{bitlockeryRecoveryKeyId}?$select=key
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметр `$select` запроса OData для возврата **свойства ключа.** Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|ocp-client-name|Имя клиентского приложения, которое выполняет вызов API. Этот загон используется для отладки. Необязательный параметр.|
|ocp-client-version|Версия клиентского приложения с вызовом API. Этот загон используется для отладки. Необязательный параметр.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) в теле ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-get-the-bitlocker-key-by-specifying-the-key-id"></a>Пример 1. Получить ключ BitLocker, указав ключевой id

#### <a name="request"></a>Запрос
Ниже приведен пример запроса. В этом примере свойство **ключа не** возвращается.

<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```

#### <a name="response"></a>Отклик
Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
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
    "volumeType": "1",
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
  }
}
```

### <a name="example-2-get-the-bitlocker-key-with-the-key-property"></a>Пример 2. Получить ключ BitLocker с **свойством ключа**

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey_key"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4?$select=key
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
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
    "volumeType": "1",
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
    "key": "123456-231453-873456-213546-654678-765689-123456-324565"
  }
}
```
