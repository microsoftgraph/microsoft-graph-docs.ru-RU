---
title: Тип ресурса Кербероссигнонсеттингс
description: Представляет параметры единого входа для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ebe5c584b009bd3028aece3cbfca75463f9c86dd
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862460"
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
|кербероссигнонсеттингс| [кербероссигнонсеттингс](kerberossignonsettings.md)| Параметры ограниченного делегирования Kerberos для приложений, использующих встроенную проверку подлинности Windows. |
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