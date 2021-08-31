---
title: тип ресурса embeddedSIMActivationCode
description: Встроенный код активации SIM-карты, предоставляемый мобильным оператором.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 68c900ce67f5eff6e7f9f5d9f3078f92fe60686d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787843"
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
|matchingIdentifier|Строка|MatchingIdentifier (MatchingID), как указано в разделе Технические спецификации GSMA Association SGP.22 RSP 4.1.
Вход должен соответствовать следующему регулярному выражению: "^ \[ a-zA-Z0-9 \- \] *$".|
|smdpPlusServerAddress|Строка|Полное доменное имя сервера SM-DP+, указанное в технической спецификации GSM Association SPG .22 RSP.
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



