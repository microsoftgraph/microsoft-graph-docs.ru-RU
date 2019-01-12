---
title: Тип ресурса vppTokenLicenseSummary
description: Сводка данного приложения в маркер лицензии.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0766fd4da996b57032154be98bbc22fd8c8a4a5b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939961"
---
# <a name="vpptokenlicensesummary-resource-type"></a>Тип ресурса vppTokenLicenseSummary

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сводка данного приложения в маркер лицензии.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|vppTokenId|String|Идентификатор маркера VPP.|
|appleId|String|Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.|
|organizationName|Строка|Организации, связанной с Apple тома покупки программа маркеров.|
|availableLicenseCount|Int32|Число доступных лицензий VPP.|
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





