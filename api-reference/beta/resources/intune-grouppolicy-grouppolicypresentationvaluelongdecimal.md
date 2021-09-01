---
title: groupPolicyPresentationValueLongDecimal resource type
description: Объект представляет собой неподписаное длинное значение длинной десятичной презентации текстового окна в определении политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 506bb379a85ed12b2b59f41113fee47359c0d9fb
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58818774"
---
# <a name="grouppolicypresentationvaluelongdecimal-resource-type"></a>groupPolicyPresentationValueLongDecimal resource type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект представляет собой неподписаное длинное значение длинной десятичной презентации текстового окна в определении политики.


Наследует [от groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyPresentationValueLongDecimals](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-list.md)|[коллекция groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Список свойств и связей объектов [groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|
|[Get groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-get.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Чтение свойств и связей объекта [groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|
|[Создание groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-create.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Создайте новый [объект groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|
|[Удаление groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-delete.md)|Нет|Удаляет [группуPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).|
|[Update groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-update.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Обновление свойств объекта [groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|Ключ объекта. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|значение|Int64|Неподписаное длинное значение для связанной презентации.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Значение определения групповой политики, связанное со значением представления. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|презентация|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|Презентация групповой политики, связанная со значением презентации. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueLongDecimal"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": 1024
}
```



