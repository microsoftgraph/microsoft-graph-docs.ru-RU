---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3c8db1f356890dc478833e7b77267a218f08bbc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148086"
---
# <a name="managedappconfiguration-resource-type"></a>Тип ресурса managedAppConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация


Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedAppConfigurations](../api/intune-mam-managedappconfiguration-list.md)|Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)|Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).|
|[Получение объекта managedAppConfiguration](../api/intune-mam-managedappconfiguration-get.md)|[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)|Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|String|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|String|Ключ объекта. Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|version|Строка|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|customSettings|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




