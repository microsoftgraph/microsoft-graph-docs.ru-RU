---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 525fa036f373a9e8796493ba87f24c9134aad2ad
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60448536"
---
# <a name="managedappconfiguration-resource-type"></a>Тип ресурса managedAppConfiguration

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|String|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|customSettings|Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)|Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой|

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



