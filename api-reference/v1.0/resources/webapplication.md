---
title: Тип ресурса webApplication
description: Указывает параметры для веб-приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: cd524b0692775368c6426012d1829b5cf2119827
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135491"
---
# <a name="webapplication-resource-type"></a>Тип ресурса webApplication

Пространство имен: microsoft.graph

Указывает параметры для веб-приложения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| homePageUrl | String | Главная или начальная страница приложения. |
| implicitGrantSettings | [implicitGrantSettings](implicitgrantsettings.md)| Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0. |
| logoutUrl | String | Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML. |
| redirectUris | Коллекция String | Указывает URL-адреса, в которые отправляются маркеры пользователей для входов, или IS перенаправления, в которые отправляются коды авторизации OAuth 2.0 и маркеры доступа. |

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
  "redirectUris": ["String"]
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

