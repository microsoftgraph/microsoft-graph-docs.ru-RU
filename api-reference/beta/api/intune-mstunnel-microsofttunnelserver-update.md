---
title: Обновление microsoftTunnelServer
description: Обновление свойств объекта microsoftTunnelServer.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8e878a43325dcad36f615f8eefc41e74f6a85fd3
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864860"
---
# <a name="update-microsofttunnelserver"></a>Обновление microsoftTunnelServer

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)

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
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)

В следующей таблице показаны свойства, необходимые при создании [microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id MicrosoftTunnelServer|
|displayName|String|Имя отображения MicrosoftTunnelServer|
|tunnelServerHealthStatus|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|Состояние здоровья MicrosoftTunnelServer. Возможные значения: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.|
|lastCheckinDateTime|DateTimeOffset|При последней регистрации в MicrosoftTunnelServer|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект MicrosoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "id": "b5cf0aee-0aee-b5cf-ee0a-cfb5ee0acfb5",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```




