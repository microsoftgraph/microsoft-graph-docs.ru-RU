---
title: Тип ресурса extensionProperty
description: Представляет расширение каталога
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5fb65da7151f8a5d8e3b1a852a8f90f92c130a12
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556138"
---
# <a name="extensionproperty-resource-type"></a>Тип ресурса extensionProperty

Пространство имен: microsoft.graph

Представляет расширение каталога, которое можно использовать для добавления настраиваемого свойства в объекты каталога без необходимости внешнего хранилища данных. Например, если в организации есть бизнес-приложение, требующее идентификатор Skype для каждого пользователя в каталоге, Microsoft Graph можно использовать для регистрации нового свойства **skypeId** в объекте пользователя каталога, а затем записать значение в новое свойство для определенного пользователя.

Расширения каталогов можно добавить в следующие объекты каталога:
+ [user](user.md)
+ [group](group.md)
+ [organization](organization.md)
+ [device](device.md)
+ [ресурсы приложения](application.md)

Только 100 значений расширения для всех типов  и всех приложений  можно записать в любой Azure AD ресурса.

Используйте этот ресурс и связанные методы для управления определениями расширений каталогов. Для управления данными расширения каталога в экземпляре расширенного ресурса используйте тот же запрос REST, который используется для управления экземпляром ресурса.

Дополнительные сведения о расширяемости Microsoft Graph см. в статье "Добавление настраиваемых [свойств в ресурсы с помощью расширений"](/graph/extensibility-overview).

Наследуется от [directoryObject](directoryobject.md).

> [!NOTE]
> Расширения, созданные с помощью Azure AD Graph (не рекомендуется) и пользовательские данные, синхронизированные из локальная служба Active Directory с помощью Azure AD Connect Sync, представлены как расширения каталогов в Microsoft Graph.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание объекта extensionProperties](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Создание свойства расширения для объекта application. |
| [Список объектов extensionProperties](../api/application-list-extensionproperty.md) | Коллекция [extensionProperty](extensionProperty.md) | Список свойств расширения для объекта application. |
| [Получение объекта extensionProperty](../api/extensionproperty-get.md) | Коллекция [extensionProperty](extensionProperty.md) | Список свойств расширения для объекта application. |
| [Удаление объекта extensionProperty](../api/extensionproperty-delete.md) | Нет | Удаление свойства расширения объекта application. Можно удалить только свойства, которые не синхронизируются из локальной службы Active Directory. |

> [!TIP]
> 1. Чтобы задать для свойства расширения значение экземпляра ресурса, указанного в **targetObjects**, используйте операцию обновления ресурса. Например, API [обновления пользователя](../api/user-update.md) для задания значения для пользователя.
> 2. Чтобы удалить свойство расширения и его значение из экземпляра ресурса, указанного в **targetObjects**, задайте для свойства расширения значение `null`.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appDisplayName|String| Отображаемое имя объекта приложения, для которого определено это свойство расширения. Только для чтения. |
|dataType|String| Указывает тип данных значения, которое может содержать свойство расширения. Поддерживаются следующие значения. Значение null не допускается. <ul><li>`Binary` — максимум 256 байт</li><li>`Boolean`</li><li>`DateTime` — должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</li><li>`Integer` — 32-разрядное значение.</li><li>`LargeInteger` — 64-разрядное значение.</li><li>`String` — не более 256 символов</li></ul>|
|deletedDateTime|DateTimeOffset|Дата и время удаления этого объекта. Всегда `null`, если объект не был удален. Наследуется от [directoryObject](directoryobject.md).|
|isSyncedFromOnPremises|Логический| Указывает, синхронизировано ли это свойство расширения из локальной службы Active Directory с помощью Azure AD Connect. Только для чтения. |
|name|String| Имя свойства расширения. Значение null не допускается. |
|targetObjects|Коллекция String| Поддерживаются следующие значения. Значение null не допускается. <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

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

## <a name="see-also"></a>См. также

+ [Добавление настраиваемых свойств в ресурсы с помощью расширений](/graph/extensibility-overview)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
