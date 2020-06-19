---
title: Тип ресурса Едукатионсинчронизатионкустомизатион
description: 'Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4aab80a23b72b599df7627f5734d04ad9aef0bbe
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790938"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>Тип ресурса Едукатионсинчронизатионкустомизатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям.

## <a name="properties"></a>Свойства

| Свойство                 | Тип              | Описание                                                                                                                                                                                                            |
| :----------------------- | :---------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| оптионалпропертиестосинк | Коллекция String | Коллекция имен свойств, которые необходимо синхронизировать. Если задано значение null, все свойства будут синхронизированы. **Не относится к регистрациям студентов или спискам преподавателей**                                                            |
| синчронизатионстартдате | DateTime          | Дата начала синхронизации. Это значение должно быть равно дате в будущем. Если задано значение null, то при завершении настройки профиля ресурс будет синхронизирован. **Применимо только к регистрациям для студентов** |
| иссинкдеферред           | Boolean           | Указывает, откладывается ли синхронизация родительской сущности на более позднюю дату.                                                                                                                                    |
| алловдисплайнамеупдате   | Boolean           | Указывает, может ли отображаемое имя ресурса быть перезаписано при синхронизации.                                                                                                                                     |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{
  "optionalPropertiesToSync": ["String"],
  "synchronizationStartDate": "DateTimeOffset",
  "isSyncDeferred": "Boolean",
  "allowDisplayNameUpdate": "Boolean"
}
```
