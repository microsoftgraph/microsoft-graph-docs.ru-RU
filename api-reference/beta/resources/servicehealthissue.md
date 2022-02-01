---
title: тип ресурса serviceHealthIssue
description: Представляет проблему со здоровьем службы в службе.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 9126ca6ed06ce096d2748b7c01a9a61359099656
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291276"
---
# <a name="servicehealthissue-resource-type"></a>тип ресурса serviceHealthIssue

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет проблему со здоровьем службы в службе.

Проблема со здоровьем службы может быть инцидентом службы или консультацией по обслуживанию. Например.

* Инцидент службы: "Exchange службы почтовых ящиков не существует".
* Рекомендации по обслуживанию: "Пользователи могут испытывать задержки в приеме сообщений электронной почты".

Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get serviceHealthIssue](../api/servicehealthissue-get.md)|[serviceHealthIssue](../resources/servicehealthissue.md)|Извлечение свойств и связей объекта [serviceHealthIssue](../resources/servicehealthissue.md) . |
|[Получить отчет о проверке после инцидента](../api/servicehealthissue-incidentreport.md)|Stream|Получите документ отчета об инциденте после публикации (PIR) указанной проблемы службы для клиента. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|classification|serviceHealthClassificationType|Тип проблемы со здоровьем службы. Возможные значения: `advisory`, `incident`, `unknownFutureValue`.|
|details|Коллекция ([keyValuePair](../resources/keyvaluepair.md))|Дополнительные сведения о проблеме со здоровьем службы. Это свойство не поддерживает фильтры. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|endDateTime|DateTimeOffset|Время окончания проблемы службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|функция|String|Имя функции проблемы службы.|
|featureGroup|String|Имя группы функций проблемы службы.|
|id|String|Id проблемы службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|impactDescription|String|Описание влияния проблемы службы.|
|isResolved|Логическое|Указывает, устранена ли проблема.|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время проблемы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|происхождение|serviceHealthOrigin|Указывает происхождение проблемы службы. Возможные значения: `microsoft`, `thirdParty`, `customer`, `unknownFutureValue`.|
|posts|Collection([serviceHealthIssuePost](../resources/servicehealthissuepost.md))|Коллекция исторических сообщений для проблемы службы.|
|service|String|Указывает службу, затрагиваемую проблемой.|
|startDateTime|DateTimeOffset|Время начала выпуска службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|status|serviceHealthStatus|Состояние проблемы службы. Возможные значения: `serviceOperational`, `investigating`, `restoringService`, `verifyingService`, `serviceDegradation``serviceRestored``postIncidentReviewPublished`, `serviceInterruption`, `falsePositive``mitigated``resolved``investigationSuspended``extendedRecovery``resolvedExternal``confirmed``mitigatedExternal`, . `unknownFutureValue``reported` Дополнительные сведения см. в [материале serviceHealthStatus values](#servicehealthstatus-values).|
|title|String|Название проблемы службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|

### <a name="servicehealthstatus-values"></a>значения serviceHealthStatus
|Member|Описание|
|:---|:---|
|serviceOperational|Служба здорова, и никаких проблем не выявлено.|
|изучении|Была выявлена потенциальная проблема, и в настоящее время собираются дополнительные сведения о том, что происходит, и области воздействия.|
|restoringService|Причина проблемы установлена, и принимаются меры по приведению службы в нормальное состояние.|
|verifyingService|Для решения проблемы было принято решение, и мы проверяем, является ли служба полезной.|
|serviceRestored|Исправление устранено, а служба восстановлена в нормальном состоянии. Чтобы узнать, в чем было дело, просмотрите сведения о проблеме.|
|postIncidentReviewPublished|После инцидента был опубликован отчет по определенной проблеме, включаемой сведения о первопричине, с последующими действиями, чтобы подобная проблема не повторялась.|
|serviceDegradation|Подтверждена проблема, которая может повлиять на использование службы или функции. Это состояние может отображаться, если служба работает медленнее, чем обычно, периодически возникают прерывания или если недоступна определенная функция.|
|serviceInterruption|Вы увидите этот статус, если установлено, что проблема влияет на возможность доступа пользователей к службе. В этом случае проблема является значительной и ее можно воспроизвести.|
|extendedRecovery|Этот статус указывает на то, что для восстановления службы для большинства пользователей в настоящее время принимаются меры по исправлению положения, но для охвата всех затронутых систем необходимо некоторое время. Вы также можете увидеть этот статус, если будет сделано временное исправление, чтобы уменьшить влияние, пока постоянное исправление будет применено.|
|falsePositive|После подробного исследования служба будет подтверждена, что она будет работать в штатном режиме. Не обнаружено влияния на службу или причина инцидента находится за пределами службы. Инциденты и предупреждения с таким состоянием отображаются в представлении истории до истечения срока их действия (по истечении периода времени, определенного в последнем сообщении для этого события).|
|investigationSuspended|Если наше подробное исследование потенциальной проблемы приводит к запросу дополнительных сведений от клиентов, чтобы позволить группе службы исследовать далее, вы увидите этот статус. Если группе служб нужно действовать, они будут знать, какие данные или журналы им нужны.|
|resolved|Зарезервировано для последующего использования.|
|mitigatedExternal|Зарезервировано для последующего использования.|
|смягчение|Зарезервировано для последующего использования.|
|resolvedExternal|Зарезервировано для последующего использования.|
|подтверждено|Зарезервировано для последующего использования.|
|сообщается|Зарезервировано для последующего использования.|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealthIssue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssue",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "impactDescription": "String",
  "classification": "String",
  "origin": "String",
  "posts": [
    {
      "@odata.type": "microsoft.graph.serviceHealthIssuePost"
    }
  ],
  "status": "String",
  "service": "String",
  "feature": "String",
  "featureGroup": "String",
  "isResolved": "Boolean"
}
```

