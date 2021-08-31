---
title: тип ресурса mobileAppRelationship
description: Описывает связь между двумя мобильными приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0fac38e910e4889759a07d9b38eac2ee116d0904
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58799826"
---
# <a name="mobileapprelationship-resource-type"></a>тип ресурса mobileAppRelationship

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает связь между двумя мобильными приложениями.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список мобильных устройствAppRelationships](../api/intune-apps-mobileapprelationship-list.md)|[коллекция mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Список свойств и связей объектов [mobileAppRelationship.](../resources/intune-apps-mobileapprelationship.md)|
|[Get mobileAppRelationship](../api/intune-apps-mobileapprelationship-get.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Чтение свойств и связей объекта [mobileAppRelationship.](../resources/intune-apps-mobileapprelationship.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID сущности отношений.|
|targetId|Строка|ID приложения целевого мобильного приложения.|
|targetDisplayName|Строка|Имя отображения целевого мобильного приложения.|
|targetDisplayVersion|Строка|Отображаемая версия целевого мобильного приложения.|
|targetPublisher|Строка|Издатель целевого мобильного приложения.|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|Тип отношений, указывающий, является ли цель родителем или ребенком. Возможные значения: `child`, `parent`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppRelationship"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationship",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String"
}
```



