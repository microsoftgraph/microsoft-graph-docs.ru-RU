---
title: тип ресурса serviceHealthIssue
description: Представляет проблему со здоровьем службы в службе.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 6e650333ef84bf3dcc1f32688366b3760c0f622c66ddf26ab7393bfe85e453c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54177308"
---
# <a name="servicehealthissue-resource-type"></a>тип ресурса serviceHealthIssue

Пространство имен: microsoft.graph

Представляет проблему со здоровьем службы в службе.

Проблема со здоровьем службы может быть инцидентом службы или консультацией по обслуживанию. Например,

* Инцидент службы: "Exchange службы почтовых ящиков не существует".
* Рекомендации по обслуживанию: "Пользователи могут испытывать задержки в приеме сообщений электронной почты".

Наследует от [serviceAnnouncementBase](../resources/serviceannouncementbase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get serviceHealthIssue](../api/servicehealthissue-get.md)|[serviceHealthIssue](../resources/servicehealthissue.md)|Извлечение свойств и связей объекта [serviceHealthIssue.](../resources/servicehealthissue.md) |
|[Получить отчет о проверке после инцидента](../api/servicehealthissue-incidentreport.md)|Stream|Предоставляет отчет о происшествии после публикации (PIR) для указанной проблемы службы для клиента. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|classification|serviceHealthClassificationType|Тип проблемы со здоровьем службы. Возможные значения: `advisory`, `incident`, `unknownFutureValue`.|
|подробности|[Коллекция(keyValuePair)](../resources/keyvaluepair.md)|Дополнительные сведения о проблеме со здоровьем службы. Это свойство не поддерживает фильтры. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|endDateTime|DateTimeOffset|Время окончания проблемы службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|функция|String|Имя функции проблемы службы.|
|featureGroup|String|Имя группы функций проблемы службы.|
|id|String|Id проблемы службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|impactDescription|String|Описание влияния проблемы службы.|
|isResolved|Логическое|Указывает, устранена ли проблема.|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время проблемы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|происхождение|serviceHealthOrigin|Указывает происхождение проблемы службы. Возможные значения: `microsoft`, `thirdParty`, `customer`, `unknownFutureValue`.|
|posts|[Collection(serviceHealthIssuePost)](../resources/servicehealthissuepost.md)|Коллекция исторических сообщений для проблемы службы.|
|service|String|Указывает службу, затрагиваемую проблемой.|
|startDateTime|DateTimeOffset|Время начала выпуска службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|status|serviceHealthStatus|Состояние проблемы службы. Возможные значения: `serviceOperational` `investigating` , , , , `restoringService` , `verifyingService` , `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` .|
|title|String|Название проблемы службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|

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

