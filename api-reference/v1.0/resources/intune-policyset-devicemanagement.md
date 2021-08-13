---
title: Тип ресурса deviceManagement
description: Сущность Singleton, которая выступает в качестве контейнера для всех функций управления устройствами и приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e2ba365bd9c5e1fa4360dc6b5e0ff14e69eb03d5ccbea0e1510e0287294a4842
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169447"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность Singleton, которая выступает в качестве контейнера для всех функций управления устройствами и приложениями.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune-policyset-devicemanagement-get.md)|[deviceManagement](../resources/intune-policyset-devicemanagement.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune-policyset-devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune-policyset-devicemanagement-update.md)|[deviceManagement](../resources/intune-policyset-devicemanagement.md)|Обновление свойств объекта [deviceManagement](../resources/intune-policyset-devicemanagement.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




