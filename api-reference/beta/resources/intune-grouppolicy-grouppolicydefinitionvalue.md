---
title: тип ресурса groupPolicyDefinitionValue
description: Объект значения определения сохраняет значение для определения единой групповой политики.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d0147c706711e9f34ee8680cb4ad70cf3e4b6a1f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086122"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a>тип ресурса groupPolicyDefinitionValue

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект значения определения сохраняет значение для определения единой групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyDefinitionValues](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|[коллекция groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Список свойств и связей объектов [groupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|
|[Get groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Чтение свойств и связей объекта [groupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|
|[Создание groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Создайте новый [объект GroupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|
|[Удаление groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|Нет|Удаляет [группуPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).|
|[Update groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Обновление свойств объекта [groupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|enabled|Boolean|Включает или отключает связанное определение групповой политики.|
|configurationType|[groupPolicyConfigurationType](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|Указывает, как следует настроить значение. Это может быть как политика, так и как предпочтение. Возможные значения: `policy`, `preference`.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|presentationValues|[коллекция groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Связанные значения представления групповой политики со значением определения.|
|определение|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Связанное определение групповой политики со значением.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "String (timestamp)",
  "enabled": true,
  "configurationType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



