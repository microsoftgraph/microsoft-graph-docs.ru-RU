---
title: Тип ресурса kerberosSignOnSettings
description: Представляет параметры единого знака для локального приложения, опубликованного через прокси-сервер приложения.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 85b2b4963c077b8dcb6ded4818ecc57bce635b39
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134871"
---
# <a name="onpremisespublishingsinglesignon-resource-type"></a>Тип ресурса onPremisesPublishingSingleSignOn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры единого входов для ресурса [onPremisesPublishing](onpremisespublishing.md) при публикации локального приложения с помощью прокси приложения Azure AD. Этот ресурс используется для настройки встроенной проверки подлинности Windows и проверки подлинности на основе загона в режиме единого входов. Дополнительные сведения см. в сведениях о ограниченном делегирования [Kerberos](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)для единого вход в приложения с помощью прокси приложения.

>[!NOTE]
>Не используйте это свойство для настройки SAML или единого вход на основе пароля. Если вы настраиваете единый вход SAML, это должно быть установлено в [servicePrincipal.](serviceprincipal.md)
Если вы настраиваете единый знак на основе пароля, его необходимо настроить с помощью [createPasswordSingleSignOnCredentials.](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|kerberosSignOnSettings| [kerberosSignOnSettings](kerberossignonsettings.md)| Параметры ограниченного делегирования Kerberos для приложений, которые используют встроенную проверку подлинности окон. |
|singleSignOnMode|Строка| Предпочтительный режим единого входов для приложения. Возможные значения: `none`, `onPremisesKerberos`, `headerBased`.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn",
  "baseType": null
}-->

```json
{
  "kerberosSignOnSettings": {"@odata.type": "microsoft.graph.kerberosSignOnSettings"},
  "singleSignOnMode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingSingleSignOn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
