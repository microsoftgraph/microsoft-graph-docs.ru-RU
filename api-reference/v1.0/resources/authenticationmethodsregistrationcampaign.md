---
title: тип ресурса authenticationMethodsRegistrationCampaign
description: Представляет параметры, используемые для запуска кампаний, чтобы подтолкнуть пользователей к настройке целевых методов проверки подлинности.
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 71de25c16e357ade6aca9f2bb7fd5100cf8af7cd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019168"
---
# <a name="authenticationmethodsregistrationcampaign-resource-type"></a>тип ресурса authenticationMethodsRegistrationCampaign

Пространство имен: microsoft.graph

Представляет параметры, используемые для запуска кампаний, чтобы подтолкнуть пользователей к настройке целевых методов проверки подлинности. Пользователям предложено настроить метод проверки подлинности после успешного выполнения задачи MFA. Доступно только для приложения Microsoft Authenticator для MFA.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|excludeTargets|[excludeTarget](../resources/excludetarget.md) collection|Пользователям и группам пользователей, которые не могут быть предложены к настройкам метода проверки подлинности.|
|includeTargets|[authenticationMethodsRegistrationCampaignIncludeTarget](../resources/authenticationmethodsregistrationcampaignincludetarget.md) collection|Пользователи и группы пользователей, которые могут настроить метод проверки подлинности.|
|snoozeDurationInDays|Int32|Указывает количество дней, когда пользователь снова видит подсказку, если он выбирает "Не сейчас" и не видит запрос. Минимум: 0 дней. Максимум: 14 дней. Если значение "0", пользователь получает запрос во время каждой попытки MFA.|
|state|advancedConfigState|Включить или отключить функцию. Возможные значения: `default`, `enabled`, `disabled`, `unknownFutureValue`. Значение используется, когда конфигурация не была явно заданная и использует для параметра поведение Azure Active Directory `default` по умолчанию. Значение по умолчанию — `disabled`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaign",
  "excludeTargets": [
    {
      "@odata.type": "microsoft.graph.excludeTarget"
    }
  ],
  "includeTargets": [
    {
      "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
    }
  ],
  "snoozeDurationInDays": "Int32",
  "state": "String"
}
```
