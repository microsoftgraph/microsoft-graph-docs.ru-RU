---
title: тип ресурса extensionProperty
description: Представляет расширение каталога
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d1fd966e3efb4a8537cbad56cca2a3e0fb4cbb50
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694367"
---
# <a name="extensionproperty-resource-type"></a>тип ресурса extensionProperty

Пространство имен: microsoft.graph

Представляет расширение каталога, которое можно использовать для добавления настраиваемой свойства в объекты каталогов без необходимости хранения внешних данных. Например, если в организации есть приложение для бизнеса (LOB), для которого для каждого пользователя каталога требуется Skype ID, Microsoft Graph может быть использована для регистрации нового свойства skypeId в объекте Пользователя каталога, а затем записываю значение для нового свойства для определенного пользователя.

Расширения могут быть добавлены к [ресурсам пользователей,](user.md) [групп,](group.md) [организаций,](organization.md) [устройств,](device.md) [приложений.](application.md) Только 100 значений  расширения для  всех типов и всех приложений можно написать на любой ресурс Azure AD.

> [!IMPORTANT]
> Описанные здесь расширения схем Azure AD доступны в Microsoft Graph только по причинам обратной совместимости.
> Это позволяет использовать microsoft Graph для управления свойствами расширения, добавленными через Azure AD Graph (обесценилось) или [Azure AD Подключение](/azure/active-directory/hybrid/whatis-azure-ad-connect).
> Для новых пользовательских расширений рекомендуется использовать расширения схемы microsoft Graph для добавления пользовательских [данных в ресурсы.](/graph/extensibility-overview)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание расширения](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Создание свойства расширения для объекта application. |
| [Список расширений](../api/application-list-extensionproperty.md) | Коллекция [extensionProperty](extensionProperty.md) | Список свойств расширения для объекта application. |
| [Удаление расширения](../api/application-delete-extensionproperty.md) | Нет | Удаление свойства расширения объекта application. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appDisplayName|String| Отображение имени объекта приложения, на котором определено это свойство расширения. Только для чтения. |
|dataType|String| Указывает тип данных значения, который может удерживать свойство расширения. Поддерживаются следующие значения. Значение null не допускается. <ul><li>`Binary` - максимум 256 bytes</li><li>`Boolean`</li><li>`DateTime` - Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</li><li>`Integer` - 32-битное значение.</li><li>`LargeInteger` - 64-битное значение.</li><li>`String` - максимум 256 символов</li></ul>|
|isSyncedFromOnPremises|Логический| Указывает, было ли это свойство расширения sycned из каталога onpremises с помощью Azure AD Подключение. Только для чтения. |
|name|String| Имя свойства расширения. Значение null не допускается. |
|targetObjects|Коллекция строк| Поддерживаются следующие значения. Значение null не допускается. <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

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
