---
title: Тип ресурса Кербероссигнонсеттингс
description: Представляет параметры единого входа для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f07fc81fee6fdc8e8ff3b55c246facdc4f155d11
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556444"
---
# <a name="onpremisespublishingsinglesignon-resource-type"></a>Тип ресурса Онпремисеспублишингсинглесигнон

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры единого входа для ресурса [онпремисеспублишинг](onpremisespublishing.md) при публикации локального приложения с помощью прокси приложения Azure AD. Этот ресурс используется для настройки встроенной проверки подлинности Windows и проверки подлинности на основе заголовков в режиме единого входа. Дополнительные сведения см. в статье [ограниченное делегирование Kerberos для единого входа в приложения с помощью прокси-сервера приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).

>[!NOTE]
>Не используйте это свойство для настройки SAML или единого входа на основе пароля. Если настраивается единый вход SAML, необходимо задать параметр [servicePrincipal](serviceprincipal.md).
Если вы настраиваете одиночный символ на основе пароля, его необходимо задать с помощью [креатепассвордсинглесигнонкредентиалс](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|кербероссигнонсеттингс| [кербероссигнонсеттингс](kerberossignonsettings.md)| Параметры ограниченного делегирования Kerberos для приложения. |
|синглесигнонмоде|String| Предпочтительный режим единого входа для приложения. Возможные значения: `none`, `onPremisesKerberos`, `headerBased`.|

## <a name="json-representation"></a>Представление JSON

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
  "KerberosSignOnSettings": {"@odata.type": "microsoft.graph.kerberosSignOnSettings"},
  "SingleSignOnMode": "String"
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