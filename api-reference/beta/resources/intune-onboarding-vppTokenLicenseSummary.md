---
title: Тип ресурса Впптокенлиценсесуммари
description: Сводка по лицензии для определенного приложения в маркере.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5182e9aebbefa1a1ce818e52cb442a8950b0b737
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301202"
---
# <a name="vpptokenlicensesummary-resource-type"></a>Тип ресурса Впптокенлиценсесуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по лицензии для определенного приложения в маркере.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|vppTokenId|String|Идентификатор токена VPP.|
|appleId|String|Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.|
|organizationName|Строка|Организация, связанная с токеном Apple Volume Purchase Program.|
|аваилаблелиценсекаунт|Int32|Число доступных лицензий VPP.|
|usedLicenseCount|Int32|Количество используемых лицензий VPP.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```




