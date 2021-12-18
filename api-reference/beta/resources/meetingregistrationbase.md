---
title: тип ресурса meetingRegistrationBase
description: Содержит сведения о регистрации базовых собраний.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 01bdfeaa222464c7e7b44bf5f92482b2b1c3d4e0
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565230"
---
# <a name="meetingregistrationbase-resource-type"></a>тип ресурса meetingRegistrationBase

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет базовые сведения о регистрации собрания в Интернете.

Базовый тип [meetingRegistration](meetingregistration.md) и [externalMeetingRegistration](externalmeetingregistration.md).

> [!TIP]
> Это абстрактный тип, который нельзя использовать напрямую. Вместо этого используйте производный [тип meetingRegistration](meetingregistration.md) или [externalMeetingRegistration.](externalmeetingregistration.md)

## <a name="properties"></a>Свойства

| Свойство          | Тип                                       | Описание                                 |
|:------------------|:-------------------------------------------|:--------------------------------------------|
| allowedRegistrant | [meetingAudience](#meetingaudience-values) | Указывает, кто может зарегистрироваться для собрания. |

### <a name="meetingaudience-values"></a>значения meetingAudience

| Значение              | Описание                                                            |
|--------------------|------------------------------------------------------------------------|
| все           | Зарегистрироваться на собрание может каждый.                                 |
| organization       | Все в организации организатора могут зарегистрироваться на собрание. |
| unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать.                      |

## <a name="relationships"></a>Связи

| Связь | Тип                                                         | Описание                        |
|:-------------|:-------------------------------------------------------------|:-----------------------------------|
| регистраторы  | [коллекция meetingRegistrantBase](meetingregistrantbase.md) | Регистраторы собрания в Интернете. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.meetingRegistrationBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.meetingRegistrationBase",
  "allowedRegistrant": "String",

  "registrants": [{ "@odata.type": "microsoft.graph.meetingRegistrantBase" }]
}
```
