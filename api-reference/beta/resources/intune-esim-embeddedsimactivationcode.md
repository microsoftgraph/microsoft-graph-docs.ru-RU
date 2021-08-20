---
title: тип ресурса embeddedSIMActivationCode
description: Встроенный код активации SIM-карты, предоставляемый мобильным оператором.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07acfbad5baf0cb68118472ea32d667c7f2868dac490665e61726fd5a6e4bf75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54242568"
---
# <a name="embeddedsimactivationcode-resource-type"></a>тип ресурса embeddedSIMActivationCode

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Встроенный код активации SIM-карты, предоставляемый мобильным оператором.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|интегрированныйCircuitCardIdentifier|Строка|Идентификатор интегрированной схемной карты (ICCID) для встроенного кода активации SIM-карты, как это предусмотрено мобильным оператором.
Вход должен соответствовать следующему регулярному выражению: "^ \[ 0-9 \] {19} \[ 0-9 \] ?$".|
|matchingIdentifier|String|MatchingIdentifier (MatchingID), как указано в разделе Технические спецификации GSMA Association SGP.22 RSP 4.1.
Вход должен соответствовать следующему регулярному выражению: "^ \[ a-zA-Z0-9 \- \] *$".|
|smdpPlusServerAddress|String|Полное доменное имя сервера SM-DP+, указанное в технической спецификации GSM Association SPG .22 RSP.
Вход должен соответствовать следующему регулярному выражению: '^( \[ a-zA-Z0-9 \] +(-a-zA-Z0-9 \[ \] +)* \. )+ \[ a-zA-Z \] {2,} $'.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```




