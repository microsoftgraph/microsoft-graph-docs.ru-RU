---
title: Тип ресурса Профилекардпроперти
description: Используется для обозначения нового свойства для общего доступа, для людей или для пользователя, к которому будет применено пользовательское отображаемое имя или Аннотация. Администратор может определить строку отображаемого имени по умолчанию и набор альтернативных переводов для языков, которые они поддерживают в Организации.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 974e1e7af86133ef46c7d4360def1aef153ee3ec
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051118"
---
# <a name="profilecardproperty-resource-type"></a>Тип ресурса Профилекардпроперти

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет атрибут пользователя в карточке профиля Microsoft 365, который Организация будет использовать совместно с другими пользователями.

Атрибут может быть встроенным атрибутом Azure Active Directory (Azure AD), таким как `Alias` OR `UserPrincipalName` , или может быть настраиваемым атрибутом. Для настраиваемого атрибута администратор может определить `en-us` строку отображаемого имени по умолчанию и набор альтернативных переводов для языков, поддерживаемых в Организации.

Дополнительные сведения о добавлении свойств в карточку профиля для организации можно узнать в статье Настройка карточки профиля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [Список](../api/organizationsettings-list-profilecardproperties.md) | [профилекардпроперти](profilecardproperty.md) | Чтение свойств и связей объекта **профилекардпроперти** . |
| [Создание](../api/organizationsettings-post-profilecardproperties.md); | [профилекардпроперти](profilecardproperty.md) | Чтение свойств и связей объекта **профилекардпроперти** . |
| [Get](../api/profilecardproperty-get.md) | [профилекардпроперти](profilecardproperty.md) | Чтение свойств и связей объекта **профилекардпроперти** . |
| [Update](../api/profilecardproperty-update.md)               | [профилекардпроперти](profilecardproperty.md) | Обновление объекта **профилекардпроперти** .                               |
| [Delete](../api/profilecardproperty-delete.md)               | Нет                                          | Удаление объекта **профилекардпроперти** .                               |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                                        | Описание |
|:---------------------|:------------------------------------------------------------|:------------|
|Комментарии           |Коллекция [профилекарданнотатион](profilecardannotation.md) | Позволяет администратору задать настраиваемую метку отображения для свойства каталога и локализовать ее для пользователей в клиенте.|
|директорипропертинаме |String                                                       | Определяет ресурс **профилекардпроперти** в операциях [Get](../api/profilecardproperty-get.md), [Update](../api/profilecardproperty-update.md)или [Delete](../api/profilecardproperty-delete.md) . Позволяет администратору показывать скрытые свойства Azure Active Directory (Azure AD) на карте профиля Microsoft 365 в своем клиенте. Если этот параметр указан, поле Azure AD, указанное в этом поле, будет отображаться для всех пользователей в клиенте в области контактов карточки профиля. Допустимые значения для этого поля:,,,,,,,,,,,,,,,, `UserPrincipalName` `Fax` `StreetAddress` ,, `PostalCode` `StateOrProvince` `Alias` `CustomAttribute1` `CustomAttribute2` `CustomAttribute3` `CustomAttribute4` `CustomAttribute5` `CustomAttribute6` `CustomAttribute7` , `CustomAttribute8` , `CustomAttribute9` `CustomAttribute10` `CustomAttribute11` `CustomAttribute12` `CustomAttribute13` `CustomAttribute14` `CustomAttribute15` ,,,,,,,,,,,,,. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardProperty",
  "baseType": ""
}-->

```json
{
  "annotations": [
    {
      "displayName": "String",
      "localizations": [
        {
          "languageTag": "String",
          "displayName": "String"
        }
      ]
    }
  ],
  "directoryPropertyName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->