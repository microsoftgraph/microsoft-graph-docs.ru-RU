---
title: Тип ресурса extensionProperty
description: Представляет расширение каталога
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 0b3c462353997dafc01c2d9d52be70f15af3447e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154749"
---
# <a name="extensionproperty-resource-type"></a>Тип ресурса extensionProperty

Пространство имен: microsoft.graph

Представляет расширение каталога, которое можно использовать для добавления настраиваемой свойства в объекты каталогов без необходимости хранения внешних данных. Например, если в организации есть бизнес-приложение, для которого требуется ИД Skype для каждого пользователя в каталоге, Microsoft Graph можно использовать для регистрации нового свойства skypeId в объекте User каталога и записи значения в новое свойство для определенного пользователя.

Расширения можно добавлять в ресурсы [пользователей,](user.md) [групп,](group.md) [организаций,](organization.md) [устройств,](device.md) [приложений.](application.md)

> [!IMPORTANT]
> Расширения схемы Azure AD, описанные здесь, доступны в Microsoft Graph только из соображений обратной совместимости.
> Это позволяет использовать Microsoft Graph для управления свойствами расширений, добавленными через Azure AD Graph или [Azure AD Connect.](/azure/active-directory/hybrid/whatis-azure-ad-connect)
> Для новых пользовательских расширений рекомендуется использовать расширения схемы Microsoft Graph для добавления пользовательских [данных в ресурсы.](/graph/extensibility-overview)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание расширения](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Создание свойства расширения для объекта application. |
| [Список расширений](../api/application-list-extensionproperty.md) | Коллекция [extensionProperty](extensionProperty.md) | Список свойств расширения для объекта application. |
| [Удаление расширения](../api/application-delete-extensionproperty.md) | Нет | Удаление свойства расширения объекта application. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appDisplayName|String| Отображает имя объекта приложения, в котором определено это свойство расширения. Только для чтения. |
|dataType|String| Указывает тип данных значения, который может быть в свойстве расширения. Поддерживаются следующие значения. Значение null не допускается. <ul><li>`Binary` - 256 bytes maximum</li><li>`Boolean`</li><li>`DateTime` - Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</li><li>`Integer` - 32-битное значение.</li><li>`LargeInteger` - 64-битное значение.</li><li>`String` — не более 256 символов</li></ul>|
|isSyncedFromOnPremises|Логическое| Указывает, было ли это свойство расширения sycned из каталога onpremises с помощью Azure AD Connect. Только для чтения. |
|name|String| Имя свойства расширения. Значение null не допускается. |
|targetObjects|Коллекция String| Поддерживаются следующие значения. Значение null не допускается. <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionProperty",
  "keyProperty": "id"
}-->

```json
{
  "appDisplayName": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": true,
  "name": "String",
  "targetObjects": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
