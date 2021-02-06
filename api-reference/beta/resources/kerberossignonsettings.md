---
title: Тип ресурса kerberosSignOnSettings
description: Представляет параметры kerberos для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 0220d6d85c7aafe3489e4099a2c6b1837a7439e2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130089"
---
# <a name="kerberossignonsettings-resource-type"></a>Тип ресурса kerberosSignOnSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры ограниченного делегирования Keberos (KCD) для ресурса [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) при публикации локального приложения через прокси приложения Azure AD. Прокси приложения использует ограниченное делегирование Kerberos (KCD) для поддержки единого вход в интегрированные приложения проверки подлинности Windows. Дополнительные сведения см. в сведениях о ограниченном делегирования [Kerberos](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)для единого вход в приложения с помощью прокси приложения.

>[!NOTE]
>Не используйте это свойство для настройки samL или единого вход на основе пароля. Если вы настраиваете единый вход SAML, это должно быть установлено в [servicePrincipal.](serviceprincipal.md)
При настройке единого знака на основе пароля этот код необходимо настроить с помощью [createPasswordSingleSignOnCredentials.](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|kerberosServicePrincipalName|Строка| Внутреннее spN приложения сервера приложений. Это SPN должно быть в списке служб, которым соединители могут представлять делегированную учетную данные. |
|kerberosSignOnMappingAttributeType|Строка| Делегированная идентификация для входа в систему, используемая соединитетелем от имени пользователей. Дополнительные сведения см. в работе с различными идентификаторами локальной и [облачной платформы. ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities) Возможные значения: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.|

## <a name="json-representation"></a>Представление в формате JSON

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
