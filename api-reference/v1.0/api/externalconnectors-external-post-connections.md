---
title: Создание externalConnection
description: Создайте новый объект externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d556b4925625ac929c1b13f6559c048de1b55366
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467441"
---
# <a name="create-externalconnection"></a>Создание externalConnection
Пространство имен: microsoft.graph.externalConnectors



Создайте новый объект externalConnection.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Неприменимо|
|Делегированные (личная учетная запись Майкрософт)|Неприменимо|
|Приложение| ExternalConnection.ReadWrite.OwnedBy|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /external/connections
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [externalConnection.](../resources/externalconnectors-externalconnection.md)

В следующей таблице показаны свойства, необходимые при создании [externalConnection.](../resources/externalconnectors-externalconnection.md)

|Свойство|Тип|Обязательно (Y/N) |Описание|
|:---|:---|:---|:---|
|id|String|Да|ID подключения|
|name|String|Да|Имя подключения|
|description|String|Да|Описание подключения|
|configuration|[microsoft.graph.externalConnectors.configuration](../resources/externalconnectors-configuration.md)|Нет|Конфигурации подключения|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект externalConnection](../resources/externalconnectors-externalconnection.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_externalconnection_from_connections"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/external/connections
Content-Type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system"
}
```


### <a name="response"></a>Отклик
Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
}
-->
``` http
HTTP/1.1 200 Created
Content-Type: application/json

{
  "id": "0a4f4e74-4e74-0a4f-744e-4f0a744e4f0a",
  "name": "String",
  "description": "String",
  "state": "ready",
  "configuration": {
    "authorizedAppIds": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

