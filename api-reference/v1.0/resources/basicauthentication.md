---
title: тип ресурса basicAuthentication
description: Представляет конфигурацию для использования базовой проверки подлинности в вызове API.
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9749d179ffa33020b73747e46ed21add6eb9316d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019400"
---
# <a name="basicauthentication-resource-type"></a>тип ресурса basicAuthentication

Пространство имен: microsoft.graph

Представляет конфигурацию для использования проверки подлинности HTTP Basic, которая влечет за собой имя пользователя и пароль, в вызове API. Имя пользователя и пароль отправляются в качестве загона авторизации в качестве базовой версии 64 кодированной версии `Basic {value}` `value` username:password.

Наследует [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|username|Строка| Имя пользователя. |
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
