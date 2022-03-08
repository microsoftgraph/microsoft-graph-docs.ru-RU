---
title: authenticationMethodConfigurations
description: объект authenticationMethodConfigurations.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ea0c344b1930303a34d4844a2e484fe22fae7bb9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336923"
---
# <a name="authenticationmethodconfiguration-resource-type"></a>тип ресурса authenticationMethodConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Это абстрактный тип, который представляет параметры для каждого метода проверки подлинности. Он имеет конфигурацию включения или отключения определенного метода проверки подлинности для клиента, а также возможности регистрации и использования этого метода пользователями и группами.

Следующие методы проверки подлинности вытекают из типа ресурса **authenticationMethodConfiguration** :
+ [emailAuthenticationMethodConfiguration](emailauthenticationmethodconfiguration.md)
+ [fido2AuthenticationMethodConfiguration](fido2authenticationmethodconfiguration.md)
+ [MicrosoftAuthenticatorAuthenticationMethodConfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)
+ [smsAuthenticationMethodConfiguration](smsauthenticationmethodconfiguration.md)
+ [temporaryAccessPassAuthenticationMethodConfiguration](smsauthenticationmethodconfiguration.md)
+ [x509CertificateAuthenticationMethodConfiguration](x509certificateauthenticationmethodconfiguration.md)

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
