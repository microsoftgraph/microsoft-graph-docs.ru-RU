---
title: Тип ресурса subjectRightsRequest
description: Представляет свойства запроса прав субъекта.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: b601530b71f8af9b84e1bf94b19b3b3332b12f21
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461235"
---
# <a name="subjectrightsrequest-resource-type"></a>Тип ресурса subjectRightsRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет свойства запроса прав субъекта, который является формальным запросом данных, подавным контроллеру, для выполнения действий с персональными данными. 

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление subjectRightsRequests](../api/subjectRightsRequest-list.md)|[Коллекция subjectRightsRequest](../resources/subjectRightsRequest.md)|Получение списка объектов [subjectRightsRequest](../resources/subjectRightsRequest.md) и их свойств.|
|[Создание subjectRightsRequest](../api/subjectRightsRequest-post.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|Создайте объект [subjectRightsRequest](../resources/subjectRightsRequest.md) .|
|[Получение subjectRightsRequest](../api/subjectRightsRequest-get.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|Чтение свойств и связей объекта [subjectRightsRequest](../resources/subjectRightsRequest.md) .|
|[Обновление subjectRightsRequest](../api/subjectRightsRequest-update.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|Обновление свойств объекта [subjectRightsRequest](../resources/subjectRightsRequest.md) .|
|[getFinalAttachment](../api/subjectRightsRequest-getfinalattachment.md)|Stream|Получение окончательного вложения для запроса. Вложение представляет собой ZIP-файл, содержащий все файлы, включенные администратором конфиденциальности.|
|[getFinalReport](../api/subjectRightsRequest-getfinalreport.md)|Stream|Получите окончательный отчет для запроса. Отчет представляет собой текстовый файл, содержащий сведения о файлах, включенных администратором конфиденциальности.|
|[Перечисление заметок](../api/subjectRightsRequest-list-notes.md)|[Коллекция authoredNote](../resources/authorednote.md)|Получите ресурсы authoredNote из свойства навигации примечаний.|
|[Создание authoredNote](../api/subjectRightsRequest-post-notes.md)|[authoredNote](../resources/authorednote.md)|Создайте объект authoredNote.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|assignedTo|[identity](../resources/identity.md)|Удостоверение, назначенное запросу.|
|closedDateTime|DateTimeOffset|Дата и время закрытия запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
| contentQuery         | Строка | KQL на основе запроса содержимого, который должен использоваться для поиска. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
|createdBy|[identitySet](../resources/identityset.md)|Сведения об удостоверении для сущности, создавшего запрос.|
|createdDateTime|DateTimeOffset|Дата и время создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
|dataSubject|[dataSubject](../resources/datasubject.md)|Сведения о субъекте данных.|
|dataSubjectType|dataSubjectType|Тип субъекта данных. Возможные значения: `customer`, `currentEmployee`, `formerEmployee`, `prospectiveEmployee`, `student`, `teacher`, `faculty`, `other`, `unknownFutureValue`.|
|description|Строка|Описание запроса.|
|displayName|String|Имя запроса.|
| externalId           | String| Внешний идентификатор запроса, который неизменяем после создания и используется для отслеживания запроса внешней системы. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
|Истории|[Коллекция subjectRightsRequestHistory](../resources/subjectrightsrequesthistory.md)|Коллекция событий изменения журнала.|
| includeAllVersions   | Boolean | Включите все версии документов. По умолчанию будут возвращены текущие копии документов. Если SharePoint сайтов включено управление версиями, включая все версии, будут включены исторические копии документов. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
| includeAuthoredContent| Boolean | Включите контент, созданный субъектом данных. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
|Понимание|[subjectRightsRequestDetail](../resources/subjectrightsrequestdetail.md)|Аналитические сведения о запросе.|
|internalDueDateTime|DateTimeOffset|Дата и время внутреннего выполнения запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Сведения об удостоверении сущности, которая в последний раз изменяла запрос.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
| mailboxLocations     | [subjectRightsRequestMailboxLocation](../resources/subjectrightsrequestmailboxlocation.md)|Расположения почтовых ящиков, в которых должен выполняться поиск. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
| pauseAfterEstimate   | Boolean| Приостановка запроса после завершения оценки. По умолчанию оценка данных будет выполняться, а затем приостанавливаться, что позволяет просмотреть результаты, а затем выбрать параметр для получения данных в пользовательском интерфейсе. Это свойство можно задать, `false` если требуется выполнить оценку, а затем автоматически начать с извлечения содержимого. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
|Правила|Коллекция String|Список нормативных требований, которые будет выполнять этот запрос.|
| siteLocations| [subjectRightsRequestSiteLocation](../resources/subjectrightsrequestsitelocation.md)| В SharePoint и OneDrive сайтов, в которых должен выполняться поиск. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
|stages|[Коллекция subjectRightsRequestStageDetail](../resources/subjectrightsrequeststagedetail.md)|Сведения о различных этапах запроса.|
|status|subjectRightsRequestStatus|Состояние запроса. Возможные значения: `active`, `closed`, `unknownFutureValue`.|
|type|subjectRightsRequestType|Тип запроса. Возможные значения: `export`, `delete`, `access`, `tagForAction`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|notes|[Коллекция authoredNote](../resources/authorednote.md)|Список заметок, связанных с запросом.|
|team|[team](../resources/team.md)|Сведения о Microsoft Teams, созданной для запроса.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subjectRightsRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
    "@odata.type": "#microsoft.graph.subjectRightsRequest",
    "contentQuery": "String",
    "closedDateTime": "String (timestamp)",
    "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "createdDateTime": "String (timestamp)",
    "dataSubject": {
        "@odata.type": "microsoft.graph.dataSubject"
    },
    "dataSubjectType": "customer",
    "description": "String",
    "displayName": "String",
    "externalId": "String",
    "id": "String (identifier)",
    "includeAllVersions": "Boolean",
    "includeAuthoredContent": "Boolean",
    "insight": {
        "@odata.type": "microsoft.graph.subjectRightsRequestDetail"
    },
    "internalDueDateTime": "String (timestamp)",
    "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "mailboxLocations": {
        "@odata.type": "microsoft.graph.subjectRightsRequestMailboxLocation"
    },
    "pauseAfterDownload": "Boolean",
    "regulations": [
        "String"
    ],
    "stages": [
        {
            "stage": "contentRetrieval",
            "status": "completed",
            "error": {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "contentReview",
            "status": "current",
            "error": {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "generateReport",
            "status": "notStarted",
            "error": {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "caseResolved",
            "status": "notStarted",
            "error": {
                "@odata.type": "microsoft.graph.publicError"
            }
        }
    ],
    "siteLocations": {
        "@odata.type": "microsoft.graph.subjectRightsRequestSiteLocation"
    },
    "status": "active",
    "team": {
        "@odata.type": "microsoft.graph.team"
    },
    "type": "access"
}
```

