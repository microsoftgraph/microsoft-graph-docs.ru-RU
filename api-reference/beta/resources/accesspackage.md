---
title: Тип ресурса Акцесспаккаже
description: Пакет Access определяет коллекции ролей ресурсов и политики, которые могут получить доступ к этим ресурсам для одного или нескольких пользователей.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d49ddfcc0db9b55701f0b84a223efcec85aa8dfe
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228067"
---
# <a name="accesspackage-resource-type"></a>Тип ресурса Акцесспаккаже

Пространство имен: microsoft.graph



В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)пакет Access определяет коллекции ролей ресурсов и политики того, как один или несколько пользователей могут получить доступ к этим ресурсам.  
Каждый пакет Access ссылается на один каталог пакетов доступа и содержит ссылки на ресурсы из этого каталога с помощью областей ролей, определяющих доступ к пакету.  Пакет Access также содержит ссылки на политики назначения пакетов Access, каждый из которых определяет, кто может запрашивать или назначать назначение пакета Access.

Чтобы назначить пользователя пакету Access, [Создайте акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md) , ссылающийся на политику назначения пакетов доступа и пакетов Access.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Акцесспаккажес](../api/accesspackage-list.md) | Коллекция [акцесспаккаже](accesspackage.md) | Получение списка объектов **акцесспаккаже** . |
| [Создание Акцесспаккаже](../api/accesspackage-post.md) | [акцесспаккаже](accesspackage.md) | Создание нового объекта **акцесспаккаже** . |
| [Получение Акцесспаккаже](../api/accesspackage-get.md) | [акцесспаккаже](accesspackage.md) | Чтение свойств и связей объекта **акцесспаккаже** . |
| [Удаление Акцесспаккаже](../api/accesspackage-delete.md) |Нет | Удаление **акцесспаккаже**. |
| [Список Акцесспаккажересаурцеролескопес](../api/accesspackage-list-accesspackageresourcerolescopes.md) | Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md) | Получение списка объектов **акцесспаккажересаурцеролескопе** для этого пакета Access. |
| [Создание Акцесспаккажересаурцеролескопе](../api/accesspackage-post-accesspackageresourcerolescopes.md) |Нет | Создайте новый объект **акцесспаккажересаурцеролескопе** для этого пакета Access. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|каталогид|String|Идентификатор каталога пакетов доступа, на который ссылается этот пакет Access. Только для чтения.|
|createdBy|String|Имя участника-пользователя или идентификатор субъекта, создавшего этот ресурс. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|description|String|Описание пакета Access.|
|displayName|Строка|Отображаемое имя пакета Access.|
|id|String| Только для чтения.|
|Скрытый|Логический|Указывает, является ли пакет доступа скрытым от запрашивающего.|
|исролескопесвисибле|Логический|Указывает, видимы ли области ролей.|
|модифиедби|String|Имя участника-пользователя, который последним изменил этот ресурс. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|акцесспаккажеассигнментполиЦиес|Коллекция [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md)| Только для чтения. Допускается значение null.|
|акцесспаккажекаталог|[акцесспаккажекаталог](accesspackagecatalog.md)| Только для чтения. Допускается значение null.|
|акцесспаккажересаурцеролескопес|Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md)| Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
