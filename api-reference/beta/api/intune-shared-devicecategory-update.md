---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 248bb5627243bc9724f54e46e36cce593a18bd05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980388"
---
# <a name="update-devicecategory"></a>Обновление объекта deviceCategory

Пространство имен: microsoft.graph

> **Важно!** API в версии/Beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).

## <a name="prerequisites"></a>Предварительные условия

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)||
| &nbsp;&nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp; &nbsp; **Адаптация** | DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений||
| &nbsp;&nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp; &nbsp; **Адаптация** | DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

**Управление устройствами**

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

**Встроенное подключение**

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a>Заголовки запросов

|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса

В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор категории устройства. Только для чтения.|
|**Адаптация**|
|description|String|Необязательное описание категории устройств.|
|displayName|String|Отображаемое имя категории устройств.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведено несколько примеров запроса.

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Представленный здесь объект отклика может быть усечен для краткости. Свойства ответа будут зависеть от контекста.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```












