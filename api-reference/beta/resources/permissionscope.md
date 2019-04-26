---
title: Тип ресурса permissionScope
description: Представляет область делегированного разрешения OAuth 2,0. Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта Application) при вызове приложения-ресурса. Свойство **oauth2Permissions** объекта ServicePrincipal и сущности приложения является коллекцией **OAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 00629a6e123ef19290d3c1bd4797e4bab3ce95c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568182"
---
# <a name="permissionscope-resource-type"></a>Тип ресурса permissionScope

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет область делегированного разрешения OAuth 2,0. Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта [Application](application.md) ) при вызове приложения-ресурса. Свойство **oauth2Permissions** объекта [ServicePrincipal](serviceprincipal.md) и сущности [приложения](application.md) является коллекцией **OAuth2Permission**.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|Админконсентдескриптион|String| Текст справки по разРешениям, который отображается в качестве согласия администратора и взаимодействия с назначением приложений. |
|Админконсентдисплайнаме|String| Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений. |
|id|Guid| Уникальный идентификатор разрешения области в коллекции oauth2Permissions. |
|isEnabled|Boolean| При создании или обновлении разрешения для этого свойства должно быть задано **значение true** (значение по умолчанию). Чтобы удалить разрешение, необходимо сначала задать для этого свойства значение **false**. В этот момент разрешение может быть удалено из последующего вызова. |
|основания|String| Для внутреннего использования. |
|type|String| Указывает, может ли пользователь иметь разрешение на доступ к области, а также о том, является ли оно разрешением, которое должно быть отослано администратором компании. Возможные значения: *User* или *Admin*. |
|Усерконсентдескриптион|String| Текст справки по разРешениям, который отображается в диалоговом окне согласия конечного пользователя. |
|Усерконсентдисплайнаме|String| Отображаемое имя разрешения, которое отображается в диалоговом окне согласия конечного пользователя. |
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
  "suppressions": [
    "Error: /api-reference/beta/resources/permissionscope.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
