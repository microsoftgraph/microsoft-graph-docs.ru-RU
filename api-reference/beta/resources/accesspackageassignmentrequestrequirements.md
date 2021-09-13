---
title: тип ресурса accessPackageAssignmentRequestRequirements
description: Определяет требования, необходимые для запроса указанного пакета доступа.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5c30389c99ed550635e48713a1ad6fa449c66814
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057959"
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
| isCustomAssignmentScheduleAllowed | Логическое | Указывает, разрешено ли запрашивать для настройки настраиваемой расписания. |
| isRequestorJustificationRequired | Логическое | Указывает, должен ли запросчик предоставить обоснование при отправке запроса на назначение. |
| policyDescription | String | Описание политики, с помощью которую пользователь пытается запрашивать доступ.  |
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
