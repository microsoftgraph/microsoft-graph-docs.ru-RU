---
title: ресурс Едукатионповерсчулдатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании PowerSchool в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6a036435cb7cc1a4ef70960b09feb600fe7f39f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972599"
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
| **Счулсидс** | Коллекция строк |  Список учебных заведений для синхронизации. |
| **Счулеар** | String |  Год учебного заведения для синхронизации. |
| **Алловтеачерсинмултиплесчулс** | Boolean |  Указывает, содержит ли источник несколько идентификаторов для одного учащегося или преподавателя. |
| **настроек** | [Едукатионсинчронизатионкустомизатионс](educationsynchronizationcustomizations.md) | Необязательная настройка, применяемая к профилю синхронизации.|

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
