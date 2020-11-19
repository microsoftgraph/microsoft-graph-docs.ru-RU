---
title: Тип ресурса Граупполиципресентатионвалуе
description: Базовый объект значения представления, в котором хранится значение для одной представления групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d44ce8e11ae1f44d10518ea2b1b0c990153923cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222809"
---
# <a name="grouppolicypresentationvalue-resource-type"></a>Тип ресурса Граупполиципресентатионвалуе

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый объект значения представления, в котором хранится значение для одной представления групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионвалуес](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|Коллекция [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Список свойств и связей объектов [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Получение Граупполиципресентатионвалуе](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Чтение свойств и связей объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Создание Граупполиципресентатионвалуе](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Создание нового объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Удаление Граупполиципресентатионвалуе](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|Нет|Удаляет объект [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).|
|[Обновление Граупполиципресентатионвалуе](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Обновление свойств объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|id|String|Ключ объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|дефинитионвалуе|[граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Значение определения групповой политики, связанное со значением представления.|
|демонстрации|[граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|Представление групповой политики, связанное со значением презентации.|

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




