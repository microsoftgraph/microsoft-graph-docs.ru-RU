---
title: Создание Микрософттуннелконфигуратион
description: Создание нового объекта Микрософттуннелконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa74bc55c739cc7ef8ad735538e9a948cfc2a2a4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242352"
---
# <a name="create-microsofttunnelconfiguration"></a>Создание Микрософттуннелконфигуратион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelConfigurations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Микрософттуннелконфигуратион в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Микрософттуннелконфигуратион.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор Микрософттуннелконфигуратион|
|displayName|String|Отображаемое имя Микрософттуннелконфигуратион|
|description|String|Описание Микрософттуннелконфигуратион|
|сетью|String|Подсеть, которая будет использоваться для выделения виртуального адреса для клиентов.|
|днссерверс|Коллекция строк|DNS-серверы, которые будут использоваться клиентами;|
|дефаултдомаинсуффикс|String|Приложение домена по умолчанию, которое будет использоваться клиентами.|
|раутесинклуде|Коллекция строк|Маршрутизации, которые будут маршрутизироваться сервером|
|раутесексклуде|Коллекция строк|Подмножества маршрутов, которые не будут маршрутизироваться сервером|
|сплитднс|Коллекция строк|Домены, которые будут разрешены с помощью предоставленных DNS-серверов|
|листенпорт|Int32|Порт, прослушиваемый портами TCP и UPD на сервере|
|адванцедсеттингс|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Дополнительные параметры, которые могут быть применены к серверу|
|lastUpdateDateTime|DateTimeOffset|При последнем обновлении Микрософттуннелконфигуратион|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations
Content-type: application/json
Content-length: 748

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 797

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "id": "b8bdb469-b469-b8bd-69b4-bdb869b4bdb8",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




