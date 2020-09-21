---
title: Тип ресурса Кербероссигнонсеттингс
description: Представляет параметры Kerberos для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c5d84b8f6ff80f146c02da1d29074181807b16c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079818"
---
# <a name="kerberossignonsettings-resource-type"></a>Тип ресурса Кербероссигнонсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры ограниченного делегирования Кеберос (ККД) для ресурса [онпремисеспублишингсинглесигнон](onpremisespublishingsinglesignon.md) при публикации локального приложения через прокси-сервер приложения Azure AD. Прокси приложения использует ограниченное делегирование Kerberos (ККД) для поддержки единого входа для встроенных приложений проверки подлинности Windows. Дополнительные сведения см. в статье [ограниченное делегирование Kerberos для единого входа в приложения с помощью прокси-сервера приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).

>[!NOTE]
>Не используйте это свойство для настройки SAML или единого входа на основе пароля. Если настраивается единый вход SAML, необходимо задать параметр [servicePrincipal](serviceprincipal.md).
Если вы настраиваете одиночный символ на основе пароля, его необходимо задать с помощью [креатепассвордсинглесигнонкредентиалс](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|кербероссервицепринЦипалнаме|String| Внутреннее имя субъекта-службы приложения сервера приложений. Это имя участника-службы должно быть в списке служб, к которому соединитель может предоставлять делегированные учетные данные. |
|кербероссигнонмаппингаттрибутетипе|String| Удостоверение делегированного имени входа для соединителя, которое будет использоваться от имени ваших пользователей. Более подробную информацию можно узнать [в статье работа с другими локальными и облачными удостоверениями ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities). Возможные значения: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.|

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

