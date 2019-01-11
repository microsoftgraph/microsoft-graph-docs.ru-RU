---
title: educationPowerSchoolDataProvider ресурсов
description: Используется для настройки синхронизации профилей данных school при PowerSchool используется в качестве источника ввода.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 48a23a2e2a50e2e235b5722466c67094275236a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868784"
---
# <a name="educationpowerschooldataprovider-resource"></a>educationPowerSchoolDataProvider ресурсов

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Используется для настройки синхронизации профилей данных school при [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) используется в качестве источника ввода.

На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **connectionUrl** | Строка | URL-адрес подключения к экземпляру PowerSchool. |
| **clientId** | Строка |  Идентификатор клиента, используемого для подключения к PowerSchool. |
| **clientSecret** | Строка |  Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool. |
| **schoolsIds** | Коллекция String |  Список школы для синхронизации. |
| **schoolYear** | Строка |  Учебный год для синхронизации. |
| **allowTeachersInMultipleSchools** | Логический |  Указывает, имеет ли источник несколько идентификаторов для одного студент и преподаватель. |
| **пользовательских настроек** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Дополнительные настройки применяется для синхронизации профилей.|

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
