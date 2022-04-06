---
title: тип ресурса simulationAutomation
description: Представляет автоматизацию моделирования, созданную для работы с клиентом.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 38f8bf63ef41053666a4bdd58121bd81e09fe51c
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758348"
---
# <a name="simulationautomation-resource-type"></a>тип ресурса simulationAutomation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет автоматизацию моделирования, созданную для работы с клиентом.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Моделирование спискаАтомации](../api/attacksimulationroot-list-simulationautomations.md)|[коллекция simulationAutomation](../resources/simulationautomation.md)|Получите список объектов [simulationAutomation](../resources/simulationautomation.md) и их свойств.|
|[Выполняется список](../api/simulationautomation-list-runs.md)|[коллекция simulationAutomationRun](../resources/simulationautomationrun.md)|Получите список запусков автоматизации моделирования атак для клиента.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[emailIdentity](../resources/emailidentity.md)|Удостоверение пользователя, создавшего автоматизацию моделирования атак.|
|createdDateTime|DateTimeOffset|Дата и время создания автоматизации моделирования атак.|
|description|String|Описание автоматизации моделирования атак.|
|displayName|String|Отображение имени автоматизации моделирования атак. Поддерживает `$filter` и `$orderby`.|
|id|String|Уникальный идентификатор для автоматизации имитации атак.|
|lastModifiedBy|[emailIdentity](../resources/emailidentity.md)|Удостоверение пользователя, который недавно изменил автоматизацию моделирования атак.|
|lastModifiedDateTime|DateTimeOffset|Дата и время, когда недавно была изменена автоматизация имитации атак.|
|lastRunDateTime|DateTimeOffset|Дата и время последнего запуска автоматизации моделирования атак.|
|nextRunDateTime|DateTimeOffset|Дата и время предстоящего запуска автоматизации моделирования атак.|
|status|[simulationAutomationStatus](#simulationautomationstatus-values)|Состояние автоматизации моделирования атак. Поддерживает `$filter` и `$orderby`. Допустимые значения: `unknown`, `draft`, `notRunning`, `running`, `completed`, `unknownFutureValue`.|

### <a name="simulationautomationstatus-values"></a>simulationAutomationStatus values

|Member|Описание |
|:---|:---|
|unknown| Состояние автоматизации моделирования не определено. |
|черновик| Автоматизация моделирования находится в режиме черновика. |
|notRunning| Автоматизация моделирования не запущена. |
|запуск| Автоматизация моделирования запущена. |
|завершено| Автоматизация моделирования завершена. |
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать. |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|выполняется|[коллекция simulationAutomationRun](../resources/simulationautomationrun.md)|Запускается коллекция автоматизации моделирования. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.simulationAutomation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationAutomation",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastRunDateTime": "String (timestamp)",
  "nextRunDateTime": "String (timestamp)",
  "status": "String"
}
```

