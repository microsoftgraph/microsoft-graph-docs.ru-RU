---
title: Тип ресурса Граупполицисеттингмаппинг
description: Параметр групповой политики для сопоставления MDM/Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d507687e6a14e276a177a5795afa55aa5fe3f051
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697478"
---
# <a name="grouppolicysettingmapping-resource-type"></a>Тип ресурса Граупполицисеттингмаппинг

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметр групповой политики для сопоставления MDM/Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполицисеттингмаппингс](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|Коллекция [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Список свойств и связей объектов [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|
|[Получение Граупполицисеттингмаппинг](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Чтение свойств и связей объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|
|[Создание Граупполицисеттингмаппинг](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Создание нового объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|
|[Удаление Граупполицисеттингмаппинг](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|Нет|Удаляет объект [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).|
|[Обновление Граупполицисеттингмаппинг](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Обновление свойств объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Пока не задокументировано.|
|parentId|Строка|Родительский идентификатор параметра групповой политики.|
|чилдидлист|Коллекция строк|Список дочерних идентификаторов параметра групповой политики.|
|settingName|String|Имя этого параметра групповой политики.|
|settingValue|Строка|Значение этого параметра групповой политики.|
|сеттингвалуетипе|Строка|Тип значения этого параметра групповой политики.|
|сеттингдисплайнаме|Строка|Отображаемое имя этого параметра групповой политики.|
|сеттингдисплайвалуе|Строка|Отображаемое значение этого параметра групповой политики.|
|сеттингдисплайвалуетипе|Строка|Отображаемый тип значения этого параметра групповой политики.|
|сеттингвалуедисплайунитс|Строка|Отображаемые единицы значения параметра групповой политики|
|сеттингкатегори|Строка|Категория, в которой находится параметр групповой политики.|
|мдмкспнаме|Строка|Имя CSP, которое сопоставляется параметру групповой политики.|
|мдмсеттингури|Строка|Универсальный код ресурса (URI) MDM CSP, которому соответствует этот параметр групповой политики.|
|мдмминимумосверсион|Int32|Минимальная версия ОС, поддерживаемая параметром MDM.|
|сеттингтипе|[groupPolicySettingType](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|Тип параметра (Security или ADMX) групповой политики. Возможные значения: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.|
|исмдмсуппортед|Логический|Указывает, поддерживается ли Intune или нет|
|mdmSupportedState|[mdmSupportedState](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|Указывает, поддерживается ли параметр в MDM. Возможные значения: `unknown`, `supported`, `unsupported`, `deprecated`.|
|сеттингскопе|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|Область применения параметра. Возможные значения: `unknown`, `device`, `user`.|
|интунесеттингурилист|Коллекция строк|Список URI параметров Intune, которые сопоставлены параметру групповой политики|
|интунесеттингдефинитионид|Строка|Идентификатор определения параметра Intune|
|адмкссеттингдефинитионид|Строка|Идентификатор групповой политики ADMX|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicySettingMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "String (identifier)",
  "parentId": "String",
  "childIdList": [
    "String"
  ],
  "settingName": "String",
  "settingValue": "String",
  "settingValueType": "String",
  "settingDisplayName": "String",
  "settingDisplayValue": "String",
  "settingDisplayValueType": "String",
  "settingValueDisplayUnits": "String",
  "settingCategory": "String",
  "mdmCspName": "String",
  "mdmSettingUri": "String",
  "mdmMinimumOSVersion": 1024,
  "settingType": "String",
  "isMdmSupported": true,
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "String"
  ],
  "intuneSettingDefinitionId": "String",
  "admxSettingDefinitionId": "String"
}
```





