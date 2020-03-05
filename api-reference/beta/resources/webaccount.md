---
title: Тип ресурса "учетная запись"
description: Тип ресурса "учетная запись"
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ceb282dbcf0370e5eca2001b582660bdcaa1f1aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519451"
---
# <a name="webaccount-resource-type"></a>Тип ресурса "учетная запись"

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет веб-учетные записи, которые пользователь указал, используют или добавили в свой [профиль](profile.md)пользователя.

Этот тип ресурса наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

| Метод                                     | Возвращаемый тип                 | Описание                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [Получение учетной записи службы](../api/webaccount-get.md) | [Учетная запись учетной записи](webaccount.md) | Чтение свойств и связей объекта веб- **учетных записей** . |
| [Обновление учетной записи](../api/webaccount-update.md)      | [Учетная запись учетной записи](webaccount.md) | Обновление объекта **учетной записи** .                               |
| [Удаление учетной записи службы](../api/webaccount-delete.md)      | Нет                        | Удаление объекта **учетной записи** .                               |

## <a name="properties"></a>Свойства

| Свойство     | Тип                                      | Описание                                                                                    |
|:-------------|:------------------------------------------|:-----------------------------------------------------------------------------------------------|
|description   |String                                     | Содержит описание, предоставленное пользователем для учетной записи службы, на которую выполняется ссылка.|
|service       |[сервицеинформатион](serviceinformation.md)| Содержит основные сведения о связанной службе.                              |
|статусмессаже |String                                     | Содержит сообщение о состоянии от облачной службы, если оно предоставлено или синхронизировано.                  |
|userId        |String                                     | Имя пользователя, отображаемое для учетной записи Account.                                    |
|webUrl        |String                                     | Содержит ссылку на профиль пользователя в облачной службе, если она существует.                       |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": ""
}-->

```json
{
  "description": "String",
  "service": {"@odata.type": "microsoft.graph.serviceInformation"},
  "statusMessage": "String",
  "userId": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webAccount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
