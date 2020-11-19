---
title: Тип ресурса Ембеддедсимактиватионкоде
description: Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea17bc01e37b8e44f3fc904918f76859a9fcb40f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288469"
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
Входные данные должны быть согласованы со следующим регулярным выражением: ' ^ \[ 0-9 \] {19} \[ 0-9 \] ? $ '.|
|матчингидентифиер|String|Матчингидентифиер (Матчингид), как указано в разделе ГСМА Association СГП. 22 RSP, раздел 4,1.
Входные данные должны быть согласованы со следующим регулярным выражением: ' ^ \[ a – ZA ' Z0 – 9 \- \] * $ '.|
|смдпплуссервераддресс|String|Полное доменное имя сервера SM — DP + Server, как указано в технической спецификации GSM Association СПГ .22 RSP.
Входные данные должны быть согласованы со следующим регулярным выражением: ' ^ ( \[ a-zA-Z0-9 \] + (- \[ a-zA-Z0-9 \] +) * \. ) + \[ a-zA-Z \] {2,} $ '.|

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




