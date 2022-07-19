---
title: Тип ресурса caseOperation
description: Абстрактная сущность, представляющая длительный процесс.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 8c4dfce0e55cd8ff2e781b3bedad0a63adb3c87e
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839698"
---
# <a name="caseoperation-resource-type"></a>Тип ресурса caseOperation

Пространство имен: microsoft.graph.security



Наследует [от сущности](../resources/entity.md).

Абстрактная сущность, представляющая длительный процесс обнаружения электронных данных. Он содержит общий набор свойств, которые являются общими для наследуемых сущностей.  Сущности, производные от **caseOperation** :

- [Операция индексирования](../resources/security-ediscoveryindexoperation.md)
- [Операция удержания](../resources/security-ediscoveryholdoperation.md)
- [Операция оценки](../resources/security-ediscoveryestimateoperation.md)
- [Добавление для проверки операции набора](../resources/security-ediscoveryaddtoreviewsetoperation.md)
- [Операция тега](../resources/security-ediscoverytagoperation.md)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление caseOperations](../api/security-ediscoverycase-list-operations.md)|[Коллекция microsoft.graph.security.caseOperation](../resources/security-caseoperation.md)|Получение списка объектов [caseOperation](../resources/security-caseoperation.md) и их свойств.|
|[Получение caseOperation](../api/security-caseoperation-get.md)|[microsoft.graph.security.caseOperation](../resources/security-caseoperation.md)|Чтение свойств и связей объекта [caseOperation](../resources/security-caseoperation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|[microsoft.graph.security.caseAction](../resources/security-caseoperation.md#caseaction-values)| Тип действия, представляемого операцией. Возможные значения: `addToReviewSet`,,,`contentExport`,`convertToPdf``estimateStatistics``applyTags`,`purgeData`|
|completedDateTime|DateTimeOffset| Дата и время завершения операции. |
|createdBy|[identitySet](../resources/identityset.md)| Пользователь, создавшего операцию. |
|createdDateTime|DateTimeOffset| Дата и время создания операции. |
|id|Строка| Идентификатор операции. Только для чтения. |
|percentProgress|Int32| Ход выполнения операции. |
|resultInfo|[resultInfo](../resources/resultinfo.md)| Содержит сведения о результатах успешного выполнения и сбоя. |
|status|[microsoft.graph.security.caseOperationStatus](../resources/security-caseoperation.md#caseoperationstatus-values)| Состояние операции обращения. Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

### <a name="caseaction-values"></a>Значения caseAction

|Member|Описание|
|:----|-----------|
| addToReviewSet | Операция представляет добавление данных в набор проверки из коллекции обнаружения электронных данных. |
| applyTags | Операция представляет собой массовое добавление тегов к документам в наборе для проверки для указанного запроса набора проверки. |
| contentExport | Операция представляет экспорт содержимого из набора для проверки. |
| convertToPdf | Операция представляет собой преобразование документов в форматы PDF с отладчиками. |
| estimateStatistics  | Операция представляет поиск в службах Microsoft 365, таких как Exchange, SharePoint и OneDrive для бизнеса. |
| holdUpdate | Операция представляет собой обновление удержания по юридическим причинам (применение или удаление) для хранителей и источников данных, не влияемых на хранение.
| index | Операция представляет индексирование источников данных хранителей и источников данных, которые не являются хранителями, чтобы сделать их доступными для поиска. |
| purgeData | Операция представляет очистку содержимого из исходных рабочих нагрузок. |

### <a name="caseoperationstatus-values"></a>Значения caseOperationStatus

|Member|Описание|
|:----|-----------|
| notStarted | Операция еще не запущена. |
| submissionFailed | Сбой отправки операции. |
| Запущена | Операция в настоящее время выполняется. |
| Удалось | Операция успешно завершена без ошибок. |
| partiallySucceeded | Операция завершена, но произошли ошибки. Дополнительные сведения об ошибке см. [в разделе resultInfo](../resources/resultinfo.md). |
| Сбой при | Сбой операции. Дополнительные сведения об ошибке см. [в разделе resultInfo](../resources/resultinfo.md). |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.caseOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.caseOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "percentProgress": "Integer",
  "status": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```
