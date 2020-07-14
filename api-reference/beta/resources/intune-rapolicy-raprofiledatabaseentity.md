---
title: Тип ресурса Рапрофиледатабасинтити
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4a90d03258e4e84706d4828aaae2d10a1c064942
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124379"
---
# <a name="raprofiledatabaseentity-resource-type"></a>Тип ресурса Рапрофиледатабасинтити

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Рапрофиледатабасинтитиес](../api/intune-rapolicy-raprofiledatabaseentity-list.md)|Коллекция [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md)|Список свойств и связей объектов [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) .|
|[Получение Рапрофиледатабасинтити](../api/intune-rapolicy-raprofiledatabaseentity-get.md)|[рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md)|Чтение свойств и связей объекта [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) .|
|[Создание Рапрофиледатабасинтити](../api/intune-rapolicy-raprofiledatabaseentity-create.md)|[рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md)|Создание нового объекта [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) .|
|[Удаление Рапрофиледатабасинтити](../api/intune-rapolicy-raprofiledatabaseentity-delete.md)|Отсутствует|Удаляет объект [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md).|
|[Обновление Рапрофиледатабасинтити](../api/intune-rapolicy-raprofiledatabaseentity-update.md)|[рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md)|Обновление свойств объекта [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|version|Int32|Пока нет описания|
|isDeleted|Boolean|Пока не задокументировано|
|софтделетедтиме|DateTimeOffset|Пока не задокументировано.|
|displayName|Строка|Пока не задокументировано.|
|линкедпрофилеидс|Коллекция объектов Guid|Пока не задокументировано.|
|профилетипенаме|String|Пока не задокументировано.|
|профилебоди|String|Пока не задокументировано.|
|профилебодихаш|String|Пока не задокументировано.|
|platformType|Int32|Пока нет описания|
|трансформедпрофилебоди|String|Пока не задокументировано.|
|трансформедпрофилебодихаш|String|Пока не задокументировано.|
|tenantId|Guid|Пока не задокументировано.|
|профилеид|Guid|Пока не задокументировано.|
|eTag|String|Пока не задокументировано.|
|Схемы|[раполицисервицеверсионс](../resources/intune-rapolicy-rapolicyserviceversions.md)|Еще не задокументировано. Возможные значения: `initial`, `betaStart`, `experimentStart`, `mmpcStart`, `iosStart`.|
|Дата|DateTimeOffset|Пока не задокументировано.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.raProfileDatabaseEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
  "version": 1024,
  "isDeleted": true,
  "softDeletedTime": "String (timestamp)",
  "displayName": "String",
  "linkedProfileIds": [
    "Guid"
  ],
  "profileTypeName": "String",
  "profileBody": "String",
  "profileBodyHash": "String",
  "platformType": 1024,
  "transformedProfileBody": "String",
  "transformedProfileBodyHash": "String",
  "tenantId": "Guid",
  "profileId": "Guid",
  "eTag": "String",
  "schemaVersion": "String",
  "lastModified": "String (timestamp)"
}
```



