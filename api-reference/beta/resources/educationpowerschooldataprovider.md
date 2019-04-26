---
title: ресурс Едукатионповерсчулдатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании PowerSchool в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cee763995dd5a75b64d94e5f170d6fea992c20b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340579"
---
# <a name="educationpowerschooldataprovider-resource"></a>ресурс Едукатионповерсчулдатапровидер

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для настройки профиля синхронизации данных School при использовании [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) в качестве источника входных данных.

Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **Коннектионурл** | String | URL-адрес подключения к экземпляру PowerSchool. |
| **clientId** | String |  Идентификатор клиента, используемый для подключения к PowerSchool. |
| **clientSecret** | String |  Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool. |
| **Счулсидс** | Коллекция String |  Список учебных заведений для синхронизации. |
| **Счулеар** | String |  Год учебного заведения для синхронизации. |
| **Алловтеачерсинмултиплесчулс** | Логический |  Указывает, содержит ли источник несколько идентификаторов для одного учащегося или преподавателя. |
| **настроек** | [Едукатионсинчронизатионкустомизатионс](educationsynchronizationcustomizations.md) | НеОбязательная Настройка, применяемая к профилю синхронизации.|

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
  "customizations": {"@odata.type": "microsoft.graph.educationSynchronizationCustomizations"}
}
```
