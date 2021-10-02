---
title: Тип ресурса webApplication
description: Указывает параметры для веб-приложения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f4f6ec9d65dd6d30b54b030651178484392fba06
ms.sourcegitcommit: 0ec845f93eaa140ad833ba163c76c5308197a92f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2021
ms.locfileid: "60068547"
---
# <a name="webapplication-resource-type"></a>Тип ресурса webApplication

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает параметры для веб-приложения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| homePageUrl | String | Главная или начальная страница приложения. |
| implicitGrantSettings | [implicitGrantSettings](implicitgrantsettings.md)| Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0. |
| logoutUrl | String | Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML. |
| redirectUris | Коллекция String | Указывает URL-адреса, куда отправляются маркеры пользователей для регистрации, или URL-адреса перенаправления, куда отправляются коды авторизации OAuth 2.0 и маркеры доступа. |
|redirectUriSettings| [коллекция redirectUriSettings](redirecturisettings.md) | Указывает индекс URL-адресов, куда отправляются маркеры пользователей для регистрации. Это допустимо только для приложений с помощью SAML.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webApplication"
}-->

```json
{
  "homePageUrl": "String",
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
  "redirectUris": ["String"],
  "redirectUriSettings": [
    {
      "@odata.type": "microsoft.graph.redirectUriSettings"
    }
  ],
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


