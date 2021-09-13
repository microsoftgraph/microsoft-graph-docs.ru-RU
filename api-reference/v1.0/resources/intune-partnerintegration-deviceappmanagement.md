---
title: Тип ресурса deviceAppManagement
description: Единичный объект управления приложениями на устройствах.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d88fc5b27d0abc622891d03f3dc5bcd36309fd84
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072031"
---
# <a name="deviceappmanagement-resource-type"></a>Тип ресурса deviceAppManagement

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Единичный объект управления приложениями на устройствах.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceAppManagement](../api/intune-partnerintegration-deviceappmanagement-get.md)|[deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md)|Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md).|
|[Обновление объекта deviceAppManagement](../api/intune-partnerintegration-deviceappmanagement-update.md)|[deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md)|Обновление свойств объекта [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md).|

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




