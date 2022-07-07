---
title: Тип ресурса deviceManagementConfigurationRedirectSettingDefinition
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 33ee422eda6aaeebd5d3e4098be7e94964aa379c
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670578"
---
# <a name="devicemanagementconfigurationredirectsettingdefinition-resource-type"></a>Тип ресурса deviceManagementConfigurationRedirectSettingDefinition

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.


Наследует от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление deviceManagementConfigurationRedirectSettingDefinitions](../api/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition-list.md)|[Коллекция deviceManagementConfigurationRedirectSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md)|Список свойств и связей объектов [deviceManagementConfigurationRedirectSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md) .|
|[Получение объекта deviceManagementConfigurationRedirectSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition-get.md)|[deviceManagementConfigurationRedirectSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md)|Чтение свойств и связей объекта [deviceManagementConfigurationRedirectSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md) .|
|[Создание объекта deviceManagementConfigurationRedirectSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition-create.md)|[deviceManagementConfigurationRedirectSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md)|Создайте объект [deviceManagementConfigurationRedirectSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md) .|
|[Удаление объекта deviceManagementConfigurationRedirectSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition-delete.md)|Нет|Удаляет [объект deviceManagementConfigurationRedirectSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md).|
|[Обновление объекта deviceManagementConfigurationRedirectSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition-update.md)|[deviceManagementConfigurationRedirectSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md)|Обновление свойств объекта [deviceManagementConfigurationRedirectSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Применимость|[deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|Сведения о том, какой параметр устройства применим к inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|accessTypes|[deviceManagementConfigurationSettingAccessTypes](../resources/intune-shared-devicemanagementconfigurationsettingaccesstypes.md)|Режим доступа для чтения и записи параметра, унаследованного от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md). Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.|
|keywords|Коллекция строк|Токены для поиска параметров на унаследованном от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|infoUrls|Коллекция объектов string|Список ссылок, дополнительные сведения о параметре можно найти на странице Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|Вхождение|[deviceManagementConfigurationSettingOccurrence](../resources/intune-shared-devicemanagementconfigurationsettingoccurrence.md)|Указывает, является ли параметр обязательным или не унаследованным от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|Baseuri|String|Базовый путь CSP, унаследованный [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|offsetUri|String|Смещение пути CSP от base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|rootDefinitionId|String|Определение корневого параметра, если параметр является дочерним. Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|Categoryid|String|Указывает группу с областями, в которой настроен параметр в указанном поставщике служб конфигурации (CSP), унаследованном от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-shared-devicemanagementconfigurationsettingusage.md)|Тип параметра, например конфигурация и соответствие, унаследованные от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md). Возможные значения: `none`, `configuration`, `compliance`.|
|uxBehavior|[DeviceManagementConfigurationControlType](../resources/intune-shared-devicemanagementconfigurationcontroltype.md)|Задание представления типа элемента управления в пользовательском интерфейсе, унаследованном от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md). Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.|
|visibility|[deviceManagementConfigurationSettingVisibility](../resources/intune-shared-devicemanagementconfigurationsettingvisibility.md)|Задание области видимости для пользовательского интерфейса, унаследованного от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md). Возможные значения: `none`, `settingsCatalog`, `template`.|
|referredSettingInformationList|[Коллекция deviceManagementConfigurationReferredSettingInformation](../resources/intune-shared-devicemanagementconfigurationreferredsettinginformation.md)|Список ссылаемой информации о параметрах. Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|id|String|Идентификатор элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|description|String|Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|Helptext|String|Текст справки элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|name|String|Имя элемента, унаследованного от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|displayName|String|Отображаемое имя элемента, унаследованного от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|version|String|Версия элемента, наследуемая [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|deepLink|String|Прямая ссылка, указывав на определенное расположение в консоли Intune, из которой необходимо управлять поддержкой функций.|
|redirectMessage|String|Сообщение о том, что при щелчке по ссылке пользователь перенаправляется на поддерживаемую страницу для управления параметрами.|
|redirectReason|String|Указывает причину перенаправления пользователя в альтернативное расположение в консоли.  Например, профили Wi-Fi не поддерживаются в каталоге параметров и должны быть созданы с помощью политики шаблонов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationRedirectSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationRedirectSettingDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "String",
    "platform": "String",
    "deviceMode": "String",
    "technologies": "String"
  },
  "accessTypes": "String",
  "keywords": [
    "String"
  ],
  "infoUrls": [
    "String"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 1024,
    "maxDeviceOccurrence": 1024
  },
  "baseUri": "String",
  "offsetUri": "String",
  "rootDefinitionId": "String",
  "categoryId": "String",
  "settingUsage": "String",
  "uxBehavior": "String",
  "visibility": "String",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "String"
    }
  ],
  "id": "String (identifier)",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "version": "String",
  "deepLink": "String",
  "redirectMessage": "String",
  "redirectReason": "String"
}
```




