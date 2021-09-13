---
title: тип ресурса mobileAppSupersedence
description: Описывает отношение суперпотенции между двумя мобильными приложениями.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff91da571956d7579d27f65d485d97c158c17bee
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075853"
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
|targetDisplayVersion|String|Отображаемая версия целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
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



