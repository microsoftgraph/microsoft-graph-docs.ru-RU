---
title: Тип ресурса Енкриптионрепортполицидетаилс
description: Сведения о политике для отчета о шифровании
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c9903b54483fc6f77cd183abee0e54b10acf9cc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771014"
---
# <a name="encryptionreportpolicydetails-resource-type"></a>Тип ресурса Енкриптионрепортполицидетаилс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о политике для отчета о шифровании

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Полициид|String|Идентификатор политики для отчета о шифровании|
|policyName|String|Имя политики для отчета о шифровании|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptionReportPolicyDetails",
  "policyId": "String",
  "policyName": "String"
}
```





