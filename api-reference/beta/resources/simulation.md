---
title: тип ресурсов моделирования
description: Представляете кампанию моделирования атак и учебной кампании клиента.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: b61a361f92e1abd8e168e1a59eac68e4edab0c96
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979752"
---
# <a name="simulation-resource-type"></a>тип ресурсов моделирования

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляете кампанию моделирования атак и учебной кампании клиента.

Моделирование атак и обучение — это служба, доступная в [microsoft Defender для](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true)Office 365. Эта служба позволяет пользователям в клиенте испытать реалистичную доброкачественная фишинговая атака и учиться у нее. Служба позволяет администраторам клиентов имитировать, назначать тренинги и читать полученные сведения о поведении пользователей в интернете в фишинговых симуляторах. Служба предоставляет отчеты об имитации атак, которые помогают арендаторам выявлять пробелы в знаниях о безопасности, чтобы они могли дополнительно обучать пользователей снижению их восприимчивости к атакам. 

API моделирования и подготовки атак позволяет  администраторам клиентов перечислять [](report-m365defender-reports-overview.md) запущенные упражнения и тренинги моделирования, а также получать отчеты о полученных сведениях о поведении пользователей в интернете в фишинговых симуляторах. 

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Моделирование списка](../api/attacksimulationroot-list-simulations.md)|[коллекция моделирования](../resources/simulation.md)|Получите список объектов [моделирования](../resources/simulation.md) и их свойств.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|attackTechnique|[simulationAttackTechnique](#simulationattacktechnique-values)|Метод социальной инженерии, используемый в кампании моделирования атак и обучения. Поддерживает `$filter` и `$orderby`. Возможные значения: `unknown`, `credentialHarvesting`, `attachmentMalware`, `driveByUrl`, `linkInAttachment`, `linkToMalwareFile`, `unknownFutureValue`. Дополнительные сведения о типах методов атак социальной инженерии см. в [симуляторах.](/microsoft-365/security/office-365-security/attack-simulation-training-get-started?view=o365-worldwide&preserve-view=true#simulations)|
|attackType|[simulationAttackType](#simulationattacktype-values)|Тип атаки для имитации атаки и учебной кампании. Поддерживает `$filter` и `$orderby`. Возможные значения: `unknown`, `social`, `cloud`, `endpoint`, `unknownFutureValue`.|
|cleanupArtifacts|Логический|Флаг, представляющий, были ли артефакты очищены в ходе имитации атаки и учебной кампании.|
|completionDateTime|DateTimeOffset|Дата и время завершения имитации атаки и учебной кампании. Поддерживает `$filter` и `$orderby`.|
|createdBy|[emailIdentity](../resources/emailidentity.md)|Удостоверение пользователя, создавшего имитацию атаки и обучающую кампанию.|
|createdDateTime|DateTimeOffset|Дата и время создания кампании моделирования атак и обучения.|
|description|Строка|Описание кампании моделирования атак и учебной кампании.|
|displayName|Строка|Отображение имени кампании моделирования атак и учебной кампании. Поддерживает `$filter` и `$orderby`.|
|enableRegionTimezoneDelivery|Логический|Флаг, представляющий, включить или отключить доставку полезной нагрузки фишинговых служб в кампании моделирования атак и обучения.|
|id|Строка|ID кампании моделирования атак и учебной кампании.|
|includeAllAccountTargets|Логический|Флаг, представляющий включение всех пользователей клиента в кампанию моделирования атак и обучения.|
|isAutomated|Boolean|Флаг, представляющий, была ли кампания моделирования атаки и учебной кампании создана из потока автоматизации моделирования. Поддерживает `$filter` и `$orderby`. |
|lastModifiedBy|[emailIdentity](../resources/emailidentity.md)|Удостоверение пользователя, который недавно изменил имитацию атаки и обучающую кампанию.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последней модификации кампании моделирования и обучения атак.|
|launchDateTime|DateTimeOffset|Дата и время запуска и начала кампании моделирования и обучения атак. Поддерживает `$filter` и `$orderby`.|
|mode|[simulationMode](#simulationmode-values)|Режим имитации атаки и учебной кампании. Поддерживает `$filter` и `$orderby`. Возможные значения: `real`, `preview`, `unknownFutureValue`.|
|payloadDeliveryPlatform|payloadDeliveryPlatform|Метод доставки полезной нагрузки фишинга, используемой в кампании моделирования атак и обучения. Возможные значения: `unknown`, `sms`, `email`, `teams`, `unknownFutureValue`.|
|payloadSource|[payloadSource](#payloadsource-values)|Источник фишинговой полезной нагрузки в кампании моделирования атак и обучения. Возможные значения: `unknown`, `global`, `tenant`, `unknownFutureValue`.|
|отчет|[simulationReport](../resources/simulationreport.md)|Отчет об имитации атаки и учебной кампании.|
|status|simulationStatus|Состояние кампании моделирования атак и обучения. Поддерживает `$filter` и `$orderby`. Возможные значения: `unknown`, `draft`, `inProgress`, `scheduled`, `completed`, `partiallyCompleted`, `failed`, `cancelled`, `excluded`, `deleted`, `included`, `unknownFutureValue`.|
|trainingAssignmentPreference|[trainingAssignmentPreference](#trainingassignmentpreference-values)|Предпочтение администратора клиента для назначения обучения пользователей в кампании моделирования атак и обучения. Возможные значения: `unknown`, `auto`, `manual`, `unknownFutureValue`.|
|trainingContentPreference|[trainingContentPreference](#trainingcontentpreference-values)|Предпочтение администратора клиента для источника обучающего контента, назначаемого пользователям в кампании моделирования атак и обучения. Возможные значения: `unknown`, `microsoft`, `custom`, `noTraining`, `unknownFutureValue`.|
|trainingDueDateTime|DateTimeOffset|Дата и время, до которых необходимо завершить обучение пользователей в кампании моделирования атак и обучения.|

### <a name="simulationattacktechnique-values"></a>значения simulationAttackTechnique

|Member|Описание |
|:---|:---|
|unknown| Техника атаки не определена. |
|credentialHarvesting| Метод атаки, который включает конечный пользователь, поставляющий учетные данные. |
|attachmentMalware| Метод атаки, который включает в себя нажатие вложения конечным пользователем. |
|driveByUrl| Метод атаки, который включает в себя, что конечный пользователь щелкнуть ссылку URL-адрес в фишинговой полезной нагрузки. |
|linkInAttachment| Метод атаки, который включает в себя нажатие конечным пользователем ссылки URL-адреса в вложении. |
|linkToMalwareFile| Метод атаки, который включает в себя, что конечный пользователь щелкнув URL-ссылку на файл вредоносных программ. |
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать. |

### <a name="simulationattacktype-values"></a>значения simulationAttackType

|Member|Описание |
|:---|:---|
|unknown| Тип атаки не определен. |
|социальные| Атака, которая использует социальные навыки для психологического управления жертвами, создавая ложное чувство любопытства, срочности или страха. |
|облако| Атака на хост или пользователя в облачной среде, например, отказ в атаках на службу.|
|конечная точка| Атака на конечные точки корпоративной сети, такие как настольные компьютеры, ноутбуки, мобильные телефоны, устройства интернета вещей. |
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать. |

### <a name="simulationmode-values"></a>значения simulationMode

|Member|Описание |
|:---|:---|
|real| Кампания запущена для всех необходимых конечных пользователей. |
|preview| Кампания, запущенная только пользователю администратора для предварительного просмотра полученной полезной нагрузки фишинга. |
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать. |

### <a name="payloadsource-values"></a>значения payloadSource

|Member|Описание |
|:---|:---|
|unknown| Источник полезной нагрузки не определен. |
|глобальный| Полезной нагрузки из коллекции полезной нагрузки, поставляемой Корпорацией Майкрософт. |
|клиент| Полезной нагрузки из коллекции полезной нагрузки, поставляемой клиентом. |
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать. |

### <a name="trainingassignmentpreference-values"></a>значения trainingAssignmentPreference

|Member|Описание |
|:---|:---|
|unknown| Предпочтение назначения обучения не определено. |
|Авто| Назначение учебных занятий конечным пользователям на основе заранее определенных критериев. |
|Вручную| Назначение учебных занятий конечным пользователям на основе критериев, определенных администратором. |
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать. |

### <a name="trainingcontentpreference-values"></a>значения trainingContentPreference

|Member|Описание |
|:---|:---|
|unknown| Предпочтения обучающего контента не определены. |
|Microsoft| Обучение контенту из коллекции тренингов, предоставленных Корпорацией Майкрософт. |
|настраиваемый| Обучение контента, предоставленного клиентом. |
|noTraining| Нет назначения обучения конечным пользователям в рамках кампании. |
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.simulation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulation",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "attackType": "String",
  "attackTechnique": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "launchDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "includeAllAccountTargets": "Boolean",
  "enableRegionTimezoneDelivery": "Boolean",
  "mode": "String",
  "isAutomated": "Boolean",
  "cleanupArtifacts": "Boolean",
  "payloadSource": "String",
  "payloadDeliveryPlatform": "String",
  "trainingAssignmentPreference": "String",
  "trainingContentPreference": "String",
  "trainingDueDateTime": "String (timestamp)",
  "report": {
    "@odata.type": "microsoft.graph.simulationReport"
  }
}
```


## <a name="see-also"></a>См. также
- [Имитация фишинговой атаки](/microsoft-365/security/office-365-security/attack-simulation-training?view=o365-worldwide&preserve-view=true)
- [Начало работы с обучением имитации атак.](/microsoft-365/security/office-365-security/attack-simulation-training-get-started?view=o365-worldwide&preserve-view=true#simulations)
