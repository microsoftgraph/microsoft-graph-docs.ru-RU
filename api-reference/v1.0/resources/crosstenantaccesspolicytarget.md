---
title: Тип ресурса crossTenantAccessPolicyTarget
description: Определяет, как настроить параметры политики межтенантного доступа. Параметры могут быть нацелены на определенных пользователей, группы или приложения.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 19f58264312d8f1b519d9de9b6f66365c29f0def
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604739"
---
# <a name="crosstenantaccesspolicytarget-resource-type"></a>Тип ресурса crossTenantAccessPolicyTarget

Пространство имен: microsoft.graph

Определяет, как настроить параметры политики межтенантного доступа. Параметры могут быть нацелены на определенных пользователей, группы или приложения. Можно также использовать ключевые слова для конкретных групп или приложений.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| target | String | Уникальный идентификатор пользователя, группы или приложения; Одно из следующих ключевых слов: `AllUsers` или `AllApplications`для целевых объектов, которые являются приложениями, можно использовать [зарезервированные значения](#reserved-values-for-targets-that-are-applications). |
| Targettype | crossTenantAccessPolicyTargetType | Тип ресурса, на который вы хотите нацелить. Допустимые значения: `user`, `group`, `application`, `unknownFutureValue`. |

### <a name="reserved-values-for-targets-that-are-applications"></a>Зарезервированные значения для целевых объектов, которые являются приложениями

При настройке целевых объектов приложения можно также использовать следующие зарезервированные значения:

| Символ | Описание |
|:---|:---|
| AllMicrosoftApps | Относится к любому [облачному приложению Майкрософт](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps#microsoft-cloud-applications). |
| Office365 | Включает приложения, упомянутые в составе [набора Office365](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps#office-365) . |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyTarget"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyTarget",
  "target": "String",
  "targetType": "microsoft.graph.crossTenantAccessPolicyTargetType"
}
```
