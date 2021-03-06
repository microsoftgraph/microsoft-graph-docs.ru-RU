---
title: Тип ресурса Граупполиципресентатионвалуетекст
description: Сущность представляет строковое значение для раскрывающегося списка, поля со списком или представления текстового поля в определении политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: be976ec5a80b8e94274d7aa1727e77865ddc72ed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298290"
---
# <a name="grouppolicypresentationvaluetext-resource-type"></a>Тип ресурса Граупполиципресентатионвалуетекст

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность представляет строковое значение для раскрывающегося списка, поля со списком или представления текстового поля в определении политики.


Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионвалуетекстс](../api/intune-grouppolicy-grouppolicypresentationvaluetext-list.md)|Коллекция [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|Список свойств и связей объектов [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .|
|[Получение Граупполиципресентатионвалуетекст](../api/intune-grouppolicy-grouppolicypresentationvaluetext-get.md)|[граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|Чтение свойств и связей объекта [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .|
|[Создание Граупполиципресентатионвалуетекст](../api/intune-grouppolicy-grouppolicypresentationvaluetext-create.md)|[граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|Создание нового объекта [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .|
|[Удаление Граупполиципресентатионвалуетекст](../api/intune-grouppolicy-grouppolicypresentationvaluetext-delete.md)|Нет|Удаляет объект [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).|
|[Обновление Граупполиципресентатионвалуетекст](../api/intune-grouppolicy-grouppolicypresentationvaluetext-update.md)|[граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|Обновление свойств объекта [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|value|String|Строковое значение для связанной презентации.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|дефинитионвалуе|[граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Значение определения групповой политики, связанное со значением представления. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|демонстрации|[граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|Представление групповой политики, связанное со значением презентации. Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": "String"
}
```




