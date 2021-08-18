---
title: тип ресурса mobileAppRelationship
description: Описывает связь между двумя мобильными приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ee9793d2f505394f3188368bc812b79a741decb30a95f27cfbd522af5df6141e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236551"
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
|id|String|ID сущности отношений.|
|targetId|String|ID приложения целевого мобильного приложения.|
|targetDisplayName|Строка|Имя отображения целевого мобильного приложения.|
|targetDisplayVersion|String|Отображаемая версия целевого мобильного приложения.|
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




