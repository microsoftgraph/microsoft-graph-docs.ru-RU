---
title: Тип ресурса Ембеддедсимактиватионкоде
description: Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 28a2344c6e31e944074bc14a7c779a3f165e506a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469113"
---
# <a name="embeddedsimactivationcode-resource-type"></a>Тип ресурса Ембеддедсимактиватионкоде

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|интегратедЦиркуиткардидентифиер|String|Идентификатор интегрированной цепи (ИКЦИД) для этого встроенного кода активации SIM-карты, предоставленный оператором мобильной связи.
Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ 0-9\]{19}\[0-9\]? $ '.|
|матчингидентифиер|String|Матчингидентифиер (Матчингид), как указано в разделе ГСМА Association СГП. 22 RSP, раздел 4,1.
Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ a –\-\]ZA ' Z0 – 9 * $ '.|
|смдпплуссервераддресс|String|Полное доменное имя сервера SM — DP + Server, как указано в технической спецификации GSM Association СПГ .22 RSP.
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



