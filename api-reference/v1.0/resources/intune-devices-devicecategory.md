---
title: Тип ресурса deviceCategory
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d455d1788cdb9f992201228be3ca6fbad67bd45cf5637795f2539b2fd7f0f84f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192406"
---
# <a name="devicecategory-resource-type"></a>Тип ресурса deviceCategory

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceCategory](../api/intune-devices-devicecategory-get.md)|[deviceCategory](../resources/intune-devices-devicecategory.md)|Чтение свойств и связей объекта [deviceCategory](../resources/intune-devices-devicecategory.md).|
|[Обновление объекта deviceCategory](../api/intune-devices-devicecategory-update.md)|[deviceCategory](../resources/intune-devices-devicecategory.md)|Обновление свойств объекта [deviceCategory](../resources/intune-devices-devicecategory.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор категории устройства. Только для чтения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)"
}
```




