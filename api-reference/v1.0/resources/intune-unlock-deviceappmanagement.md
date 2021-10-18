---
title: Тип ресурса deviceAppManagement
description: Сущность Singleton, которая выступает в качестве контейнера для всех функций управления устройствами и приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e7d729b242787200986dc13f61d6b46d12ef639b
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60456659"
---
# <a name="deviceappmanagement-resource-type"></a>Тип ресурса deviceAppManagement

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность Singleton, которая выступает в качестве контейнера для всех функций управления устройствами и приложениями.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceAppManagement](../api/intune-unlock-deviceappmanagement-get.md)|[deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md)|Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md).|
|[Обновление объекта deviceAppManagement](../api/intune-unlock-deviceappmanagement-update.md)|[deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md)|Обновление свойств объекта [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md).|

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
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



