---
title: Обновление оборудованияКонфигурация
description: Обновление свойств объекта hardwareConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6fac95e1e99fd4548668fb336f8d2661b399830
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291017"
---
# <a name="update-hardwareconfiguration"></a>Обновление оборудованияКонфигурация

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) .

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
PATCH /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) .

В следующей таблице показаны свойства, необходимые при создании [аппаратнойконфигурации](../resources/intune-deviceconfig-hardwareconfiguration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор конфигурации оборудования|
|version|Int32|Версия конфигурации оборудования (например. 1, 2, 3 ...)|
|displayName|String|Имя конфигурации оборудования|
|description|String|Описание конфигурации оборудования|
|createdDateTime|DateTimeOffset|Время создания конфигурации оборудования. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Время изменения конфигурации оборудования. Это свойство доступно только для чтения.|
|fileName|String|Имя файла конфигурации оборудования|
|configurationFileContent|Binary|Содержимое файла конфигурации оборудования|
|hardwareConfigurationFormat|[hardwareConfigurationFormat](../resources/intune-deviceconfig-hardwareconfigurationformat.md)|Тип Oem конфигурации оборудования (например. DELL, HP, Surface и SurfaceDock). Возможные значения: `dell`, `surface`, `surfaceDock`.|
|roleScopeTagIds|Коллекция String|Список ID-тегов области для конфигурации оборудования|
|perDevicePasswordDisabled|Логическое|Значение, указывающее, отключен ли каждый devcive pasword|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код `200 OK` отклика и обновленный объект [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.hardwareConfiguration",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "fileName": "File Name value",
  "configurationFileContent": "Y29uZmlndXJhdGlvbkZpbGVDb250ZW50",
  "hardwareConfigurationFormat": "surface",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "perDevicePasswordDisabled": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "@odata.type": "#microsoft.graph.hardwareConfiguration",
  "id": "da410f27-0f27-da41-270f-41da270f41da",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "fileName": "File Name value",
  "configurationFileContent": "Y29uZmlndXJhdGlvbkZpbGVDb250ZW50",
  "hardwareConfigurationFormat": "surface",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "perDevicePasswordDisabled": true
}
```




