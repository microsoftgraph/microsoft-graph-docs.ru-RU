---
title: тип ресурса mobileAppDependency
description: Описывает тип зависимости между двумя мобильными приложениями.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d85f2d15a50aa98a9e1dc57d902153617a012877
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040535"
---
# <a name="mobileappdependency-resource-type"></a>тип ресурса mobileAppDependency

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает тип зависимости между двумя мобильными приложениями.


Наследует от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileAppDependencies](../api/intune-apps-mobileappdependency-list.md)|[коллекция mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Список свойств и связей объектов [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|
|[Get mobileAppDependency](../api/intune-apps-mobileappdependency-get.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Чтение свойств и связей объекта [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|
|[Создание mobileAppDependency](../api/intune-apps-mobileappdependency-create.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Создание нового [объекта mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|
|[Удаление mobileAppDependency](../api/intune-apps-mobileappdependency-delete.md)|Нет|Удаляет [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).|
|[Обновление mobileAppDependency](../api/intune-apps-mobileappdependency-update.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Обновление свойств объекта [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID сущности отношений. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|ID приложения целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|String|Имя отображения целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayVersion|String|Отображаемая версия целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetPublisher|String|Издатель целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|Тип отношений, указывающий, является ли цель родителем или ребенком. Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md). Возможные значения: `child`, `parent`.|
|dependencyType|[mobileAppDependencyType](../resources/intune-apps-mobileappdependencytype.md)|Тип зависимости между родительскими и детскими приложениями. Возможные значения: `detect`, `autoInstall`.|
|dependentAppCount|Int32|Общее число приложений, которые напрямую или косвенно зависят от родительского приложения.|
|dependsOnAppCount|Int32|Общее число приложений, от которых напрямую или косвенно зависит детское приложение.|

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



