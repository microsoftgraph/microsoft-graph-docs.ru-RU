---
title: Тип ресурса embeddedSIMActivationCode
description: Встроенный код активации диспетчера установки как предоставленный оператором мобильной.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74f1725ab8f12cb103144dc1897e9bf965c5361b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422469"
---
# <a name="embeddedsimactivationcode-resource-type"></a>Тип ресурса embeddedSIMActivationCode

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Встроенный код активации диспетчера установки как предоставленный оператором мобильной.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|integratedCircuitCardIdentifier|String|Идентификатор карточки интегральной (ICCID) для данного встроенного кода активации диспетчера установки, предоставленный оператор мобильной связи.
Входные данные должно соответствовать следующим регулярным выражением: "^\[0-9\]{19}\[0-9\]?$".|
|matchingIdentifier|String|MatchingIdentifier (MatchingID), указанный в GSMA связь SGP.22 Отклика технические спецификации раздел 4.1.
Входные данные должно соответствовать следующим регулярным выражением: "^\[a-zA-Z0-9\-\]* $".|
|smdpPlusServerAddress|String|Полное доменное имя SM-DP + server технические спецификации Отклика SPG связи GSM.22.
Входные данные должно соответствовать следующим регулярным выражением: "^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) *\.) +\[a-zA-Z\]{2,}$".|

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




