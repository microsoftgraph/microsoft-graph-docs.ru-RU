---
title: тип ресурса extensionProperty
description: Представляет расширение каталога
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2f26495298d38b80544108f2d0c2967c5d4a9a7f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335999"
---
# <a name="extensionproperty-resource-type"></a>тип ресурса extensionProperty

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расширение каталога, которое можно использовать для добавления настраиваемой свойства в объекты каталогов без необходимости хранения внешних данных. Например, если в организации есть приложение бизнес-интерфейса, для которого для каждого пользователя каталога требуется Skype ID, Microsoft Graph может быть использована для регистрации нового свойства с именем skypeId в объекте Пользователя каталога, а затем записываю значение для нового свойства для определенного пользователя.

Расширения могут быть добавлены к [ресурсам пользователей](user.md), [групп](group.md), [организаций](organization.md), [устройств](device.md), [приложений](application.md) . Только 100 значений расширения для всех типов  и всех приложений  можно написать на любой ресурс Azure AD.

Наследуется от [directoryObject](directoryobject.md).

> [!IMPORTANT]
> Описанные здесь расширения схем Azure AD доступны в Microsoft Graph только по причинам обратной совместимости.
> Это позволяет использовать microsoft Graph для управления свойствами расширения, добавленными через Azure AD Graph (амортизации) или [Azure AD Подключение](/azure/active-directory/hybrid/whatis-azure-ad-connect).
> Для новых пользовательских расширений рекомендуется использовать Graph microsoft Graph для [добавления пользовательских данных в ресурсы](/graph/extensibility-overview).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание свойств расширения](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Создание свойства расширения для объекта application. |
| [Свойства расширения списка](../api/application-list-extensionproperty.md) | Коллекция [extensionProperty](extensionProperty.md) | Список свойств расширения для объекта application. |
| [Получить extensionProperty](../api/extensionproperty-get.md) | Коллекция [extensionProperty](extensionProperty.md) | Список свойств расширения для объекта application. |
| [Удаление extensionProperty](../api/extensionproperty-delete.md) | Нет | Удаление свойства расширения объекта application. |

> [!TIP]
> 1. Чтобы установить значение свойства расширения экземпляру ресурса, указанному в **targetObjects**, используйте операцию Update ресурса. Например, API [для обновления](../api/user-update.md) пользователя, чтобы установить значение для пользователя.
> 2. Чтобы удалить свойство расширения и его значение из экземпляра ресурса, указанного в **targetObjects**, установите значение свойства расширения `null`.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appDisplayName|String| Отображение имени объекта приложения, на котором определено это свойство расширения. Только для чтения. |
|dataType|String| Указывает тип данных значения, который может удерживать свойство расширения. Поддерживаются следующие значения. Значение null не допускается. <ul><li>`Binary` - максимум 256 bytes</li><li>`Boolean`</li><li>`DateTime` - Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</li><li>`Integer` - 32-битное значение.</li><li>`LargeInteger` - 64-битное значение.</li><li>`String` - максимум 256 символов</li></ul>|
|deletedDateTime|DateTimeOffset|Дата и время удаления этого объекта. Всегда `null` , когда объект не был удален. Наследуется от [directoryObject](directoryobject.md).|
|isSyncedFromOnPremises|Boolean| Указывает, синхронизировано ли это свойство расширения из локального активного каталога с помощью Azure AD Подключение. Только для чтения. |
|name|String| Имя свойства расширения. Значение null не допускается. |
|targetObjects|Коллекция объектов string| Поддерживаются следующие значения. Значение null не допускается. <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.extensionProperty",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extensionProperty",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "name": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": "Boolean",
  "targetObjects": [
    "String"
  ]
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
