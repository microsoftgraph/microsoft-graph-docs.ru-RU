---
title: Тип ресурса Мобилеаппсуперседенце
description: Описывает отношение замены между двумя мобильными приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2bdc14c1d9e65d32e664318d894e11bd08d56320
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48719710"
---
# <a name="mobileappsupersedence-resource-type"></a>Тип ресурса Мобилеаппсуперседенце

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает отношение замены между двумя мобильными приложениями.


Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Мобилеаппсуперседенцес](../api/intune-apps-mobileappsupersedence-list.md)|Коллекция [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md)|Список свойств и связей объектов [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md) .|
|[Получение Мобилеаппсуперседенце](../api/intune-apps-mobileappsupersedence-get.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Чтение свойств и связей объекта [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md) .|
|[Создание Мобилеаппсуперседенце](../api/intune-apps-mobileappsupersedence-create.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Создание нового объекта [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md) .|
|[Удаление Мобилеаппсуперседенце](../api/intune-apps-mobileappsupersedence-delete.md)|Нет|Удаляет объект [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md).|
|[Обновление Мобилеаппсуперседенце](../api/intune-apps-mobileappsupersedence-update.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Обновление свойств объекта [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|targetId|Строка|Идентификатор приложения целевого приложения для мобильных устройств. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|таржетдисплайнаме|Строка|Отображаемое имя целевого мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|Тип связи, указывающий, является ли целевой объект родительским или дочерним. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md). Возможные значения: `child`, `parent`.|
|суперседенцетипе|[mobileAppSupersedenceType](../resources/intune-apps-mobileappsupersedencetype.md)|Тип отношения замены между родительским и дочерним приложениями. Возможные значения: `update`, `replace`.|
|суперседедаппкаунт|Int32|Общее число приложений, напрямую или косвенно заменяющих дочерним приложением.|
|суперседингаппкаунт|Int32|Общее число приложений, напрямую или косвенно заменяющих родительское приложение.|

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
  "targetType": "String",
  "supersedenceType": "String",
  "supersededAppCount": 1024,
  "supersedingAppCount": 1024
}
```





