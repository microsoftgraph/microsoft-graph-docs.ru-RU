---
title: тип ресурса groupPolicyPresentationValueBoolean
description: Объект представляет значение Boolean презентации контрольных ящиков в определении политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0a6fcb751d44c1be63bd8954bf2f8ee30342a1b9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788425"
---
# <a name="grouppolicypresentationvalueboolean-resource-type"></a>тип ресурса groupPolicyPresentationValueBoolean

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект представляет значение Boolean презентации контрольных ящиков в определении политики.


Наследует [от groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyPresentationValueBooleans](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-list.md)|[коллекция groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|Список свойств и связей объектов [groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|
|[Get groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-get.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|Чтение свойств и связей объекта [groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|
|[Создание groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-create.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|Создайте новый [объект groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|
|[Удаление groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-delete.md)|Нет|Удаляет [группуPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).|
|[Update groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-update.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|Обновление свойств объекта [groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|Строка|Ключ объекта. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|value|Boolean|Значение boolean для связанной презентации.|

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
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": true
}
```



