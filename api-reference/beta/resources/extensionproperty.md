---
title: Тип ресурса Екстенсионпроперти
description: Представляет расширение каталога
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f42ac98e0e13d8482f025e8b86886b1658d80d1d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939069"
---
# <a name="extensionproperty-resource-type"></a>Тип ресурса Екстенсионпроперти

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расширение каталога, которое можно использовать для добавления настраиваемого свойства к объектам каталога без использования внешнего хранилища данных. Например, если в Организации есть бизнес-приложение, для которого требуется идентификатор Skype для каждого пользователя в каталоге, Microsoft Graph можно использовать для регистрации нового свойства с именем Скипеид в объекте пользователя каталога, а затем для записи значения в новое свойство. для определенного пользователя.

Расширения можно добавлять в ресурсы " [пользователь](user.md)", " [Группа](group.md)", " [Организация](organization.md)", " [устройство](device.md)" и "ресурсы [приложения](application.md) ".

> [!IMPORTANT]
> Расширения схемы Azure AD, описанные в этой статье, доступны только в целях обеспечения обратной совместимости в Microsoft Graph.
> Он позволяет использовать Microsoft Graph, чтобы продолжить управление свойствами расширения, добавленными через Azure AD Graph или [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).
> Для новых настраиваемых расширений рекомендуется использовать расширения схемы Microsoft Graph для [добавления пользовательских данных в ресурсы](/graph/extensibility-overview).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Расширения списка](../api/application-list-extensionproperty.md) | Коллекция [екстенсионпроперти](extensionProperty.md) | Список свойств расширения для объекта Application. |
| [Создание расширения](../api/application-post-extensionproperty.md) | [екстенсионпроперти](extensionProperty.md) | Создание свойства расширения для объекта Application. |
| [Удаление расширения](../api/application-delete-extensionproperty.md) | Нет. | Удаление свойства расширения из объекта Application. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appDisplayName|String| Отображаемое имя объекта приложения, для которого определено это свойство расширения. Только для чтения. |
|dataType|String| Задает тип данных значения, которое может содержать свойство Extension. Поддерживаются следующие значения: Значение null не допускается. <ul><li>`Binary`– 256 байт (максимум)</li><li>`Boolean`</li><li>`DateTime`-Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</li><li>`Integer`— значение 32 — бит.</li><li>`LargeInteger`— значение 64 — бит.</li><li>`String`– 256 символов максимум</li></ul>|
|иссинцедфромонпремисес|Логический| Указывает, было ли это свойство расширения сикнед из локального каталога с помощью Azure AD Connect. Только для чтения. |
|name|Строка| Имя свойства расширения. Значение null не допускается. |
|таржетобжектс|Коллекция строк| Поддерживаются следующие значения: Значение null не допускается. <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionProperty",
  "baseType": "",
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
