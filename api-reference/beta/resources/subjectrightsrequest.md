---
title: тип ресурса subjectRightsRequest
description: Представляет свойства запроса на права субъекта.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 6aaa40989723309eb073c69aa22d53354bdbda7d
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60452107"
---
# <a name="subjectrightsrequest-resource-type"></a>тип ресурса subjectRightsRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет свойства запроса на права субъекта, который является формальным запросом субъекта данных контроллера для принятия действий по своим личным данным. 

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[List subjectRightsRequests](../api/subjectRightsRequest-list.md)|[коллекция subjectRightsRequest](../resources/subjectRightsRequest.md)|Получите список объектов [subjectRightsRequest](../resources/subjectRightsRequest.md) и их свойств.|
|[Создание subjectRightsRequest](../api/subjectRightsRequest-post.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|Создайте новый [объект subjectRightsRequest.](../resources/subjectRightsRequest.md)|
|[Get subjectRightsRequest](../api/subjectRightsRequest-get.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|Ознакомьтесь с свойствами и отношениями [объекта subjectRightsRequest.](../resources/subjectRightsRequest.md)|
|[Обновление subjectRightsRequest](../api/subjectRightsRequest-update.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|Обновление свойств объекта [subjectRightsRequest.](../resources/subjectRightsRequest.md)|
|[getFinalAttachment](../api/subjectRightsRequest-getfinalattachment.md)|Stream|Получите окончательное вложение для запроса. Вложение — это почтовый файл, содержащий все файлы, включенные администратором конфиденциальности.|
|[getFinalReport](../api/subjectRightsRequest-getfinalreport.md)|Stream|Получите окончательный отчет для запроса. Отчет — это текстовый файл, содержащий сведения о файлах, включенных администратором конфиденциальности.|
|[Заметки списка](../api/subjectRightsRequest-list-notes.md)|[authoredNote](../resources/authorednote.md) collection|Получите ресурсы authoredNote из свойства навигации примечаний.|
|[Создание authoredNote](../api/subjectRightsRequest-post-notes.md)|[authoredNote](../resources/authorednote.md)|Создание нового объекта authoredNote.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|assignedTo|[identity](../resources/identity.md)|Удостоверение, которое назначено запросу.|
|closedDateTime|DateTimeOffset|Дата и время закрытия запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|createdBy|[identitySet](../resources/identityset.md)|Сведения о удостоверениях для объекта, создающего запрос.|
|createdDateTime|DateTimeOffset|Дата и время создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
|dataSubject|[dataSubject](../resources/datasubject.md)|Сведения о субъекте данных.|
|dataSubjectType|dataSubjectType|Тип субъекта данных. Возможные значения: `customer`, `currentEmployee`, `formerEmployee`, `prospectiveEmployee`, `student`, `teacher`, `faculty`, `other`, `unknownFutureValue`.|
|description|String|Описание запроса.|
|displayName|String|Имя запроса.|
|история|[коллекция subjectRightsRequestHistory](../resources/subjectRightsRequesthistory.md)|Коллекция событий изменения истории.|
|insight|[subjectRightsRequestDetail](../resources/subjectRightsRequestdetail.md)|Сведения о запросе.|
|internalDueDateTime|DateTimeOffset|Дата и время, когда должен быть запротвирован внутренний запрос. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Сведения о удостоверениях для объекта, который в последний раз изменил запрос.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|нормативные акты|Коллекция строк|Список правил, которые будет выполнять этот запрос.|
|stages|[subjectRightsRequestStageDetail](../resources/subjectRightsRequeststagedetail.md) collection|Сведения о различных этапах запроса.|
|status|subjectRightsRequestStatus|Состояние запроса.. Возможные значения: `active`, `closed`, `unknownFutureValue`.|
|type|subjectRightsRequestType|Тип запроса. Возможные значения: `export`, `delete`, `access`, `tagForAction`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|notes|[authoredNote](../resources/authorednote.md) collection|Список заметок, ассицированных с запросом.|
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
    "type": "access",
    "dataSubjectType": "customer",
    "regulations": [
        "String"
    ],
    "displayName": "String",
    "description": "String",
    "status": "active",
    "internalDueDateTime": "String (timestamp)",
    "closedDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "id": "String (identifier)",
    "createdDateTime": "String (timestamp)",
    "stages": [
        {
            "stage": "contentRetrieval",
            "status": "completed",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "contentReview",
            "status": "current",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "generateReport",
            "status": "notStarted",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "caseResolved",
            "status": "notStarted",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        }
    ],
    "insight": {
        "@odata.type": "microsoft.graph.subjectRightsRequestDetail"
    },
    "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "dataSubject": {
        "@odata.type": "microsoft.graph.dataSubject",
    },
    "team": {
        "@odata.type": "microsoft.graph.team"
    }
}
```

