---
title: Тип ресурса profileCardProperty
description: Используется для назначить новое свойство, которое будет отображаться в общем, пользовательском или пользовательском отображаемом имени или аннотации. Администратор может определить строку отображаемого имени по умолчанию и набор альтернативных переводов для поддерживаемого в организации языка.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 33d2b1111580ba2302848ab1dbce3f773055a0b4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153566"
---
# <a name="profilecardproperty-resource-type"></a>Тип ресурса profileCardProperty

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет атрибут пользователя в карточке профиля Microsoft 365, чтобы организация представляла общий интерфейс пользователей.

Атрибут может быть встроенным атрибутом Azure Active Directory (Azure AD), например или настраиваемый `Alias` `UserPrincipalName` атрибут. Для настраиваемого атрибута администратор может определить строку отображаемого имени по умолчанию и набор альтернативных переводов для поддерживаемого в `en-us` организации языка.

Дополнительные сведения о добавлении свойств в карточку профиля для организации см. в [подстройке карточки профиля.](/graph/add-properties-profilecard)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [Список](../api/organizationsettings-list-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Получите коллекцию ресурсов **profileCardProperty** организации. |
| [Создание](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Создайте ресурс **profileCardProperty** для организации. |
| [Получение](../api/profilecardproperty-get.md) | [profileCardProperty](profilecardproperty.md) | Прочитайте свойства и связи ресурса **profileCardProperty,** который содержит настройки карточки профиля, которые существуют в организации Microsoft 365 для заданного поля. |
| [Обновление](../api/profilecardproperty-update.md)               | [profileCardProperty](profilecardproperty.md) | Обновление объекта **profileCardProperty.**                               |
| [удаление](../api/profilecardproperty-delete.md);               | Нет                                          | Удаление объекта **profileCardProperty.**                               |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                                        | Описание |
|:---------------------|:------------------------------------------------------------|:------------|
|аннотации           |[Коллекция profileCardAnnotation](profilecardannotation.md) | Позволяет администратору установить настраиваемую метку отображения для свойства каталога и локализовать ее для пользователей в клиенте.|
|directoryPropertyName |String                                                       | Определяет ресурс **profileCardProperty** в операциях [Get,](../api/profilecardproperty-get.md) [Update](../api/profilecardproperty-update.md)и [Delete.](../api/profilecardproperty-delete.md) Позволяет администратору использовать скрытые свойства Azure Active Directory (Azure AD) в карточке профиля Microsoft 365 в клиенте. Если заметен, поле Azure AD, на который ссылается это поле, будет видно всем пользователям в клиенте в области контактов карточки профиля. Допустимые значения для этого поля: , , , , `UserPrincipalName` , , `Fax` `StreetAddress` `PostalCode` `StateOrProvince` `Alias` `CustomAttribute1` , `CustomAttribute2` `CustomAttribute3` `CustomAttribute4` `CustomAttribute5` `CustomAttribute6` `CustomAttribute7` `CustomAttribute8` `CustomAttribute9` `CustomAttribute10` `CustomAttribute11` `CustomAttribute12` `CustomAttribute13` `CustomAttribute14` . `CustomAttribute15` |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardProperty"
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

