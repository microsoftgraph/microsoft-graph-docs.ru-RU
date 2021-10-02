---
title: тип ресурса redirectUriSettings
description: Указывает индекс для redirectUri
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 756b1e1caf92e505e62380e0ca56cc2a6f549aef
ms.sourcegitcommit: 0ec845f93eaa140ad833ba163c76c5308197a92f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2021
ms.locfileid: "60069351"
---
# <a name="redirecturisettings-resource-type"></a>тип ресурса redirectUriSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает индекс URL-адресов, куда отправляются маркеры пользователей для регистрации. Это допустимо только для приложений с помощью SAML.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| uri | String | Указывает URI, в который отправляются маркеры. |
|index|Int32|Определяет определенный URI в коллекции redirectURIs в потоках SSO SAML. Значение по умолчанию — `null`. Индекс уникален во всех перенаправлениях для приложения.|


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.redirectUriSettings"
}-->

``` json
{
  "@odata.type": "#microsoft.graph.redirectUriSettings",
  "uri": "String",
  "index": "Integer"
}
```
