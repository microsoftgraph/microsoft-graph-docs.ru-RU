---
title: тип ресурса groupPolicyMigrationReport
description: Отчет о миграции групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c093dd3987a16ec0cb69a861c2614a55caf4e9f7
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817357"
---
# <a name="grouppolicymigrationreport-resource-type"></a>тип ресурса groupPolicyMigrationReport

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Отчет о миграции групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyMigrationReports](../api/intune-gpanalyticsservice-grouppolicymigrationreport-list.md)|[коллекция groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Список свойств и связей объектов [groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|
|[Get groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-get.md)|[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Чтение свойств и связей объекта [groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|
|[Создание groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-create.md)|[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Создайте новый [объект GroupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|
|[Удаление groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-delete.md)|Нет|Удаляет [группуPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).|
|[Update groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-update.md)|[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Обновление свойств объекта [groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|
|[действие createMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-createmigrationreport.md)|String|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано.|
|groupPolicyObjectId|Guid|GUID объекта групповой политики из контента GPO Xml|
|displayName|String|Имя объекта групповой политики из контента GPO Xml|
|ouDistinguishedName|String|Отличительное имя OU.|
|createdDateTime|DateTimeOffset|Дата и время создания GroupPolicyMigrationReport.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения GroupPolicyMigrationReport.|
|groupPolicyCreatedDateTime|DateTimeOffset|Дата и время создания GroupPolicyMigrationReport.|
|groupPolicyLastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения GroupPolicyMigrationReport.|
|migrationReadiness|[groupPolicyMigrationReadiness](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|Покрытие Intune для связанного объекта групповой политики. Возможные значения: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|targetedInActiveDirectory|Логический|Свойство Targeted in AD из GPO Xml Content|
|totalSettingsCount|Int32|Общее число групповых политик Параметры из GPO-файла.|
|supportedSettingsCount|Int32|Количество групповых политик Параметры поддерживается Intune.|
|supportedSettingsPercent|Int32|Процент групповой политики Параметры поддерживается Intune.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupPolicySettingMappings|[коллекция groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Список параметров групповой политики для сопоставлений MDM/Intune.|
|unsupportedGroupPolicyExtensions|[коллекция unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|Список неподтверченных расширений групповой политики внутри объекта групповой политики.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyMigrationReport"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "String (identifier)",
  "groupPolicyObjectId": "Guid",
  "displayName": "String",
  "ouDistinguishedName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "groupPolicyCreatedDateTime": "String (timestamp)",
  "groupPolicyLastModifiedDateTime": "String (timestamp)",
  "migrationReadiness": "String",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 1024,
  "supportedSettingsCount": 1024,
  "supportedSettingsPercent": 1024
}
```



