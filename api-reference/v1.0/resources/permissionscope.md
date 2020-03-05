---
title: Тип ресурса permissionScope
description: Представляет область делегированного разрешения OAuth 2,0.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bdc022f82f2e0dc7a1277d2674f215b58d521679
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447215"
---
# <a name="permissionscope-resource-type"></a>Тип ресурса permissionScope

Пространство имен: Microsoft. Graph

Представляет область делегированного разрешения OAuth 2,0. Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта [Application](application.md) ) при вызове приложения-ресурса. Свойство **oauth2Permissions** <!-- of the [servicePrincipal](serviceprincipal.md) entity and --> объекта [Application](application.md) — коллекция **permissionScope**.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|админконсентдескриптион|String| Текст справки по разрешениям, который отображается в качестве согласия администратора и взаимодействия с назначением приложений. |
|админконсентдисплайнаме|String| Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений. |
|id|GUID| Уникальный идентификатор разрешения области в коллекции oauth2Permissions. |
|isEnabled|Boolean| При создании или обновлении разрешения для этого свойства должно быть задано **значение true** (значение по умолчанию). Чтобы удалить разрешение, необходимо сначала задать для этого свойства значение **false**. В этот момент разрешение может быть удалено из последующего вызова. |
|основания|String| Для внутреннего использования. |
|type|String| Указывает, может ли пользователь иметь разрешение на доступ к области, а также о том, является ли оно разрешением, которое должно быть отослано администратором компании. Возможные значения: *User* или *Admin*. |
|усерконсентдескриптион|String| Текст справки по разрешениям, который отображается в диалоговом окне согласия конечного пользователя. |
|усерконсентдисплайнаме|String| Отображаемое имя разрешения, которое отображается в диалоговом окне согласия конечного пользователя. |
|value|String| Значение утверждения области, которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
