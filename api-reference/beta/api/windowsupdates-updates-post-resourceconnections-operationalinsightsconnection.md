---
title: Создание operationalInsightsConnection
description: Создайте объект operationalInsightsConnection.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 85990438cec500e8c7f45c08ee1fe907f1f97efc
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856813"
---
# <a name="create-operationalinsightsconnection"></a>Создание operationalInsightsConnection
Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|WindowsUpdates.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|WindowsUpdates.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/resourceConnections
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) в формате JSON.

При создании **operationalInsightsConnection** необходимо указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|azureResourceGroupName|Строка|Имя группы ресурсов Azure, содержащего рабочую область Log Analytics.|
|azureSubscriptionId|String|Идентификатор подписки Azure, содержащий рабочую область Log Analytics.|
|workspaceName|Строка|Имя рабочей области Log Analytics.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) в тексте отклика.

Возможны следующие ошибки:

|Код ответа|Сообщение|
|:---|:---|
|`400 Bad Request`|Не удалось связать указанную рабочую область. Убедитесь, что свойства ключа верны.|
|`403 Forbidden`|Не удалось связать указанную рабочую область. Убедитесь, что подписка Azure активна.|
|`409 Conflict`|Указанный ресурс уже существует.|

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_operationalInsightsConnection_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/resourceConnections
Content-Type: application/json
Content-length: 97

{
  "@odata.type": "#microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "azureSubscriptionId": "322ec614-e9c2-4cd5-a55c-5711fdecf02e",
  "azureResourceGroupName": "target-resource-group",
  "workspaceName": "my-workspace"
}
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.operationalInsightsConnection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "id": "85fbecb2-e407-34e9-9298-4d587857795d",
  "azureSubscriptionId": "322ec614-e9c2-4cd5-a55c-5711fdecf02e",
  "azureResourceGroupName": "target-resource-group",
  "workspaceName": "my-workspace",
  "state": "connected"
}
```