---
title: тип ресурса accessPackageAssignmentRequestRequirements
description: Определяет требования, необходимые для запроса указанного пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: febe429bb3c29da1a58454bb2758ee0fae16735b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259367"
---
# <a name="accesspackageassignmentrequestrequirements-resource-type"></a>тип ресурса accessPackageAssignmentRequestRequirements

Пространство имен: microsoft.graph

Представляет требования, которые должен выполнить звонячий для успешного создания **accessPackageAssignmentRequest** для **accessPackage,** указанного в URL-адресе. Требования определяются путем оценки политик, связанных с **accessPackage.** 

## <a name="properties"></a>Свойства
| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| existingAnswers | [коллекция accessPackageAnswer](../resources/accesspackageanswer.md)  | Ответы, которые уже предоставлены. |
| isApprovalRequired | Логический | Указывает, должен ли запрашивать одобрение утвердитель. |
| isApprovalRequiredForExtension  | Логический | Указывает, требуется ли утверждение, если пользователь пытается расширить доступ. |
| isCustomAssignmentScheduleAllowed | Логический | Указывает, разрешено ли запрашивать для настройки настраиваемой расписания. |
| isRequestorJustificationRequired | Логический | Указывает, должен ли запросчик предоставить обоснование при отправке запроса на назначение. |
| policyDescription | Строка | Описание политики, с помощью которую пользователь пытается запрашивать доступ.  |
| policyDisplayName | String | Отображает имя политики, с помощью которого пользователь пытается запрашивать доступ. |
| policyId | String | Идентификатор политики, с которую связаны эти требования. Этот идентификатор можно использовать при создании нового запроса на назначение. |
| вопросы | [коллекция accessPackageQuestion](../resources/accesspackagequestion.md) | Вопросы, настроенные в политике. Вопросы могут быть обязательными или необязательными; Звонители могут определить, является ли вопрос обязательным или необязательным на основе **свойства isRequired** в **accessPackageQuestion.** |
| schedule | [requestSchedule](../resources/requestschedule.md) | Расписание введенных ограничений, если таковые есть. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже приводится представление JSON этого типа.

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequestRequirements" 
}-->

``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequestRequirements",
  "policyId": "String",
  "policyDisplayName": "String",
  "policyDescription": "String",
  "isApprovalRequired": false,
  "isApprovalRequiredForExtension": false,
  "isCustomAssignmentScheduleAllowed": false,
  "isRequestorJustificationRequired": false,
  "schedule": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "questions": [
    {
      "@odata.type": "microsoft.graph.accessPackageQuestion"
    }
  ],
  "existingAnswers": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerString"
    }
  ]
}
```
