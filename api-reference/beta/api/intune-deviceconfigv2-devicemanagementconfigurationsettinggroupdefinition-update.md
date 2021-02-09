---
title: Обновление deviceManagementConfigurationSettingGroupDefinition
description: Обновление свойств объекта deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61c2d97af46e718d31eace72ac2b19c437410bb4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158921"
---
# <a name="update-devicemanagementconfigurationsettinggroupdefinition"></a>Обновление deviceManagementConfigurationSettingGroupDefinition

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса предопределение представления объекта [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|применимость|[deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|Сведения о том, какой параметр устройства применим к inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|accessTypes|[deviceManagementConfigurationSettingAccessTypes](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|Режим доступа для чтения и записи параметра. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.|
|keywords|Коллекция String|Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|infoUrls|Коллекция String|Список ссылок, дополнительные сведения о параметре можно найти по адресу Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|occurrence|[deviceManagementConfigurationSettingOccurrence](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|baseUri|String|Базовый путь CSP Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|offsetUri|String|Смещение пути CSP от Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|rootDefinitionId|String|Определение корневого параметра, если этот параметр является параметром-child. Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|categoryId|String|Указывает группу области, в которой настроен параметр в указанном поставщике служб конфигурации (CSP), наследуемом от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|Тип параметра, например конфигурация и соответствие. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) Возможные значения: `none`, `configuration`.|
|uxBehavior|[deviceManagementConfigurationControlType](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|Представление типа параметра в UX. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.|
|id|String|Идентификатор элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|description|String|Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|helpText|String|Текст справки для элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|name|String|Имя элемента. Наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|displayName|String|Отображающее имя элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|version|String|Версия элемента. Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|childIds|Коллекция String|Зависимые параметры для этой группы параметров|
|dependentOn|[Коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)|Список зависимостей для группы параметров|
|dependedOnBy|[Коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)|Список параметров, которые зависят от этого параметра|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1477

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "macOS",
    "deviceMode": "kiosk",
    "technologies": "mdm"
  },
  "accessTypes": "add",
  "keywords": [
    "Keywords value"
  ],
  "infoUrls": [
    "Info Urls value"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 3,
    "maxDeviceOccurrence": 3
  },
  "baseUri": "Base Uri value",
  "offsetUri": "Offset Uri value",
  "rootDefinitionId": "Root Definition Id value",
  "categoryId": "Category Id value",
  "settingUsage": "configuration",
  "uxBehavior": "dropdown",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "childIds": [
    "Child Ids value"
  ],
  "dependentOn": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
      "dependentOn": "Dependent On value",
      "parentSettingId": "Parent Setting Id value"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "Depended On By value",
      "required": true
    }
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1526

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "macOS",
    "deviceMode": "kiosk",
    "technologies": "mdm"
  },
  "accessTypes": "add",
  "keywords": [
    "Keywords value"
  ],
  "infoUrls": [
    "Info Urls value"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 3,
    "maxDeviceOccurrence": 3
  },
  "baseUri": "Base Uri value",
  "offsetUri": "Offset Uri value",
  "rootDefinitionId": "Root Definition Id value",
  "categoryId": "Category Id value",
  "settingUsage": "configuration",
  "uxBehavior": "dropdown",
  "id": "95dc9604-9604-95dc-0496-dc950496dc95",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "childIds": [
    "Child Ids value"
  ],
  "dependentOn": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
      "dependentOn": "Dependent On value",
      "parentSettingId": "Parent Setting Id value"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "Depended On By value",
      "required": true
    }
  ]
}
```




