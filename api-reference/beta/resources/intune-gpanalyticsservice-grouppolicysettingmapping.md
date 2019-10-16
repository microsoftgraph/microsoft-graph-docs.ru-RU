---
title: Тип ресурса Граупполицисеттингмаппинг
description: Параметр групповой политики для сопоставления MDM/Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cacc4a03a8c8b974eec91bc0100ddb4d56c0cfbd
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539192"
---
# <a name="grouppolicysettingmapping-resource-type"></a>Тип ресурса Граупполицисеттингмаппинг

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметр групповой политики для сопоставления MDM/Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполицисеттингмаппингс](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|Коллекция [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Список свойств и связей объектов [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|
|[Получение Граупполицисеттингмаппинг](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Чтение свойств и связей объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|
|[Создание Граупполицисеттингмаппинг](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Создание нового объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|
|[Удаление Граупполицисеттингмаппинг](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|Нет|Удаляет объект [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).|
|[Обновление Граупполицисеттингмаппинг](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Обновление свойств объекта [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано.|
|parentId|String|Родительский идентификатор параметра групповой политики.|
|чилдидлист|Коллекция String|Список дочерних идентификаторов параметра групповой политики.|
|settingName|String|Имя этого параметра групповой политики.|
|settingValue|String|Значение этого параметра групповой политики.|
|сеттингвалуетипе|String|Тип значения этого параметра групповой политики.|
|сеттингдисплайнаме|String|Отображаемое имя этого параметра групповой политики.|
|сеттингдисплайвалуе|String|Отображаемое значение этого параметра групповой политики.|
|сеттингдисплайвалуетипе|String|Отображаемый тип значения этого параметра групповой политики.|
|сеттингвалуедисплайунитс|String|Отображаемые единицы значения параметра групповой политики|
|сеттингкатегори|String|Категория, в которой находится параметр групповой политики.|
|мдмкспнаме|String|Имя CSP, которое сопоставляется параметру групповой политики.|
|мдмсеттингури|String|Универсальный код ресурса (URI) MDM CSP, которому соответствует этот параметр групповой политики.|
|мдмминимумосверсион|Int32|Минимальная версия ОС, поддерживаемая параметром MDM.|
|сеттингтипе|[граупполицисеттингтипе](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|Тип параметра (Security или ADMX) групповой политики. Возможные значения: `unknown`, `policy`, `account`.|
|исмдмсуппортед|Логический|Указывает, поддерживается ли Intune или нет|
|сеттингскопе|[граупполицисеттингскопе](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|Область применения параметра. Возможные значения: `unknown`, `device`, `user`.|
|интунесеттингурилист|Коллекция String|Список URI параметров Intune, которые сопоставлены параметру групповой политики|

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
  "settingScope": "String",
  "intuneSettingUriList": [
    "String"
  ]
}
```



