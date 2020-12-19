---
title: Тип ресурса basicAuthentication
description: Представляет конфигурацию для использования базовой проверки подлинности в вызове API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9de5fad9746e8562f51d1ddc8fcea350c41979ed
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720442"
---
# <a name="basicauthentication-resource-type"></a>Тип ресурса basicAuthentication

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет конфигурацию для использования проверки подлинности HTTP Basic, которая влечет за собой имя пользователя и пароль, в вызове API. Имя пользователя и пароль отправляются в качестве загона авторизации, где находится кодированная версия username:password в кодированном коде `Basic {value}` `value` base 64.

Наследуется [от apiAuthenticationConfigurationBase.](../resources/apiauthenticationconfigurationbase.md)

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|username|String| Имя пользователя. |
|password|Строка| Пароль. Он не возвращается в ответах. |

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.basicAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.basicAuthentication",
  "password": "String",
  "username": "String"
}
```
