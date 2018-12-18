---
title: educationPowerSchoolDataProvider ресурсов
description: Используется для настройки синхронизации профилей данных school при PowerSchool используется в качестве источника ввода.
author: mmast-msft
ms.openlocfilehash: 714866d03c70aae8ea03a27b63fb3efbb4fa5ba4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312805"
---
# <a name="educationpowerschooldataprovider-resource"></a>educationPowerSchoolDataProvider ресурсов

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Используется для настройки синхронизации профилей данных school при [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) используется в качестве источника ввода.

На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **connectionUrl** | String. | URL-адрес подключения к экземпляру PowerSchool. |
| **clientId** | String. |  Идентификатор клиента, используемого для подключения к PowerSchool. |
| **clientSecret** | String. |  Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool. |
| **schoolsIds** | Коллекция String |  Список школы для синхронизации. |
| **schoolYear** | String. |  Учебный год для синхронизации. |
| **allowTeachersInMultipleSchools** | Boolean. |  Указывает, имеет ли источник несколько идентификаторов для одного студент и преподаватель. |
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
