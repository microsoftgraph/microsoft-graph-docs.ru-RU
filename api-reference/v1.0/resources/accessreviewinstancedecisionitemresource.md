---
title: accessReviewInstanceDecisionItemResource type
description: Представляет ресурс, связанный с элементом решения.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fadfa73ca826c7f38ea179e80abf429c9092e071
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161111"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>accessReviewInstanceDecisionItemResource type

Пространство имен: microsoft.graph

Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу. Ресурс идентифицирован объектом accessReviewInstanceDecisionItemResource. 

[accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionitemresource.md) — открытый тип, который позволяет передавать другие свойства и является базовым типом для следующих ресурсов: [accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource](accessreviewinstancedecisionitemaccesspackageassignmentpolicyresource.md), [accessReviewInstanceDecisionItemAzureRoleResource](accessreviewinstancedecisionitemazureroleresource.md)и [accessReviewInstanceDecisionItemServicePrincipalResource](accessreviewinstancedecisionitemserviceprincipalresource.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображение имени ресурса|
|id|Строка|Идентификатор ресурса|
|type|Строка|Тип ресурса. Типы включают: `Group` , , , , `ServicePrincipal` `DirectoryRole` `AzureRole` `AccessPackageAssignmentPolicy` .|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String"
}
```
