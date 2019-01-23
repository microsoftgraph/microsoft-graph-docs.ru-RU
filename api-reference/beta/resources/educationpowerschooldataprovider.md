---
title: educationPowerSchoolDataProvider ресурсов
description: Используется для настройки синхронизации профилей данных school при PowerSchool используется в качестве источника ввода.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4028170c2780cee426ec961a44b51e0362b0187f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406922"
---
# <a name="educationpowerschooldataprovider-resource"></a>educationPowerSchoolDataProvider ресурсов

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Используется для настройки синхронизации профилей данных school при [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) используется в качестве источника ввода.

На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **connectionUrl** | String | URL-адрес подключения к экземпляру PowerSchool. |
| **clientId** | String |  Идентификатор клиента, используемого для подключения к PowerSchool. |
| **clientSecret** | String |  Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool. |
| **schoolsIds** | Коллекция String |  Список школы для синхронизации. |
| **schoolYear** | String |  Учебный год для синхронизации. |
| **allowTeachersInMultipleSchools** | Логический |  Указывает, имеет ли источник несколько идентификаторов для одного студент и преподаватель. |
| **пользовательских настроек** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Дополнительные настройки применяется для синхронизации профилей.|

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
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
