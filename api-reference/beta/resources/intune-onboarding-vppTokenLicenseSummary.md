---
title: Тип ресурса Впптокенлиценсесуммари
description: Сводка по лицензии для определенного приложения в маркере.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47d56f27ac08d1b4ca657973cf6e5ae0690ba498
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527702"
---
# <a name="vpptokenlicensesummary-resource-type"></a>Тип ресурса Впптокенлиценсесуммари

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по лицензии для определенного приложения в маркере.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|vppTokenId|String|Идентификатор токена VPP.|
|appleId|String|Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.|
|organizationName|String|Организация, связанная с токеном Apple Volume Purchase Program.|
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



