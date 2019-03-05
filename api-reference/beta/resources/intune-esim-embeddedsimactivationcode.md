---
title: Тип ресурса Ембеддедсимактиватионкоде
description: Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 955dccb226332b297e30c4d40768f84936b04dbe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145229"
---
# <a name="embeddedsimactivationcode-resource-type"></a>Тип ресурса Ембеддедсимактиватионкоде

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ИнтегратедЦиркуиткардидентифиер|String|Идентификатор интегрированной цепи (ИКЦИД) для этого встроенного кода активации SIM-карты, предоставленный оператором мобильной связи.
входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ 0-9\]{19}\[0-9\]_км_ $ '.|
|Матчингидентифиер|String|Матчингидентифиер (Матчингид), как указано в разделе ГСМА Association СГП. 22 RSP, раздел 4,1.
Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ a –\-\]ZA ' Z0 – 9 * $ '.|
|Смдпплуссервераддресс|String|Полное доменное имя сервера SM — DP + Server, как указано в технической спецификации GSM Association СПГ .22 RSP.
Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ (a-\]Za-z0\[-9 + (-a-\]Za-z0\.-9\[+) *) +\]{2,}a-zA-Z $ '.|

## <a name="relationships"></a>Отношения
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




