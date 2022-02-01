---
title: Обновление deviceManagementConfigurationCategory
description: Обновление свойств объекта deviceManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83c52ecd53828057eed3cb9878c6d33bd5424b9b
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292083"
---
# <a name="update-devicemanagementconfigurationcategory"></a>Обновление deviceManagementConfigurationCategory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .

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
PATCH /deviceManagement/complianceCategories/{deviceManagementConfigurationCategoryId}
PATCH /deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .

В следующей таблице показаны свойства, необходимые при создании [устройстваManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор элемента|
|description|String|Описание элемента|
|categoryDescription|String|Описание загона категории|
|helpText|String|Справка текста элемента|
|name|String|Имя элемента|
|displayName|String|Отображение имени элемента|
|платформы|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Типы платформ, которые имеются в этой категории. Возможные значения: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|технологии|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Типы технологий, которые имеют параметры в категории. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|Указывает, что категория содержит параметры, используемые для соответствия требованиям или конфигурации. Возможные значения: `none`, `configuration`, `compliance`.|
|parentCategoryId|String|Родительский id категории.|
|rootCategoryId|String|Корневой id категории.|
|childCategoryIds|Коллекция объектов string|Список детских ids этой категории.|



## <a name="response"></a>Отклик
В случае успешного `200 OK` выполнения этот метод возвращает код ответа и обновленный [объект deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/complianceCategories/{deviceManagementConfigurationCategoryId}
Content-type: application/json
Content-length: 523

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "description": "Description value",
  "categoryDescription": "Category Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "android",
  "technologies": "mdm",
  "settingUsage": "configuration",
  "parentCategoryId": "Parent Category Id value",
  "rootCategoryId": "Root Category Id value",
  "childCategoryIds": [
    "Child Category Ids value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 572

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "cff34dd2-4dd2-cff3-d24d-f3cfd24df3cf",
  "description": "Description value",
  "categoryDescription": "Category Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "android",
  "technologies": "mdm",
  "settingUsage": "configuration",
  "parentCategoryId": "Parent Category Id value",
  "rootCategoryId": "Root Category Id value",
  "childCategoryIds": [
    "Child Category Ids value"
  ]
}
```




