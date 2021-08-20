---
title: тип ресурса mobileAppSupersedence
description: Описывает отношение суперпотенции между двумя мобильными приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4072570fafac01df30a9542f80bf0ccae9ff9e18606f7e09e8da3a822da04328
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54161411"
---
# <a name="mobileappsupersedence-resource-type"></a>тип ресурса mobileAppSupersedence

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает отношение суперпотенции между двумя мобильными приложениями.


Наследует от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileAppSupersedences](../api/intune-apps-mobileappsupersedence-list.md)|[коллекция mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Список свойств и связей объектов [mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)|
|[Get mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-get.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Чтение свойств и связей объекта [mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)|
|[Создание mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-create.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Создание нового [объекта mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)|
|[Удаление mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-delete.md)|Нет|Удаляет [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md).|
|[Обновление mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-update.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Обновление свойств объекта [mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID сущности отношений. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|ID приложения целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|String|Имя отображения целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayVersion|Строка|Отображаемая версия целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetPublisher|String|Издатель целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|Тип отношений, указывающий, является ли цель родителем или ребенком. Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md). Возможные значения: `child`, `parent`.|
|supersedenceType|[mobileAppSupersedenceType](../resources/intune-apps-mobileappsupersedencetype.md)|Тип отношения supersedence между родительскими и детскими приложениями. Возможные значения: `update`, `replace`.|
|supersededAppCount|Int32|Общее количество приложений, прямо или косвенно выменимых детским приложением.|
|supersedingAppCount|Int32|Общее число приложений, прямо или косвенно выменив родительское приложение.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppSupersedence"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String",
  "supersedenceType": "String",
  "supersededAppCount": 1024,
  "supersedingAppCount": 1024
}
```




