---
title: тип ресурса crossTenantAccessPolicyTarget
description: 'Определяет, как нацелить параметры политики доступа между клиентами. Параметры могут быть ориентированы на определенных пользователей, группы или приложения.'
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicytarget-resource-type"></a>тип ресурса crossTenantAccessPolicyTarget

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, как нацелить параметры политики доступа между клиентами. Параметры могут быть ориентированы на определенных пользователей, группы или приложения. Вы также можете использовать ключевые слова для целевых групп или приложений.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| target | Строка | Уникальный идентификатор пользователя, группы или приложения; одно из следующих ключевых слов: `AllUsers` и `AllApplications`( или для целей, которые являются приложениями, можно использовать [зарезервированные значения](#reserved-values-for-targets-that-are-applications). |
| targetType | crossTenantAccessPolicyTargetType | Тип ресурса, на который нужно нацелить. Допустимые значения: `user`, `group`, `application`, `unknownFutureValue`. |

### <a name="reserved-values-for-targets-that-are-applications"></a>Зарезервированные значения для целей, которые являются приложениями

При настройке целей приложения можно также использовать следующие зарезервированные значения:

| Символ | Описание |
|:---|:---|
| AllMicrosoftApps | Относится к [любому облачному приложению Майкрософт](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps#microsoft-cloud-applications). |
| Office365 | Включает приложения, упомянутые в [пакете Office365](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps#office-365) . |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

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
