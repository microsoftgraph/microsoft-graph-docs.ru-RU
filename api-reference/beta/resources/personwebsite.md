---
title: Тип ресурса personWebsite
description: Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c26bda366fe03893e138551cb3ae3e8ab1efd8c8
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900480"
---
# <a name="personwebsite-resource-type"></a>Тип ресурса personWebsite

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.

Наследуется [от itemFacet](itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление веб-сайтов](../api/profile-list-websites.md)|[Коллекция personWebsite](../resources/personwebsite.md)|Получите ресурсы personWebsite из свойства навигации веб-сайтов.|
|[Создание personWebsite](../api/profile-post-websites.md)|[personWebsite](../resources/personwebsite.md)|Создайте объект personWebsite.|
|[Получение personWebsite](../api/personwebsite-get.md)|[personWebsite](../resources/personwebsite.md)|Чтение свойств и связей объекта [personWebsite](../resources/personwebsite.md) .|
|[Обновление personWebsite](../api/personwebsite-update.md)|[personWebsite](../resources/personwebsite.md)|Обновление свойств объекта [personWebsite](../resources/personwebsite.md) .|
|[Удаление personWebsite](../api/personwebsite-delete.md)|Нет|Удаляет объект [personWebsite](../resources/personwebsite.md) .|

## <a name="properties"></a>Свойства

| Свойство     | Тип              | Описание                                                                                   |
|:-------------|:------------------|:----------------------------------------------------------------------------------------------|
|categories    |Коллекция String  | Содержит категории, связанные пользователем с веб-сайтом (например, личные, рецепты).  |
|description   |Строка             | Содержит описание веб-сайта.                                                        |
|displayName   |Строка             | Содержит понятное имя веб-сайта.                                                     |
|webUrl        |String             | Содержит ссылку на сам веб-сайт.                                                        |

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personWebsite",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "categories": [
    "String"
  ],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```


