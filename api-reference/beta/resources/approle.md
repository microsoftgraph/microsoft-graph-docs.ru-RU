---
title: Тип ресурса роли приложения
description: Представляет роль приложения, которое может быть затребованы клиентское приложение вызов другого приложения или, который может использоваться для назначения приложения для пользователей или групп в указанном приложении роли. Свойство **appRoles** servicePrincipal сущности и сущности приложения — это коллекция **роли приложения**.
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525796"
---
# <a name="approle-resource-type"></a>Тип ресурса роли приложения

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет роль приложения, которое может быть затребованы клиентское приложение вызов другого приложения или, который может использоваться для назначения приложения для пользователей или групп в указанном приложении роли. Свойство **appRoles** [servicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **роли приложения**.

> Важно: Эта функция отключена в текущем выпуске.

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
|allowedMemberTypes|Коллекция String|Указывает ли определение роли в этом приложении можно назначить пользователям и группам, настройку «User» или другие приложения (которые обращаются к этого приложения в сценариях службы демон), задав для «Приложения» или оба.|
|description|String|Разрешение текст, который отображается в назначении приложения администрирования справки и соглашаетесь каждый раз.|
|displayName|String|Отображаемое имя для разрешения, которое отображается в admin согласия и приложение назначения приемы и способы работы.|
|id|Guid|Уникальный идентификатор роли в коллекцию **appRoles** .|
|isEnabled|Логический|При создании или обновлении определения роли, это должно быть присвоено **значение true** (по умолчанию). Чтобы удалить роль, это необходимо сначала задать значение **false**.  На этом этапе в последующих вызовов, с этой ролью может быть удален.|
|value|String|Задает значение утверждения роли, приложение должно привести в маркеры проверки подлинности и доступа.|

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
