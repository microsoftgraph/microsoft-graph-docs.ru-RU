---
title: Тип ресурса Граупполицидефинитионвалуе
description: Сущность значения определения хранит значение для одного определения групповой политики.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2aa0eef1b4921d1b364486b9af254fba2a8322c0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800996"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a>Тип ресурса Граупполицидефинитионвалуе

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность значения определения хранит значение для одного определения групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполицидефинитионвалуес](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Список свойств и связей объектов [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .|
|[Получение Граупполицидефинитионвалуе](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[Граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Чтение свойств и связей объекта [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .|
|[Создание Граупполицидефинитионвалуе](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[Граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Создание нового объекта [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .|
|[Удаление Граупполицидефинитионвалуе](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|Нет|Удаляет объект [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).|
|[Обновление Граупполицидефинитионвалуе](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[Граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Обновление свойств объекта [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|enabled|Boolean|Включает или отключает соответствующее определение групповой политики.|
|Конфигуратионтипе|[Граупполициконфигуратионтипе](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|Указывает, как должно настраиваться значение. Это может быть либо политика, либо предпочтение. Возможные значения: `policy`, `preference`.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|Пресентатионвалуес|Коллекция [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Связанные значения представления групповой политики со значением определения.|
|RDLC|[Граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Связанное определение групповой политики со значением.|

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





