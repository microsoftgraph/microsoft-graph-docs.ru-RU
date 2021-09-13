---
title: тип ресурса groupPolicyMigrationReport
description: Отчет о миграции групповой политики.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb50a01e3f812b1e4e5cb6b986ef52d4ec1817de
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086248"
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
|targetedInActiveDirectory|Логическое|Свойство Targeted in AD из GPO Xml Content|
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



