---
title: Тип ресурса Едукатионсинчронизатионкустомизатион
description: 'Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 397f4d732bc25d086b2aeae6efc697d2048e6a03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334095"
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
|**Иссинкдеферред** |Логический | Указывает, откладывается ли синхронизация родительской сущности на более позднюю дату. |
| **Алловдисплайнамеупдате** | Логический |  Указывает, может ли отображаемое имя ресурса быть перезаписано при синхронизации.         |


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
