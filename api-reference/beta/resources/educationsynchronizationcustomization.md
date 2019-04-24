---
title: Тип ресурса Едукатионсинчронизатионкустомизатион
description: 'Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507054"
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
