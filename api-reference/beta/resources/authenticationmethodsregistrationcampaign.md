---
title: тип ресурса authenticationMethodsRegistrationCampaign
description: Представляет параметры, используемые для запуска кампаний, чтобы подтолкнуть пользователей к настройке целевых методов проверки подлинности.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: be989bc86e5e708a89cd33c700e57edce42d9e50
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682935"
---
# <a name="authenticationmethodsregistrationcampaign-resource-type"></a>тип ресурса authenticationMethodsRegistrationCampaign

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры, используемые для запуска кампаний, чтобы подтолкнуть пользователей к настройке целевых методов проверки подлинности. Пользователям предложено настроить метод проверки подлинности после успешного выполнения задачи MFA. Доступно только для приложения Microsoft Authenticator для MFA.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|excludeTargets|[excludeTarget](../resources/excludetarget.md) collection|Пользователям и группам пользователей, которые не могут быть предложены к настройкам метода проверки подлинности.|
|includeTargets|[authenticationMethodsRegistrationCampaignIncludeTarget](../resources/authenticationmethodsregistrationcampaignincludetarget.md) collection|Пользователи и группы пользователей, которые могут настроить метод проверки подлинности.|
|snoozeDurationInDays|Int32|Указывает количество дней, когда пользователь снова видит подсказку, если он выбирает "Не сейчас" и не видит запрос. Минимум 0 дней. Максимум: 14 дней. Если значение "0" — пользователь получает запрос во время каждой попытки MFA.|
|state|advancedConfigState|Включить или отключить функцию. Возможные значения: `default`, `enabled`, `disabled`, `unknownFutureValue`. Значение используется, когда конфигурация не была явно заданная и использует для параметра поведение `default` Azure AD по умолчанию. Значение по умолчанию — `disabled`.|

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
  "snoozeDurationInDays": "Integer",
  "state": "String"
}
```
