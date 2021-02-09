---
title: Тип ресурса mobileAppDependency
description: Описывает тип зависимостей между двумя мобильными приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e8e6bdcd9cf5903d07fb858103bd3620e9a187da
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161567"
---
# <a name="mobileappdependency-resource-type"></a>Тип ресурса mobileAppDependency

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает тип зависимостей между двумя мобильными приложениями.


Наследуется от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileAppDependencies](../api/intune-apps-mobileappdependency-list.md)|[Коллекция mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Список свойств и связей объектов [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|
|[Get mobileAppDependency](../api/intune-apps-mobileappdependency-get.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Чтение свойств и связей объекта [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|
|[Создание mobileAppDependency](../api/intune-apps-mobileappdependency-create.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Создание объекта [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|
|[Удаление mobileAppDependency](../api/intune-apps-mobileappdependency-delete.md)|Нет|Удаляет [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|
|[Обновление mobileAppDependency](../api/intune-apps-mobileappdependency-update.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Обновление свойств объекта [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ИД сущности отношения. Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|ИД целевого мобильного приложения. Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|String|Отображаемое имя целевого мобильного приложения. Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayVersion|String|Отображаемая версия целевого мобильного приложения. Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetPublisher|String|Издатель целевого мобильного приложения. Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|Тип связи, указывающий, является ли целевой объект родительским или родительским. Наследуется [от mobileAppRelationship.](../resources/intune-apps-mobileapprelationship.md) Возможные значения: `child`, `parent`.|
|dependencyType|[mobileAppDependencyType](../resources/intune-apps-mobileappdependencytype.md)|Тип отношения зависимостей между родительским и родительским приложениями. Возможные значения: `detect`, `autoInstall`.|
|dependentAppCount|Int32|Общее количество приложений, которые напрямую или косвенно зависят от родительского приложения.|
|dependsOnAppCount|Int32|Общее количество приложений, от которых непосредственно или косвенно зависит это приложение.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String",
  "dependencyType": "String",
  "dependentAppCount": 1024,
  "dependsOnAppCount": 1024
}
```




