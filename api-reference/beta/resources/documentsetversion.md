---
title: Тип ресурса documentSetVersion
description: Представляет версию элемента набора документов в списке.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: c86cad9d0e5fe251c3d67145f56c9de2578b22c3
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061226"
---
# <a name="documentsetversion-resource-type"></a>Тип ресурса documentSetVersion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет версию элемента набора документов в списке.

Наследуется [от listItemVersion](../resources/listitemversion.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление documentSetVersions](../api/listitem-list-documentsetversions.md)|[Коллекция documentSetVersion](../resources/documentsetversion.md)|Получение ресурсов [documentSetVersion](../resources/documentsetversion.md) из свойства навигации **documentSetVersions** .|
|[Создание documentSetVersion](../api/listitem-post-documentsetversions.md)|[documentSetVersion](../resources/documentsetversion.md)|Создайте объект [documentSetVersion](../resources/documentsetversion.md) .|
|[Получение documentSetVersion](../api/documentsetversion-get.md)|[documentSetVersion](../resources/documentsetversion.md)|Чтение свойств и связей объекта [documentSetVersion](../resources/documentsetversion.md) .|
|[Удаление documentSetVersion](../api/documentsetversion-delete.md)|Нет|Удаление объекта [documentSetVersion](../resources/documentsetversion.md) .|
|[Восстановить](../api/documentsetversion-restore.md)|[documentSetVersion](../resources/documentsetversion.md)|[Восстановите documentSetVersion](../resources/documentsetversion.md).|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| comment | string | Комментарий к записанной версии.|
| createdBy   | [identitySet](../resources/identityset.md) | Пользователь, записавший версию.|
| createdDateTime     | dateTime | Дата и время создания этой версии.|
| id                  | string                                               | Идентификатор версии. Только для чтения. Наследуется [от listItemVersion](../resources/listitemversion.md).|
| items     | [Коллекция documentSetVersionItem](../resources/documentsetversionitem.md) | Элементы в наборе документов, которые записываются как часть этой версии.|
| lastModifiedBy       | [identitySet](../resources/identityset.md)           | Удостоверение пользователя, который последним изменил версию. Только для чтения. Наследуется [от listItemVersion](../resources/listitemversion.md).|
| lastModifiedDateTime | [Datetimeoffset](../resources/timestamp.md)          | Дата и время последнего изменения версии. Только для чтения. Наследуется [от listItemVersion](../resources/listitemversion.md).     |
| Опубликовано            | [publicationFacet](../resources/publicationfacet.md). | Указывает состояние публикации конкретной версии. Только для чтения. Наследуется [от listItemVersion](../resources/listitemversion.md).| 
| shouldCaptureMinorVersion | boolean  | Если `true`также записываются дополнительные версии элементов; в противном случае будут записаны только основные версии. Значение по умолчанию — `false`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
| fields        | [fieldValueSet](../resources/fieldvalueset.md) | Коллекция полей и значений для этой версии элемента списка. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.documentSetVersion",
  "baseType": "microsoft.graph.listItemVersion",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.documentSetVersion",
  "comment": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "items": [
    {
      "@odata.type": "microsoft.graph.documentSetVersionItem"
    }
  ],
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "shouldCaptureMinorVersion": "Boolean"
}
```

