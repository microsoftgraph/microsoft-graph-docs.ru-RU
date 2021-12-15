---
title: тип ресурса bookingCustomerInformation
description: Регистрирует свойства клиента для встречи. Встреча содержит список сведений о клиентах, и каждое подразделение указывает свойства клиента, который является частью этого назначения.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: d72f54794cc637e7cb90a2f11b59cc2cb026d7ed
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525658"
---
# <a name="bookingcustomerinformation-resource-type"></a>тип ресурса bookingCustomerInformation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Регистрирует свойства клиента для встречи. Встреча содержит список сведений о клиентах, и каждое подразделение указывает свойства клиента, который является частью этого назначения.

Наследует [от bookingCustomerInformationBase](bookingcustomerinformationbase.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|customerId|Строка|ID [bookingCustomer](../resources/bookingcustomer.md) для этого назначения. Если при назначении не указывается номер, создается новый объект **bookingCustomer.** После набора следует считать customerId неуменяемым. |
|customQuestionAnswers|[коллекция bookingQuestionAnswer](../resources/bookingquestionanswer.md)|Он состоит из списка пользовательских вопросов и ответов, данных клиентом в рамках встречи. |
|emailAddress|String| SMTP-адрес **bookingCustomer,** который бронирует встречу. |
|location|[location](../resources/location.md)| Представляет сведения о расположении **для bookingCustomer,** который бронирует встречу. |
|name|String|Имя клиента. |
|notes|String|Заметки от клиента, связанного с этим назначением. Значение можно получить только при чтении этого **bookingAppointment** по его ID. Это свойство можно установить только при первоначальном создании встречи с новым клиентом. После этого значение вычисляется от клиента, представленного **customerId.** |
|phone|String|Номер телефона клиента. |
|timeZone|String|Часовой пояс клиента. Список возможных значений см. в [списке dateTimeTimeZone.](../resources/datetimetimezone.md)|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingCustomerInformation"
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

