---
title: тип ресурсов моделирования
description: Представляет обучающую кампанию по имитации атак в клиенте.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: fbd043bd16176834c523d3b5083fab5ce69c406d
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757838"
---
# <a name="simulation-resource-type"></a>тип ресурсов моделирования

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет обучающую кампанию по имитации атак в клиенте.

Моделирование атак и обучение — это служба, доступная в [microsoft Defender для](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true) Office 365. Эта служба позволяет пользователям в клиенте испытать на себе реалистичную учебную фишинговую атаку и извлечь уроки. Служба позволяет администраторам клиентов имитировать, назначать тренинги и читать полученные сведения о поведении пользователей в интернете в фишинговых симуляторах. Служба предоставляет отчеты об имитации атак, которые помогают арендаторам выявлять пробелы в знаниях о безопасности, чтобы они могли дополнительно обучать пользователей снижению их восприимчивости к атакам.

API моделирования и подготовки атак позволяет администраторам клиентов перечислять  запущенные упражнения и тренинги моделирования, [](report-m365defender-reports-overview.md) а также получать отчеты о полученных сведениях о поведении пользователей в интернете в фишинговых симуляторах.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление симуляций](../api/attacksimulationroot-list-simulations.md)|[коллекция моделирования](../resources/simulation.md)|Получите список объектов [моделирования](../resources/simulation.md) и их свойств.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|attackTechnique|[simulationAttackTechnique](#simulationattacktechnique-values)|Метод социальной инженерии, используемый в кампании моделирования атак и обучения. Поддерживает `$filter` и `$orderby`. Возможные значения: `unknown`, `credentialHarvesting`, `attachmentMalware`, `driveByUrl`, `linkInAttachment`, `linkToMalwareFile`, `unknownFutureValue`. Дополнительные сведения о типах методов атак социальной инженерии см. в [симуляторах](/microsoft-365/security/office-365-security/attack-simulation-training-get-started?view=o365-worldwide&preserve-view=true#simulations).|
|attackType|[simulationAttackType](#simulationattacktype-values)|Тип атаки для имитации атаки и учебной кампании. Поддерживает `$filter` и `$orderby`. Возможные значения: `unknown`, `social`, `cloud`, `endpoint`, `unknownFutureValue`.|
|automationId|String|Уникальный идентификатор для автоматизации имитации атак.|
|completionDateTime|DateTimeOffset|Дата и время завершения имитации атаки и учебной кампании. Поддерживает `$filter` и `$orderby`.|
|createdBy|[emailIdentity](../resources/emailidentity.md)|Удостоверение пользователя, создавшего имитацию атаки и обучающую кампанию.|
|createdDateTime|DateTimeOffset|Дата и время создания кампании моделирования атак и обучения.|
|description|String|Описание кампании моделирования атак и учебной кампании.|
|displayName|String|Отображение имени кампании моделирования атак и учебной кампании. Поддерживает `$filter` и `$orderby`.|
|id|String|Уникальный идентификатор для имитации атаки и учебной кампании.|
|isAutomated|Логическое|Флаг, представляющий, была ли кампания моделирования атаки и учебной кампании создана из потока автоматизации моделирования. Поддерживает `$filter` и `$orderby`. |
|lastModifiedBy|[emailIdentity](../resources/emailidentity.md)|Удостоверение пользователя, который недавно изменил имитацию атаки и обучающую кампанию.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последней модификации кампании моделирования и обучения атак.|
|launchDateTime|DateTimeOffset|Дата и время запуска и начала кампании моделирования и обучения атак. Поддерживает `$filter` и `$orderby`.|
|payloadDeliveryPlatform|payloadDeliveryPlatform|Метод доставки полезной нагрузки фишинга, используемой в кампании моделирования атак и обучения. Возможные значения: `unknown`, `sms`, `email`, `teams`, `unknownFutureValue`.|
|отчет|[simulationReport](../resources/simulationreport.md)|Отчет об имитации атаки и учебной кампании.|
|status|[simulationStatus](#simulationstatus-values)|Состояние кампании моделирования атак и обучения. Поддерживает `$filter` и `$orderby`. Возможные значения: `unknown`, `draft`, `running`, `scheduled`, `succeeded`, `failed`, `cancelled`, `excluded`, `unknownFutureValue`.|

### <a name="simulationstatus-values"></a>значения simulationStatus

|Member|Описание |
|:---|:---|
|unknown| Состояние моделирования не определено. |
|черновик| Моделирование находится в режиме черновика. |
|запуск| Моделирование запущено. |
|scheduled| Моделирование запланировано. |
|успешно| Моделирование удалось. |
|не удалось| Моделирование не удалось. |
|отменено| Имитация отменяется. |
|исключено| Моделирование исключено. |
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать. |

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
  "isAutomated": "Boolean",
  "automationId": "String",
  "payloadDeliveryPlatform": "String",
  "report": {
    "@odata.type": "microsoft.graph.simulationReport"
  }
}
```


## <a name="see-also"></a>См. также
- [Имитация фишинговой атаки](/microsoft-365/security/office-365-security/attack-simulation-training?view=o365-worldwide&preserve-view=true)
- [Приступай к обучению имитации атак](/microsoft-365/security/office-365-security/attack-simulation-training-get-started?view=o365-worldwide&preserve-view=true#simulations).
