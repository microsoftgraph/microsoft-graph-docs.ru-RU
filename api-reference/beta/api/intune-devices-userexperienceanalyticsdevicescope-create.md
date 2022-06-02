---
title: Создание объекта userExperienceAnalyticsDeviceScope
description: Создайте объект userExperienceAnalyticsDeviceScope.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edca6bf2c5a88a17ea155510ac8a5fb0e1c07d2a
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857997"
---
# <a name="create-userexperienceanalyticsdevicescope"></a>Создание объекта userExperienceAnalyticsDeviceScope

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте объект [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceScopes
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта userExperienceAnalyticsDeviceScope в формате JSON.

В следующей таблице показаны свойства, необходимые при создании объекта userExperienceAnalyticsDeviceScope.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для конфигурации области устройства.|
|deviceScopeName|Строка|Имя конфигурации области устройства аналитики пользовательского интерфейса.|
|ownerId|Строка|Уникальный идентификатор пользователя (администратора), создавшего конфигурацию области устройства.|
|isBuiltIn|Boolean|Указывает, является ли конфигурация области устройства встроенной или пользовательской. Если значение равно TRUE, конфигурация области устройства является встроенной. Если значение равно FALSE, конфигурация области устройства является настраиваемой. Значение по умолчанию — FALSE.|
|enabled|Boolean|Указывает, включена или отключена область устройства. Если значение равно TRUE, область устройства включена. Если значение равно FALSE, область устройства отключена. Значение по умолчанию — FALSE.|
|status|[deviceScopeStatus](../resources/intune-devices-devicescopestatus.md)|Указывает состояние области устройства после включения области устройства. Возможные значения: none, computing, insufficientData или completed. Значение по умолчанию — none. Возможные значения: `none`, `computing`, `insufficientData`, `completed`, `unknownFutureValue`.|
|параметр|[deviceScopeParameter](../resources/intune-devices-devicescopeparameter.md)|Параметр конфигурации области устройства. В будущем он будет расширен для добавления дополнительных параметров. Например, параметр области устройства может быть версией ОС, типом диска, производителем устройства, моделью устройства или тегом области. Значение по умолчанию: scopeTag. Возможные значения: `none`, `scopeTag`, `unknownFutureValue`.|
|operator|[deviceScopeOperator](../resources/intune-devices-devicescopeoperator.md)|Оператор запроса конфигурации области устройства. Возможные значения: equals, notEquals, contains, notContains, greaterThan, lessThan. Значение по умолчанию: равно. Возможные значения: `none`, `equals`, `unknownFutureValue`.|
|valueObjectId|Строка|Уникальный идентификатор идентификатора тега области пользовательского устройства, используемого для создания конфигурации области устройства.|
|value|String|Значение предложения запроса конфигурации области устройства.|
|createdDateTime|DateTimeOffset|Указывает дату и время создания пользовательской области устройства.|
|lastModifiedDateTime|DateTimeOffset|Указывает дату и время последнего обновления для области пользовательского устройства.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScopes
Content-type: application/json
Content-length: 350

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScope",
  "deviceScopeName": "Device Scope Name value",
  "ownerId": "Owner Id value",
  "isBuiltIn": true,
  "enabled": true,
  "status": "computing",
  "parameter": "scopeTag",
  "operator": "equals",
  "valueObjectId": "Value Object Id value",
  "value": "Value value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 522

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScope",
  "id": "936b0460-0460-936b-6004-6b9360046b93",
  "deviceScopeName": "Device Scope Name value",
  "ownerId": "Owner Id value",
  "isBuiltIn": true,
  "enabled": true,
  "status": "computing",
  "parameter": "scopeTag",
  "operator": "equals",
  "valueObjectId": "Value Object Id value",
  "value": "Value value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




