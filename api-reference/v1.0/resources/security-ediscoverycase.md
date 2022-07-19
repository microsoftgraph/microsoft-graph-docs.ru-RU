---
title: Тип ресурса ediscoveryCase
description: В контексте обнаружения электронных данных содержатся хранители, удержания, коллекции и наборы проверки.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 3348c6c718a1ccd23977b4b1164cc21111198eac
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839920"
---
# <a name="ediscoverycase-resource-type"></a>Тип ресурса ediscoveryCase

Пространство имен: microsoft.graph.security



В контексте обнаружения электронных данных содержатся хранители, поисковые запросы, наборы проверки. Дополнительные сведения см[. в разделе "Обзор Microsoft Purview eDiscovery (Премиум)"](/microsoft-365/compliance/overview-ediscovery-20).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление ediscoveryCases](../api/security-casesroot-list-ediscoverycases.md)|[Коллекция microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md)|Получение списка объектов [ediscoveryCase](../resources/security-ediscoverycase.md) и их свойств.|
|[Создание ediscoveryCase](../api/security-casesroot-post-ediscoverycases.md)|[microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md)|Создайте объект [ediscoveryCase](../resources/security-ediscoverycase.md) .|
|[Получение ediscoveryCase](../api/security-ediscoverycase-get.md)|[microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md)|Чтение свойств и связей объекта [ediscoveryCase](../resources/security-ediscoverycase.md) .|
|[Обновление ediscoveryCase](../api/security-ediscoverycase-update.md)|[microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md)|Обновление свойств объекта [ediscoveryCase](../resources/security-ediscoverycase.md) .|
|[Удаление ediscoveryCase](../api/security-casesroot-delete-ediscoverycases.md)|Нет|Удаление объекта [ediscoveryCase](../resources/security-ediscoverycase.md) .|
|[Перечисление хранителей](../api/security-ediscoverycase-list-custodians.md)|[Коллекция microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Получите ресурсы ediscoveryCustodian из свойства навигации хранителей.|
|[Создание объекта ediscoveryCustodian](../api/security-ediscoverycase-post-custodians.md)|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Создайте объект ediscoveryCustodian.|
|[Перечисление объектов noncustodialDataSources](../api/security-ediscoverysearch-list-noncustodialsources.md)|[Коллекция microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Получите ресурсы ediscoveryNoncustodialDataSource из свойства навигации noncustodialDataSources.|
|[Создание объекта ediscoveryNoncustodialDataSource](../api/security-ediscoverycase-post-noncustodialdatasources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Создайте объект ediscoveryNoncustodialDataSource.|
|[Операции со списком](../api/security-ediscoverycase-list-operations.md)|[Коллекция microsoft.graph.security.caseOperation](../resources/security-caseoperation.md)|Получение ресурсов caseOperation из свойства навигации операций.|
|[Перечисление наборов reviewSets](../api/security-ediscoverycase-list-reviewsets.md)|[Коллекция microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Получите ресурсы ediscoveryReviewSet из свойства навигации reviewSets.|
|[Создание объекта ediscoveryReviewSet](../api/security-ediscoverycase-post-reviewsets.md)|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Создайте объект ediscoveryReviewSet.|
|[Поиск по спискам](../api/security-ediscoverycase-list-searches.md)|[Коллекция microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Получите ресурсы ediscoverySearch из свойства навигации поиска.|
|[Создание ediscoverySearch](../api/security-ediscoverycase-post-searches.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Создайте объект ediscoverySearch.|
|[Перечисление тегов](../api/security-ediscoverycase-list-tags.md)|[Коллекция microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Получите ресурсы ediscoveryReviewTag из свойства навигации тегов.|
|[Создание ediscoveryReviewTag](../api/security-ediscoverycase-post-tags.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Создайте объект ediscoveryReviewTag.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|closedBy|[Microsoft.graph.identitySet](../resources/identityset.md)|Пользователь, закрывавший дело.|
|closedDateTime|DateTimeOffset|Дата и время закрытия дела. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|createdBy|[Microsoft.graph.identitySet](/graph/api/resources/identityset)|Пользователь, создавший дело.|
|createdDateTime|DateTimeOffset|Дата и время создания сущности. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|description|Строка|Описание варианта.|
|displayName|String|Имя регистра.|
|externalId|String|Номер внешнего обращения для ссылки на клиента.|
|id|Строка|Идентификатор дела обнаружения электронных данных. Только для чтения. |
|lastModifiedBy|[Microsoft.graph.identitySet](../resources/identityset.md)|Последний пользователь, который изменил дело.
|lastModifiedDateTime|DateTimeOffset|Последняя дата и время изменения дела. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|status|microsoft.graph.security.caseStatus|Состояние обращения. Возможные значения: `unknown`, `active`, `pendingDelete`, , `closing`, и `closedWithError``closed`. Дополнительные сведения см. в следующей таблице.

### <a name="casestatus-values"></a>Значения caseStatus

|Member|Описание|
|:----|-----------|
| unknown | Состояние обращения неизвестно. |
| Активных | Регистр активен. |
| pendingDelete | Обращение было удалено, но удаление было выполнено не полностью. |
| Закрытие | Обращение закрыто, но операция не была полностью транзакция. |
| Закрыт | Обращение закрыто. |
| closedWithError | Дело закрыто, но в этом случае произошли ошибки, связанные с освобождением удержаний. |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|Хранителей|[Коллекция microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Возвращает список объектов **case ediscoveryCustodian** для этого **случая**.|
|noncustodialDataSources|[Коллекция microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Возвращает список объектов **case ediscoveryNoncustodialDataSource** для этого **случая**.|
|operations|[Коллекция microsoft.graph.security.caseOperation](../resources/security-caseoperation.md)|Возвращает список объектов **caseOperation** для этого **случая**.|
|reviewSets|[Коллекция microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Возвращает список объектов **eDiscoveryReviewSet** в деле.|
|Поиск|[Коллекция microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Возвращает список объектов **eDiscoverySearch** , связанных с этим делом.|
|settings|[microsoft.graph.security.ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md)|Возвращает список объектов **eDIscoverySettings** в деле.|
|tags|[Коллекция microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Возвращает список объектов **ediscoveryReviewTag** , связанных с этим делом.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryCase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryCase",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "closedDateTime": "String (timestamp)",
  "externalId": "String"
}
```

