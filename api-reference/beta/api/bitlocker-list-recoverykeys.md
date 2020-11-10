---
title: Список Рековерикэйс
description: Получение списка объектов Битлоккеррековерикэй и их свойств.
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 865e44cf6c8d696ed4da549bad05d50229e29601
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961304"
---
# <a name="list-recoverykeys"></a>Список Рековерикэйс
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) и их свойств. 

Эта операция не возвращает свойство **Key** . Сведения о том, как прочитать свойство **Key** , можно найти в статье [Get битлоккеррековерикэй](bitlockerrecoverykey-get.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|BitLocker. ReadBasic. ALL, BitLocker. Read. ALL|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложения|Не поддерживается|

>**Примечание**. для делегированных разрешений, чтобы разрешить приложениям получать ресурсы битлоккеррековерикэй от имени вошедшего пользователя, администратору клиента должен быть назначен один из следующих ролей, либо пользователь должен быть зарегистрированным владельцем устройства, для которого была создана резервная копия ключа восстановления BitLocker: 
* Глобальный администратор
* Администратор облачных устройств
* Администратор службы поддержки
* администратор службы Intune;
* Администратор безопасности
* Читатель безопасности
* Глобальный читатель

## <a name="http-request"></a>HTTP-запрос
Чтобы получить список ключей BitLocker в клиенте, выполните следующие действия:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys
```

Чтобы получить список ключей BitLocker в клиенте, отфильтрованном по **идентификатору устройства** :

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys?$filter=deviceId eq '{deviceId}'
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает `$filter` параметр запроса OData для фильтрации результатов по **идентификатору устройства** , в которое было Последнее резервное копирование. Подробнее: [Пример 2](#example-2). Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

Ответ также может содержать объект `odata.nextLink` , который можно использовать для отображения результатов в наборе результатов. Дополнительные сведения см в разделе [разбиение данных Microsoft Graph](/graph/paging).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|OCP — имя клиента|Имя клиентского приложения, выполняющего вызов API. Обязательный.|
|OCP — Client – Version|Версия клиентского приложения, выполняющего вызов API. Обязательно.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1"></a>Пример 1
Получение списка ключей BitLocker в клиенте.

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys
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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
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
      "volumeType": 1,
      "deviceId": "2ef04ef1-23b0-2e00-a3a5-ab345e567ab6"
    },
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "6a30ed7b-247b-4d26-86b5-2f405e55ea42",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
### <a name="example-2"></a>Пример 2
Получение списка ключей BitLocker, отфильтрованных по **идентификатору устройства**.

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleIds": ["1ab40ab2-32a8-4b00-b6b5-ba724e407de9"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys?$filter=deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'
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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
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
      "volumeType": 1,
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
