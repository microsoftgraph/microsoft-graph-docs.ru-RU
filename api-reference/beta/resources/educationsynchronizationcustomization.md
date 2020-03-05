---
title: Тип ресурса Едукатионсинчронизатионкустомизатион
description: 'Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 368117a5293f4ede59282fa1ced12d024976de52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500466"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>Тип ресурса Едукатионсинчронизатионкустомизатион

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. 

>**Примечание:** Свойство **синчронизатионстартдате** применяется только к объекту **студентенроллмент** .

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **оптионалпропертиестосинк** | Коллекция String |  Коллекция имен свойств, которые необходимо синхронизировать. Если задано значение null, все свойства будут синхронизированы.       |
| **синчронизатионстартдате** | DateTime |  Дата начала синхронизации. Это значение должно быть равно дате в будущем. Если задано значение null, то при завершении настройки профиля ресурс будет синхронизирован. **Примечание:** Это относится только к свойству **студентенроллмент** .      |
|**иссинкдеферред** |Логический | Указывает, откладывается ли синхронизация родительской сущности на более позднюю дату. |
| **алловдисплайнамеупдате** | Логический |  Указывает, может ли отображаемое имя ресурса быть перезаписано при синхронизации.         |


## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
