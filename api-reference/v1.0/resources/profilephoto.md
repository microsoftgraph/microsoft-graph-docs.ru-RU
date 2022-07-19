---
title: Тип ресурса profilePhoto
description: Возвращает фотографию профиля пользователя, группы, группы или контакта Outlook, доступ к Exchange Online или Azure Active Directory (Azure AD).
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7a149d1321766298b6d55977ce58b2601c4c88cf
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856122"
---
# <a name="profilephoto-resource-type"></a>Тип ресурса profilePhoto

Пространство имен: microsoft.graph

Возвращает фотографию профиля пользователя, группы, группы или контакта Outlook, доступ к Exchange Online или Azure Active Directory (Azure AD). Данные являются двоичными и не кодируются в base-64.

Поддерживаемые размеры фотографий HD на Exchange Online: `48x48`, , , , `96x96`, `120x120`, `240x240`, `360x360`,`432x432`, и `648x648``504x504`. `64x64` В Azure AD фотографии могут быть любого измерения.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение объекта profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilephoto.md)|Чтение свойств и связей объекта фотографии профиля.|
|[Обновление profilePhoto](../api/profilephoto-update.md)|[profilePhoto](../resources/profilephoto.md)|Обновление свойств объекта фотографии профиля.|

> [!NOTE]
> Управление фотографиями пользователей с помощью microsoft API Graph в настоящее время не поддерживается в Azure AD B2C.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Только для чтения.|
|height|int32|Высота фотографии. Только для чтения.|
|width|int32|Ширина фотографии. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "String",
  "height": 240,
  "width": 240
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

