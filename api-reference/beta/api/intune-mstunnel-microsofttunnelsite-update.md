---
title: Обновление microsoftTunnelSite
description: Обновление свойств объекта microsoftTunnelSite.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 840ca65d6cd612e2744569ca4ca3d99cc34b8b45
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342995"
---
# <a name="update-microsofttunnelsite"></a>Обновление microsoftTunnelSite

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
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
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса устройте представление JSON для [объекта microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)

В следующей таблице показаны свойства, необходимые при создании [microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id MicrosoftTunnelSite|
|displayName|String|Имя отображения MicrosoftTunnelSite|
|description|Строка|Описание MicrosoftTunnelSite|
|publicAddress|Строка|Имя или IP-адрес общественного домена MicrosoftTunnelSite|
|upgradeWindowUtcOffsetInMinutes|Int32|Зона времени сайта, представленная в качестве минутного смещения от UTC|
|upgradeWindowStartTime|TimeOfDay|Время запуска окна обновления сайта|
|upgradeWindowEndTime|TimeOfDay|Время окончания дня окна обновления сайта|
|upgradeAutomatically|Boolean|Параметр автоматического обновления сайта. True для автоматических обновлений, false для ручного управления|
|upgradeAvailable|Boolean|True, если доступно обновление|
|internalNetworkProbeUrl|String|URL-адрес зонда внутреннего доступа к сети MicrosoftTunnelSite|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `200 OK` обновленный [объект microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
Content-type: application/json
Content-length: 524

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "upgradeWindowUtcOffsetInMinutes": 15,
  "upgradeWindowStartTime": "12:01:27.3030000",
  "upgradeWindowEndTime": "11:57:17.9830000",
  "upgradeAutomatically": true,
  "upgradeAvailable": true,
  "internalNetworkProbeUrl": "https://example.com/internalNetworkProbeUrl/",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 573

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "b2f7dc3e-dc3e-b2f7-3edc-f7b23edcf7b2",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "upgradeWindowUtcOffsetInMinutes": 15,
  "upgradeWindowStartTime": "12:01:27.3030000",
  "upgradeWindowEndTime": "11:57:17.9830000",
  "upgradeAutomatically": true,
  "upgradeAvailable": true,
  "internalNetworkProbeUrl": "https://example.com/internalNetworkProbeUrl/",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




