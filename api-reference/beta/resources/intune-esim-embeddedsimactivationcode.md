---
title: Тип ресурса embeddedSIMActivationCode
description: Встроенный код активации диспетчера установки как предоставленный оператором мобильной.
author: tfitzmac
ms.openlocfilehash: 4e768a4047b8ddc785b545d3b850128a8e44f256
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311790"
---
# <a name="embeddedsimactivationcode-resource-type"></a>Тип ресурса embeddedSIMActivationCode

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Встроенный код активации диспетчера установки как предоставленный оператором мобильной.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|integratedCircuitCardIdentifier|String.|Идентификатор карточки интегральной (ICCID) для данного встроенного кода активации диспетчера установки, предоставленный оператор мобильной связи.
Входные данные должно соответствовать следующим регулярным выражением: "^\[0-9\]{19}\[0-9\]?$".|
|matchingIdentifier|String.|MatchingIdentifier (MatchingID), указанный в GSMA связь SGP.22 Отклика технические спецификации раздел 4.1.
Входные данные должно соответствовать следующим регулярным выражением: "^\[a-zA-Z0-9\-\]* $".|
|smdpPlusServerAddress|String.|Полное доменное имя SM-DP + server технические спецификации Отклика SPG связи GSM.22.
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





