---
title: Тип ресурса accessReviewInstanceDecisionItemResource
description: Каждый элемент принятия решений в проверке доступа представляет доступ субъекта к ресурсу. accessReviewInstanceDecisionItemResource представляет ресурс, связанный с элементом принятия решения.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3f35317538a1cac512e6f3dfc0997bb721ac9681
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698151"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>Тип ресурса accessReviewInstanceDecisionItemResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Каждый элемент принятия решений в проверке доступа представляет доступ субъекта к ресурсу. Ресурс идентифицируется объектом accessReviewInstanceDecisionItemResource.

[accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionitemresource.md) — это открытый тип, который позволяет передавать другие свойства и является базовым типом для следующих ресурсов: [accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource](accessreviewinstancedecisionitemaccesspackageassignmentpolicyresource.md), [accessReviewInstanceDecisionItemAzureRoleResource](accessreviewinstancedecisionitemazureroleresource.md) и [accessReviewInstanceDecisionItemServicePrincipalResource](accessreviewinstancedecisionitemserviceprincipalresource.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя ресурса|
|id|String|Идентификатор ресурса|
|type|Строка|Тип ресурса. Типы: `Group`, , `ServicePrincipal``DirectoryRole`, , `AzureRole``AccessPackageAssignmentPolicy`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
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
