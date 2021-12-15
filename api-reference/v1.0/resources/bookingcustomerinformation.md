---
title: тип ресурса bookingCustomerInformation
description: Регистрирует свойства клиента для встречи. Встреча будет содержать список сведений о клиентах, и каждое подразделение будет указывать свойства клиента, который является частью этого назначения.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 05e557b69b9a38227a496193d10eb48b8e621370
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525124"
---
# <a name="bookingcustomerinformation-resource-type"></a>тип ресурса bookingCustomerInformation

Пространство имен: microsoft.graph

Регистрирует свойства клиента для встречи. Встреча будет содержать список сведений о клиентах, и каждое подразделение будет указывать свойства клиента, который является частью этого назначения.

Наследует [от bookingCustomerInformationBase](bookingcustomerinformationbase.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|emailAddress|String| SMTP-адрес [bookingCustomer,](../resources/bookingcustomer.md) который бронирует встречу |
|customerId|Строка|ID **bookingCustomer** для этого назначения. Если при назначении не указывается номер, создается новый объект **bookingCustomer.** После набора следует считать **customerId** неуменяемым. |
|location|[location](../resources/location.md)| Представляет сведения о расположении для bookingCustomer, который бронирует встречу. |
|name|String|Имя клиента. |
|notes|String|Заметки от клиента, связанного с этим назначением. Значение можно получить только при чтении этого **bookingAppointment** по его ID. Это свойство можно установить только при первоначальном создании встречи с новым клиентом. После этого значение вычисляется от клиента, представленного **customerId.** |
|phone|String|Номер телефона клиента. |
|timeZone|String|Часовой пояс клиента. Список возможных значений см. в [списке dateTimeTimeZone.](../resources/datetimetimezone.md)|
|customQuestionAnswers|[коллекция bookingQuestionAnswer](../resources/bookingquestionanswer.md)|Он состоит из списка пользовательских вопросов и ответов, данных клиентом в рамках встречи |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingCustomerInformation",
  "baseType": "microsoft.graph.bookingCustomerInformationBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingCustomerInformation",
  "customerId": "String",
  "name": "String",
  "emailAddress": "String",
  "phone": "String",
  "notes": "String",
  "location": {
    "@odata.type": "microsoft.graph.location"
  },
  "timeZone": "String",
  "customQuestionAnswers": [
    {
      "@odata.type": "microsoft.graph.bookingQuestionAnswer"
    }
  ]
}
```

