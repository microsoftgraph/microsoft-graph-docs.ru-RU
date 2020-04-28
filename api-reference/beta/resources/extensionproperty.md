---
title: Тип ресурса Екстенсионпроперти
description: Представляет расширение каталога
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3d6f6e89ca6e54e1c74e43c6201766aa199f454d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423799"
---
# <a name="extensionproperty-resource-type"></a>Тип ресурса Екстенсионпроперти

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расширение каталога, которое можно использовать для добавления настраиваемого свойства к объектам каталога без использования внешнего хранилища данных. Например, если в Организации есть бизнес-приложение, для которого требуется идентификатор Skype для каждого пользователя в каталоге, Microsoft Graph можно использовать для регистрации нового свойства с именем Скипеид в объекте пользователя каталога, а затем для записи значения в новое свойство для определенного пользователя.

Расширения можно добавлять в ресурсы " [пользователь](user.md)", " [Группа](group.md)", " [Организация](organization.md)", " [устройство](device.md)" и "ресурсы [приложения](application.md) ".

> [!IMPORTANT]
> Расширения схемы Azure AD, описанные в этой статье, доступны только в целях обеспечения обратной совместимости в Microsoft Graph.
> Он позволяет использовать Microsoft Graph, чтобы продолжить управление свойствами расширения, добавленными через Azure AD Graph или [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).
> Для новых настраиваемых расширений рекомендуется использовать расширения схемы Microsoft Graph для [добавления пользовательских данных в ресурсы](/graph/extensibility-overview).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список расширений](../api/application-list-extensionproperty.md) | Коллекция [extensionProperty](extensionProperty.md) | Список свойств расширения для объекта application. |
| [Создание расширения](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Создание свойства расширения для объекта application. |
| [Удаление расширения](../api/application-delete-extensionproperty.md) | Нет | Удаление свойства расширения объекта application. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appDisplayName|String| Отображаемое имя объекта приложения, для которого определено это свойство расширения. Только для чтения. |
|dataType|String| Задает тип данных значения, которое может содержать свойство Extension. Поддерживаются следующие значения: Значение null не допускается. <ul><li>`Binary`– 256 байт (максимум)</li><li>`Boolean`</li><li>`DateTime`-Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</li><li>`Integer`— значение 32 — бит.</li><li>`LargeInteger`— значение 64 — бит.</li><li>`String`– 256 символов максимум</li></ul>|
|иссинцедфромонпремисес|Boolean| Указывает, было ли это свойство расширения сикнед из локального каталога с помощью Azure AD Connect. Только для чтения. |
|name|Строка| Имя свойства расширения. Значение null не допускается. |
|таржетобжектс|Коллекция объектов string| Поддерживаются следующие значения: Значение null не допускается. <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

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
