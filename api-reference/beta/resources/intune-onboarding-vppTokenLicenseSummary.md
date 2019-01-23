---
title: Тип ресурса vppTokenLicenseSummary
description: Сводка данного приложения в маркер лицензии.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8fb84a549d95459db1e4b39c11b526f73db08752
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395183"
---
# <a name="vpptokenlicensesummary-resource-type"></a>Тип ресурса vppTokenLicenseSummary

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка данного приложения в маркер лицензии.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|vppTokenId|String|Идентификатор маркера VPP.|
|appleId|String|Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.|
|organizationName|Строка|Организации, связанной с Apple тома покупки программа маркеров.|
|availableLicenseCount|Int32|Число доступных лицензий VPP.|
|usedLicenseCount|Int32|Количество используемых лицензий VPP.|

## <a name="relationships"></a>Отношения
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




