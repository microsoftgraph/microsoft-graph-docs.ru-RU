---
title: Тип ресурса embeddedSIMActivationCode
description: Встроенный код активации диспетчера установки как предоставленный оператором мобильной.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: af8bf020953dbc014f42aa6d363d3ca9e30db8a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987407"
---
# <a name="embeddedsimactivationcode-resource-type"></a>Тип ресурса embeddedSIMActivationCode

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Встроенный код активации диспетчера установки как предоставленный оператором мобильной.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|integratedCircuitCardIdentifier|Строка|Идентификатор карточки интегральной (ICCID) для данного встроенного кода активации диспетчера установки, предоставленный оператор мобильной связи.
Входные данные должно соответствовать следующим регулярным выражением: "^\[0-9\]{19}\[0-9\]?$".|
|matchingIdentifier|Строка|MatchingIdentifier (MatchingID), указанный в GSMA связь SGP.22 Отклика технические спецификации раздел 4.1.
Входные данные должно соответствовать следующим регулярным выражением: "^\[a-zA-Z0-9\-\]* $".|
|smdpPlusServerAddress|Строка|Полное доменное имя SM-DP + server технические спецификации Отклика SPG связи GSM.22.
Входные данные должно соответствовать следующим регулярным выражением: "^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) *\.) +\[a-zA-Z\]{2,}$".|

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





