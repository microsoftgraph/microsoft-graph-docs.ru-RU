---
title: тип ресурса warrantyOffer
description: Модели и производство meatadata для управляемых устройств в учетной записи
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f8045dcc99c2c9e28099a39e54baa1e0561b5d2
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292461"
---
# <a name="warrantyoffer-resource-type"></a>тип ресурса warrantyOffer

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Модели и производство meatadata для управляемых устройств в учетной записи

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|type|[warrantyType](../resources/intune-devices-warrantytype.md)|Тип предложения гарантии. Возможные значения: `unknown`, `manufacturer`, `contractual`, `unknownFutureValue`.|
|description|String|Описание предложения по гарантии|
|startDateTime|DateTimeOffset|Дата начала предложения гарантии|
|endDateTime|DateTimeOffset|Дата окончания предложения по гарантии|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.warrantyOffer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.warrantyOffer",
  "type": "String",
  "description": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```




