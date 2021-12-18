---
title: тип ресурса externalMeetingRegistration
description: Содержит сведения о регистрации внешних собраний.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: af59114df32f24c36c1cd8d75e344162ac6e0d88
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565237"
---
# <a name="externalmeetingregistration-resource-type"></a>тип ресурса externalMeetingRegistration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет внешние сведения о регистрации собрания в Интернете.

Наследует [от meetingRegistrationBase](meetingregistrationbase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание externalMeetingRegistration](../api/externalmeetingregistration-post.md)|[externalMeetingRegistration](externalmeetingregistration.md)|Создайте [новый объект externalMeetingRegistration.](externalmeetingregistration.md)|
|[Get externalMeetingRegistration](../api/externalmeetingregistration-get.md)|[externalMeetingRegistration](externalmeetingregistration.md)|Ознакомьтесь с свойствами и отношениями [объекта externalMeetingRegistration.](externalmeetingregistration.md)|
|[Удаление externalMeetingRegistration](../api/externalmeetingregistration-delete.md)|Нет|Удаление [объекта externalMeetingRegistration.](externalmeetingregistration.md)|

## <a name="properties"></a>Свойства

| Свойство          | Тип                                       | Описание                                 |
|:------------------|:-------------------------------------------|:--------------------------------------------|
| allowedRegistrant | [meetingAudience](#meetingaudience-values) | Указывает, кто может зарегистрироваться для собрания. Наследуется [от meetingRegistrationBase](meetingregistrationbase.md). |

### <a name="meetingaudience-values"></a>значения meetingAudience

| Значение              | Описание                                                            |
|--------------------|------------------------------------------------------------------------|
| все           | Зарегистрироваться на собрание может каждый.                                 |
| organization       | Все в организации организатора могут зарегистрироваться на собрание. |
| unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать.                      |

## <a name="relationships"></a>Связи

| Связь | Тип                                                                 | Описание                        |
|:-------------|:---------------------------------------------------------------------|:-----------------------------------|
| регистраторы  | [коллекция externalMeetingRegistrant](externalmeetingregistrant.md) | Регистраторы собрания в Интернете. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalMeetingRegistration",
  "baseType": "microsoft.graph.meetingRegistrationBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalMeetingRegistration",
  "allowedRegistrant": "String",

  "registrants": [{ "@odata.type": "microsoft.graph.externalMeetingRegistrant" }]
}
```
