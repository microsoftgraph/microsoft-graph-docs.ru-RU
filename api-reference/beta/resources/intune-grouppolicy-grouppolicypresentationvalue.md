---
title: Тип ресурса Граупполиципресентатионвалуе
description: Базовый объект значения представления, в котором хранится значение для одной представления групповой политики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 38686cdbda5003beb0ffe9a020325742294605a4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998550"
---
# <a name="grouppolicypresentationvalue-resource-type"></a>Тип ресурса Граупполиципресентатионвалуе

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый объект значения представления, в котором хранится значение для одной представления групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионвалуес](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|Коллекция [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Список свойств и связей объектов [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Получение Граупполиципресентатионвалуе](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[Граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Чтение свойств и связей объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Создание Граупполиципресентатионвалуе](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[Граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Создание нового объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Удаление Граупполиципресентатионвалуе](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|Нет|Удаляет объект [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).|
|[Обновление Граупполиципресентатионвалуе](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[Граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Обновление свойств объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|id|String|Ключ объекта.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|Дефинитионвалуе|[Граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Значение определения групповой политики, связанное со значением представления.|
|демонстрации|[Граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|Представление групповой политики, связанное со значением презентации.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)"
}
```





