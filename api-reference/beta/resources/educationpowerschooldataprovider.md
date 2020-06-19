---
title: ресурс Едукатионповерсчулдатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании PowerSchool в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9b85870f44eae936411e2aacf71781876858eee3
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790945"
---
# <a name="educationpowerschooldataprovider-resource"></a>ресурс Едукатионповерсчулдатапровидер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для настройки профиля синхронизации данных School при использовании [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) в качестве источника входных данных.

Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство                       | Тип                                     | Описание                                                                            |
| :----------------------------- | :--------------------------------------- | :------------------------------------------------------------------------------------- |
| алловтеачерсинмултиплесчулс | Boolean                                  | Указывает, содержит ли источник несколько идентификаторов для одного учащегося или преподавателя. |
| clientId                       | String                                   | Идентификатор клиента, используемый для подключения к PowerSchool.                                          |
| clientSecret                   | String                                   | Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool.          |
| коннектионурл                  | String                                   | URL-адрес подключения к экземпляру PowerSchool.                                        |
| счулсидс                     | Коллекция String                        | Список учебных заведений для синхронизации.                                                           |
| счулеар                     | String                                   | Год учебного заведения для синхронизации.                                                               |
| настроек                 | [едукатионсинчронизатионкустомизатионс] | Необязательная настройка, применяемая к профилю синхронизации.                   |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md
[едукатионсинчронизатионкустомизатионс]: educationsynchronizationcustomizations.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
  "connectionUrl": "String",
  "clientId": "String",
  "clientSecret": "String",
  "schoolsIds": ["String"],
  "schoolYear": "String",
  "allowTeachersInMultipleSchools": "Boolean",
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```
