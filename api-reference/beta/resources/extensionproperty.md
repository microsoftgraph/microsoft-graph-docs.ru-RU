---
title: тип ресурса extensionProperty
description: Представляет расширение каталога
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 33603d0d16cc44fd2f07177da4c6c6bb4208b082
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941787"
---
# <a name="extensionproperty-resource-type"></a>тип ресурса extensionProperty

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расширение каталога, которое можно использовать для добавления настраиваемой свойства в объекты каталогов без необходимости хранения внешних данных. Например, если в организации есть приложение для бизнеса (LOB), для которого для каждого пользователя каталога требуется skype ID, Microsoft Graph можно использовать для регистрации нового свойства skypeId в объекте Пользователя каталога, а затем записываю значение для нового свойства для определенного пользователя.

Расширения могут быть добавлены к [ресурсам пользователей,](user.md) [групп,](group.md) [организаций,](organization.md) [устройств,](device.md) [приложений.](application.md) Только 100 значений  расширения для  всех типов и всех приложений можно написать на любой ресурс Azure AD.

> [!IMPORTANT]
> Описанные здесь расширения схем Azure AD доступны в Microsoft Graph только по причинам обратной совместимости.
> Это позволяет использовать Microsoft Graph для управления свойствами расширения, добавленными через Azure AD Graph или [Azure AD Connect.](/azure/active-directory/hybrid/whatis-azure-ad-connect)
> Для новых пользовательских расширений рекомендуется использовать расширения схемы Microsoft Graph для [добавления пользовательских данных в ресурсы.](/graph/extensibility-overview)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список расширений](../api/application-list-extensionproperty.md) | Коллекция [extensionProperty](extensionProperty.md) | Список свойств расширения для объекта application. |
| [Создание расширения](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Создание свойства расширения для объекта application. |
| [Удаление расширения](../api/application-delete-extensionproperty.md) | Нет | Удаление свойства расширения объекта application. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appDisplayName|String| Отображение имени объекта приложения, на котором определено это свойство расширения. Только для чтения. |
|dataType|String| Указывает тип данных значения, который может удерживать свойство расширения. Поддерживаются следующие значения. Значение null не допускается. <ul><li>`Binary` - максимум 256 bytes</li><li>`Boolean`</li><li>`DateTime` - Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</li><li>`Integer` - 32-битное значение.</li><li>`LargeInteger` - 64-битное значение.</li><li>`String` - максимум 256 символов</li></ul>|
|isSyncedFromOnPremises|Boolean| Указывает, было ли это свойство расширения sycned из каталога onpremises с помощью Azure AD Connect. Только для чтения. |
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
