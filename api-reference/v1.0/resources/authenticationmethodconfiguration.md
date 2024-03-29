---
title: authenticationMethodConfigurations
description: объект authenticationMethodConfigurations.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b7dee4297fb00dd54e9f9b8edf19da00c866a0f4
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2022
ms.locfileid: "62238975"
---
# <a name="authenticationmethodconfiguration-resource-type"></a>тип ресурса authenticationMethodConfiguration
Пространство имен: microsoft.graph

Это абстрактный тип, который представляет параметры для каждого метода проверки подлинности. Он имеет конфигурацию включения или отключения определенного метода проверки подлинности для клиента, а также возможности регистрации и использования этого метода пользователями и группами.

Следующие методы проверки подлинности вытекают из типа ресурса **authenticationMethodConfiguration:**
+ [emailAuthenticationMethodConfiguration](emailauthenticationmethodconfiguration.md)
+ [fido2AuthenticationMethodConfiguration](fido2authenticationmethodconfiguration.md)
+ [MicrosoftAuthenticatorAuthenticationMethodConfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Имя политики.|
|state|authenticationMethodState|Состояние политики. Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```
