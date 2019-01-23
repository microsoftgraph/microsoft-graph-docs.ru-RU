---
title: Тип ресурса unsupportedDeviceConfigurationDetail
description: Описание причины сущности не поддерживается.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c03bdb20fc4c48fa7820e09b9212bf73250599aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400391"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>Тип ресурса unsupportedDeviceConfigurationDetail

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описание причины сущности не поддерживается.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|message|String|Сообщение о том, почему сущности не поддерживается.|
|propertyName|String|Если сообщение относится к определенное свойство в исходной сущности, а затем имя этого свойства.|

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




