---
title: Тип ресурса bookingCustomerInformation
description: Регистрирует свойства клиента для встречи. Встреча содержит список сведений о клиенте, и каждое подразделение указывает свойства клиента, который является частью этой встречи.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2ad296651030f8b208dacafcb4fbe7b424e08430
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160379"
---
# <a name="bookingcustomerinformation-resource-type"></a>Тип ресурса bookingCustomerInformation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Регистрирует свойства клиента для встречи. Встреча содержит список сведений о клиенте, и каждое подразделение указывает свойства клиента, который является частью этой встречи.

Наследуется [от bookingCustomerInformationBase](bookingcustomerinformationbase.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|customerId|Строка|Идентификатор объекта [bookingCustomer](../resources/bookingcustomer.md) для этой встречи. Если при создании встречи не указан идентификатор, создается новый объект **bookingCustomer** . После установки идентификатор клиента следует считать неизменяемым. |
|customQuestionAnswers|[Коллекция bookingQuestionAnswer](../resources/bookingquestionanswer.md)|Он состоит из списка пользовательских вопросов и ответов, заданных клиентом в рамках встречи. |
|emailAddress|String| SMTP-адрес **bookingCustomer** , который резервировать встречу. |
|location|[location](../resources/location.md)| Представляет сведения о расположении **для bookingCustomer** , который резервирует встречу. |
|name|String|Имя клиента. |
|notes|String|Заметки от клиента, связанного с этой встречей. Значение можно получить только при чтении **этого объекта bookingAppointment** по его идентификатору. Это свойство можно задать только при первоначальном создании встречи с новым клиентом. После этого значение вычисляется из клиента, представленного **идентификатором клиента**. |
|phone|String|Номер телефона клиента. |
|smsNotificationsEnabled|Boolean|Указывает, SMS уведомления будут отправляться клиенту для встречи.
|timeZone|String|Часовой пояс клиента. Список возможных значений см. в [разделе dateTimeTimeZone](../resources/datetimetimezone.md).|

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
  "smsNotificationsEnabled": "Boolean",
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

