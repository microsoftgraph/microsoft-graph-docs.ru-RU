---
title: ресурс Едукатионповерсчулдатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании PowerSchool в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4fda7cc98c8041aad45a0ef8453affc9af34edc5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501229"
---
# <a name="educationpowerschooldataprovider-resource"></a>ресурс Едукатионповерсчулдатапровидер

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для настройки профиля синхронизации данных School при использовании [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) в качестве источника входных данных.

Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **коннектионурл** | String | URL-адрес подключения к экземпляру PowerSchool. |
| **clientId** | String |  Идентификатор клиента, используемый для подключения к PowerSchool. |
| **clientSecret** | String |  Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool. |
| **счулсидс** | Коллекция String |  Список учебных заведений для синхронизации. |
| **счулеар** | String |  Год учебного заведения для синхронизации. |
| **алловтеачерсинмултиплесчулс** | Логический |  Указывает, содержит ли источник несколько идентификаторов для одного учащегося или преподавателя. |
| **настроек** | [едукатионсинчронизатионкустомизатионс](educationsynchronizationcustomizations.md) | Необязательная настройка, применяемая к профилю синхронизации.|

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
