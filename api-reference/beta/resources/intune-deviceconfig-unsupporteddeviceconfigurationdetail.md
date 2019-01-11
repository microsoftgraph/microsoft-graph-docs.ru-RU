---
title: Тип ресурса unsupportedDeviceConfigurationDetail
description: Описание причины сущности не поддерживается.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0a213961e6b816917b061bc56c792cf9a60e3a2a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839475"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>Тип ресурса unsupportedDeviceConfigurationDetail

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Описание причины сущности не поддерживается.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|message|String|Сообщение о том, почему сущности не поддерживается.|
|propertyName|Строка|Если сообщение относится к определенное свойство в исходной сущности, а затем имя этого свойства.|

## <a name="relationships"></a>Связи
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





