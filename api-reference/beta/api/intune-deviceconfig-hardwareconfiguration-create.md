---
title: Создание hardwareConfiguration
description: Создание нового объекта hardwareConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97b4d40b7bd99b70a46f7d6c929ff2209ef1821d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345594"
---
# <a name="create-hardwareconfiguration"></a>Создание hardwareConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта hardwareConfiguration.](../resources/intune-deviceconfig-hardwareconfiguration.md)

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
POST /deviceManagement/hardwareConfigurations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта hardwareConfiguration.

В следующей таблице показаны свойства, необходимые при создании аппаратнойконфигурации.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор конфигурации оборудования|
|version|Int32|Версия конфигурации оборудования|
|displayName|String|Имя конфигурации оборудования|
|description|Строка|Описание конфигурации оборудования|
|createdDateTime|DateTimeOffset|Время создания конфигурации оборудования. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Время изменения конфигурации оборудования. Это свойство доступно только для чтения.|
|fileName|String|Имя файла конфигурации оборудования|
|configurationFileContent|Binary|Содержимое файла конфигурации оборудования|
|hardwareConfigurationFormat|[hardwareConfigurationFormat](../resources/intune-deviceconfig-hardwareconfigurationformat.md)|Тип Oem конфигурации оборудования. Возможные значения: `dell`, `surface`, `surfaceDock`.|
|roleScopeTagIds|Коллекция String|Список ID-тегов области для конфигурации оборудования|
|perDevicePasswordDisabled|Boolean|Значение, указывающее, отключен ли каждый devcive pasword|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations
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
HTTP/1.1 201 Created
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




