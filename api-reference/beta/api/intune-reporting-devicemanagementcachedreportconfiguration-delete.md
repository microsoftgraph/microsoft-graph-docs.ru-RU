---
title: Удаление Девицеманажементкачедрепортконфигуратион
description: Удаляет объект Девицеманажементкачедрепортконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e726e9eb66c7af6480bf6077203ba096970c364e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472335"
---
# <a name="delete-devicemanagementcachedreportconfiguration"></a>Удаление Девицеманажементкачедрепортконфигуратион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Удаляет объект [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

### <a name="response"></a>Ответ
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 204 No Content
```



