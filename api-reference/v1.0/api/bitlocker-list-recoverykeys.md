---
title: Список recoveryKeys
description: Получите список объектов bitlockerRecoveryKey и их свойств.
author: hafowler
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2a530fafd42226e607aef7d9a325176fa85212e5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688182"
---
# <a name="list-recoverykeys"></a>Список recoveryKeys

Пространство имен: microsoft.graph

Получите список объектов [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) и их свойств. 

Эта операция не возвращает свойство **ключа.** Сведения о том, как читать **свойство ключей,** см. в материале [Get bitlockerRecoveryKey.](bitlockerrecoverykey-get.md)

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

Чтобы получить список ключей BitLocker в клиенте:

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /informationProtection/bitlocker/recoveryKeys
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметр запроса OData для фильтрации результатов с помощью deviceId устройства, на которое был недавно основан `$filter` ключ.  Этот метод не поддерживает `$top` . Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

В ответе также может содержаться страница, которую можно использовать для страницы `odata.nextLink` с помощью набора результатов. Подробные сведения см. [в материале Paging Microsoft Graph данных.](/graph/paging)

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|ocp-client-name|Имя клиентского приложения, которое выполняет вызов API. Этот загон используется для отладки. Необязательный параметр.|
|ocp-client-version|Версия клиентского приложения с вызовом API. Этот загон используется для отладки. Необязательный параметр.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) в теле ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-retrieve-a-list-of-bitlocker-keys-in-the-tenant"></a>Пример 1. Извлечение списка ключей BitLocker в клиенте.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "list_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/informationProtection/bitlocker/recoveryKeys
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": "1",
      "deviceId": "2ef04ef1-23b0-2e00-a3a5-ab345e567ab6"
    },
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "6a30ed7b-247b-4d26-86b5-2f405e55ea42",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": "1",
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```

### <a name="example-2-retrieve-a-list-of-bitlocker-keys-filtered-by-deviceid"></a>Пример 2. Извлечение списка ключей BitLocker, фильтруемого deviceId.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "request",
  "name": "list_bitlockerrecoverykey_filter_deviceId"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/informationProtection/bitlocker/recoveryKeys?$filter=deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": "1",
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
