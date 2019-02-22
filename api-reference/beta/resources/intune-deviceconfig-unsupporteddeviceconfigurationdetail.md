---
title: Тип ресурса Унсуппортеддевицеконфигуратиондетаил
description: Описание причин неподдерживаемого объекта.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ebdb6eb91dd64c1605288cc0cb1260f8fe7440a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148470"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>Тип ресурса Унсуппортеддевицеконфигуратиондетаил

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описание причин неподдерживаемого объекта.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|message|String|Сообщение С объяснением, почему объект не поддерживается.|
|propertyName|String|Если сообщение связано с определенным свойством в исходной сущности, то имя этого свойства.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```




