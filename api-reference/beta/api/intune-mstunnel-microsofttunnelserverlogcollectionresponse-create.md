---
title: Создание microsoftTunnelServerLogCollectionResponse
description: Создайте новый объект microsoftTunnelServerLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 68015691c2d5f3c40f8a5cb98003c330b7a3365a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864853"
---
# <a name="create-microsofttunnelserverlogcollectionresponse"></a>Создание microsoftTunnelServerLogCollectionResponse

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте [новый объект microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложения|MicrosoftTunnelGateway.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelServerLogCollectionResponses
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта microsoftTunnelServerLogCollectionResponse.

В следующей таблице показаны свойства, необходимые при создании microsoftTunnelServerLogCollectionResponse.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный ID объекта|
|status|[microsoftTunnelLogCollectionStatus](../resources/intune-mstunnel-microsofttunnellogcollectionstatus.md)|Состояние коллекции журналов. Возможные значения: `pending`, `completed`, `failed`.|
|startDateTime|DateTimeOffset|Время начала собранных журналов |
|endDateTime|DateTimeOffset|Время окончания собранных журналов|
|sizeInBytes|Int64|Размер журналов в bytes|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `201 Created` [объект microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelServerLogCollectionResponses
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "status": "completed",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "sizeInBytes": 11
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "id": "05dcc2e9-c2e9-05dc-e9c2-dc05e9c2dc05",
  "status": "completed",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "sizeInBytes": 11
}
```




