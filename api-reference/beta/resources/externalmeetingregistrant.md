---
title: тип ресурса externalMeetingRegistrant
description: Представляет внешнего регистратора собраний, который зарегистрировался на собрании в Интернете.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 05c386137ea9e062e223eb7854afc4d13458fe30
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565243"
---
# <a name="externalmeetingregistrant-resource-type"></a>тип ресурса externalMeetingRegistrant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет внешнего регистратора собраний, который зарегистрировался на собрании в Интернете.

Наследует от [meetingRegistrantBase](../resources/meetingregistrantbase.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список externalMeetingRegistrants](../api/externalmeetingregistrant-list.md)|[коллекция externalMeetingRegistrant](../resources/externalmeetingregistrant.md)|Получите список объектов [externalMeetingRegistrant](../resources/externalmeetingregistrant.md) и их свойств.|
|[Создание externalMeetingRegistrant](../api/externalmeetingregistrant-post.md)|[externalMeetingRegistrant](../resources/externalmeetingregistrant.md)|Ознакомьтесь с свойствами и отношениями [объекта externalMeetingRegistrant.](../resources/externalmeetingregistrant.md)|
|[Удаление externalMeetingRegistrant](../api/externalmeetingregistrant-delete.md)|Нет|Удаление [объекта externalMeetingRegistrant.](../resources/externalmeetingregistrant.md)|

## <a name="properties"></a>Свойства

| Свойство   | Тип   | Описание                                                                  |
|:-----------|:-------|:-----------------------------------------------------------------------------|
| id         | Строка | Уникальный идентификатор регистратора во внешней системе регистрации. Наследуется [от meetingRegistrantBase](../resources/meetingregistrantbase.md). |
| joinWebUrl | Строка | Уникальный веб-URL-адрес для регистратора, который должен присоединиться к собранию. Наследуется [от meetingRegistrantBase](../resources/meetingregistrantbase.md). Только для чтения.          |
| tenantId   | String | ID клиента этого регистратора, если в Azure Active Directory.               |
| userId     | String | Пользовательский ID этого регистратора, если в Azure Active Directory.                 |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalMeetingRegistrant",
  "baseType": "microsoft.graph.meetingRegistrantBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "userId": "String",
  "tenantId": "String"
}
```
