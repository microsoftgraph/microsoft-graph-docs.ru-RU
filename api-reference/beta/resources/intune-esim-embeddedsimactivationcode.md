---
title: Тип ресурса Ембеддедсимактиватионкоде
description: Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1e12a25db0beb124d00b2523607b40e899b4a01
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941340"
---
# <a name="embeddedsimactivationcode-resource-type"></a>Тип ресурса Ембеддедсимактиватионкоде

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ИнтегратедЦиркуиткардидентифиер|Строка|Идентификатор интегрированной цепи (ИКЦИД) для этого встроенного кода активации SIM-карты, предоставленный оператором мобильной связи.
Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ 0-9\]{19}\[0-9\]_км_ $ '.|
|Матчингидентифиер|Строка|Матчингидентифиер (Матчингид), как указано в разделе ГСМА Association СГП. 22 RSP, раздел 4,1.
Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ a –\-\]ZA ' Z0 – 9 * $ '.|
|Смдпплуссервераддресс|Строка|Полное доменное имя сервера SM — DP + Server, как указано в технической спецификации GSM Association СПГ .22 RSP.
Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ (a-\]Za-z0\[-9 + (-a-\]Za-z0\.-9\[+) *) +\]{2,}a-zA-Z $ '.|

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




