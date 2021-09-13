---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be1dd5ec3764925ecdf073a1c86cd329908a77b7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022179"
---
# <a name="update-devicecategory"></a>Обновление объекта deviceCategory

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceCategory](../resources/intune-devices-devicecategory.md).

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-devices-devicecategory.md) в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-devices-devicecategory.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор категории устройства. Только для чтения.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-devices-devicecategory.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.deviceCategory"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8"
}
```




