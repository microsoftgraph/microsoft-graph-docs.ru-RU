---
title: Тип ресурса oAuth2Permission
description: Представляет область делегированного разрешения OAuth 2,0. Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта Application) при вызове приложения-ресурса. Свойство **appRoles** объекта servicePrincipal и сущности приложения является коллекцией **oAuth2Permission**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 16dfa93d13127d585cd5b56a56987bb22ab39d8f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009575"
---
# <a name="oauth2permission-resource-type"></a>Тип ресурса oAuth2Permission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет область делегированного разрешения OAuth 2,0. Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта [Application](application.md) ) при вызове приложения-ресурса. Свойство **appRoles** объекта [servicePrincipal](serviceprincipal.md) и сущности [приложения](application.md) является коллекцией **oAuth2Permission**.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Админконсентдескриптион|String|Текст справки по разрешениям, который отображается в качестве согласия администратора и взаимодействия с назначением приложений.|
|Админконсентдисплайнаме|String|Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений.|
|id|GUID|Уникальный идентификатор разрешения области в коллекции oauth2Permissions.|
|isEnabled|Boolean|При создании или обновлении разрешения для этого свойства должно быть задано **значение true** (значение по умолчанию). Чтобы удалить разрешение, необходимо сначала задать для этого свойства значение **false**.  В этот момент разрешение может быть удалено из последующего вызова.|
|type|String|Указывает, может ли пользователь иметь разрешение на доступ к области, а также о том, является ли оно разрешением, которое должно быть отослано администратором компании.  Возможные значения: "User" или "admin".|
|Усерконсентдескриптион|String|Текст справки по разрешениям, который отображается в диалоговом окне согласия конечного пользователя.|
|Усерконсентдисплайнаме|String|Отображаемое имя разрешения, которое отображается в диалоговом окне согласия конечного пользователя.|
|value|String|Значение утверждения области, которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
