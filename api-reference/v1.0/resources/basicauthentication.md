---
title: тип ресурса basicAuthentication
description: Представляет конфигурацию для использования базовой проверки подлинности в вызове API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 361d7f98f2d594ab6193103f9a67b969cbfe6d0cb1b97cd229b89ba9449402e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126678"
---
# <a name="basicauthentication-resource-type"></a>тип ресурса basicAuthentication

Пространство имен: microsoft.graph

Представляет конфигурацию для использования проверки подлинности HTTP Basic, которая влечет за собой имя пользователя и пароль, в вызове API. Имя пользователя и пароль отправляются в качестве загона авторизации в качестве базовой версии 64 кодированной версии `Basic {value}` `value` username:password.

Наследует [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|username|String| Имя пользователя. |
|password|Строка| Пароль. Он не возвращается в ответах. |

## <a name="relationships"></a>Связи

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
