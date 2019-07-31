---
title: Тип ресурса Едукатионсинчронизатионкустомизатион
description: 'Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 46cd20bbe016110a313d5b195a518ef81ca05afe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972455"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>Тип ресурса Едукатионсинчронизатионкустомизатион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. 

>**Примечание:** Свойство **синчронизатионстартдате** применяется только к объекту **студентенроллмент** .

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **Оптионалпропертиестосинк** | Коллекция String |  Коллекция имен свойств, которые необходимо синхронизировать. Если задано значение null, все свойства будут синхронизированы.       |
| **Синчронизатионстартдате** | DateTime |  Дата начала синхронизации. Это значение должно быть равно дате в будущем. Если задано значение null, то при завершении настройки профиля ресурс будет синхронизирован. **Примечание:** Это относится только к свойству **студентенроллмент** .      |
|**Иссинкдеферред** |Boolean | Указывает, откладывается ли синхронизация родительской сущности на более позднюю дату. |
| **Алловдисплайнамеупдате** | Boolean |  Указывает, может ли отображаемое имя ресурса быть перезаписано при синхронизации.         |


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
