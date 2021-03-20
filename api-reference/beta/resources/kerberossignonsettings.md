---
title: тип ресурса kerberosSignOnSettings
description: Представляет параметры kerberos для локального приложения, опубликованного через Application Proxy.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: af00e70e1ef4603c1b1370ec5ef9e9ba75fecb4c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943665"
---
# <a name="kerberossignonsettings-resource-type"></a>тип ресурса kerberosSignOnSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры ограниченной делегирования Keberos (KCD) для ресурса [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) при публикации локального приложения с помощью прокси-сервера приложения Azure AD. Прокси-сервер приложения использует ограниченное делегирование Kerberos (KCD) для поддержки однорегистрирования в интегрированных приложениях проверки подлинности Windows. Дополнительные сведения см. в документе [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy.](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)

>[!NOTE]
>Не используйте это свойство для настройки единого знака SAML или пароля. Если вы настраивает SAML с одним входом, это должно быть установлено на [службеPrincipal.](serviceprincipal.md)
Если вы настраивает однонаправленный пароль, это необходимо установить с помощью [createPasswordSingleSignOnCredentials.](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|kerberosServicePrincipalName|Строка| SpN внутреннего приложения сервера приложений. Этот SPN должен быть в списке служб, которым соединитатель может представлять делегированную учетную данные. |
|kerberosSignOnMappingAttributeType|kerberosSignOnMappingAttributeType| Удостоверение делегирования входа, используемое соединитетелем от имени пользователей. Дополнительные сведения см. в ссылке Работа с различными [локальной и облачной идентификаторами. ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities) Возможные значения: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.kerberosSignOnSettings",
  "baseType": null
}-->

```json
{
  "kerberosServicePrincipalName": "String",
  "kerberosSignOnMappingAttributeType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "kerberosSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
