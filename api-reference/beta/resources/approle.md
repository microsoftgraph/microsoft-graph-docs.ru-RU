---
title: Тип ресурса Аппроле
description: Представляет роль приложения, которая может быть запрошена клиентским приложением, вызывающей другое приложение, или которая может использоваться для назначения приложения пользователям или группам в указанной роли приложения. Свойство **appRoles** объекта servicePrincipal и сущности приложения является коллекцией **аппроле**.
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535706"
---
# <a name="approle-resource-type"></a>Тип ресурса Аппроле

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет роль приложения, которая может быть запрошена клиентским приложением, вызывающей другое приложение, или которая может использоваться для назначения приложения пользователям или группам в указанной роли приложения. Свойство **appRoles** объекта [servicePrincipal](serviceprincipal.md) и сущности [приложения](application.md) является коллекцией **аппроле**.

> Важно! эта функция отключена в текущем выпуске.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Алловедмембертипес|Коллекция строк|Указывает, можно ли назначить это определение роли приложения пользователям и группам, задав для параметра значение "пользователь" или другие приложения (которые обращаются к этому приложению в сценариях службы демона), задав значение "Application" или как то, и другое.|
|description|String|Текст справки по разРешениям, который отображается при назначении и согласии приложения администрирования.|
|displayName|String|Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений.|
|id|Guid|Уникальный идентификатор роли в семействе **appRoles** .|
|isEnabled|Boolean|При создании или обновлении определения роли должно быть задано **значение true** (значение по умолчанию). Чтобы удалить роль, необходимо сначала задать значение **false**.  В этот момент эта роль может быть удалена в последующих вызовах.|
|value|String|Указывает значение утверждения ролей, которое должно ожидать приложение в маркерах проверки подлинности и доступа.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
