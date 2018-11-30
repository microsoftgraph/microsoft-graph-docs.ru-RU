---
title: Тип ресурса bookingBusiness
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 0ea11dcd16a129e6d6648be4b09435c5c052de9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078422"
---
# <a name="bookingbusiness-resource-type"></a>Тип ресурса bookingBusiness

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Представляет бизнеса в Microsoft резервирования. Это объект верхнего уровня в API-Интерфейс Microsoft резервирования. Он содержит бизнес-данных и связанных с ними бизнес-объекты например встреч, клиенты, службы и сотрудников.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список bookingBusinesses](../api/bookingbusiness-list.md) | [bookingBusiness](bookingbusiness.md) коллекции |Получите коллекцию объектов bookingbusiness в клиента. |
|[Создание bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | Создание нового резервирования Microsoft business. |
|[Получение bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |Чтение свойства и связи объекта bookingBusiness.|
|[Update](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |Обновление свойств в объект **bookingBusiness** . |
|[Delete](../api/bookingbusiness-delete.md) | Нет |Удалите объект **bookingBusiness** . |
|[Создание bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| Создайте новый bookingAppointment, отправку сообщений в коллекцию встреч.|
|[Список встреч](../api/bookingbusiness-list-appointments.md) |[bookingAppointment](bookingappointment.md) коллекции| Получите коллекцию объектов bookingAppointment.|
|[Создание bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| Создайте новый bookingCustomer, отправку сообщений в коллекцию customers.|
|[Список клиентов](../api/bookingbusiness-list-customers.md) |[bookingCustomer](bookingcustomer.md) коллекции| Получите коллекцию объектов bookingCustomer.|
|[Создание bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| Создайте новый bookingService, отправку сообщений в коллекцию служб.|
|[Список служб](../api/bookingbusiness-list-services.md) |[bookingService](bookingservice.md) коллекции| Получите коллекцию объектов bookingService.|
|[Создание bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| Создайте новый bookingStaffMember, отправку сообщений в коллекцию staffMembers.|
|[Список staffMembers](../api/bookingbusiness-list-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md) коллекции| Получите коллекцию объектов bookingStaffMember.|
|[Список calendarView](../api/bookingbusiness-list-calendarview.md)|[bookingAppointment](bookingappointment.md) коллекции|Получите коллекцию объектов **bookingAppointment** , что происходит в за указанный диапазон дат.|
|[Публикация](../api/bookingbusiness-publish.md)|Нет|Сделайте доступными странице планирования бизнеса внешним клиентам. Свойства **isPublished** значение true, а свойство **publicUrl** URL-адрес страницы планирования.|
|[Отмена публикации](../api/bookingbusiness-unpublish.md)|Нет| Доступность планирования страницы бизнеса не для внешних клиентов. Присвойте свойству **isPublished** значение false и свойство **publicUrl** значения NULL.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|Почтовый адрес организации. Свойство **адрес** вместе с **телефона** и **webSiteUrl**отображаются в нижнем колонтитуле предприятие планирования страницы.|
|businessHours|[bookingWorkHours](bookingworkhours.md) коллекции|Часы работы для предприятий.|
|businessType|String|Тип бизнеса.|
|defaultCurrencyIso|String|Код для валюты, предприятию работает в Microsoft резервирования.|
|displayName|String|Название организации, который взаимодействует с клиентами. Это имя отображается в верхней части бизнеса, планирование страницы.|
|email|String|Адрес электронной почты для бизнеса.|
|id|String|Уникальный программный идентификатор для бизнеса. Только для чтения.|
|isPublished|Логический|Страница расписания предоставленной внешним клиентам. Для установки этого свойства используется действий **Публикация** и **Отмена публикации** . Только для чтения.|
|phone|String|Номер телефона для бизнеса. Свойство **phone** вместе с **адресом** и **webSiteUrl**отображаются в нижнем колонтитуле предприятие планирования страницы.|
|publicUrl|String|URL-адрес для планирования страницы, которая задается после [публикации](../api/bookingbusiness-publish.md) или [отмены публикации](../api/bookingbusiness-unpublish.md) страницы. Только для чтения.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Указывает, как можно создать резервирования для бизнеса.|
|webSiteUrl|String|URL-адрес веб-сайта бизнеса. Свойство **webSiteUrl** вместе с **адреса**, **Телефон**, отображаются в нижней части страницы планирования бизнес.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Description|
|:---------------|:--------|:----------|
|appointments|[bookingAppointment](bookingappointment.md) коллекции| Все встречи бизнеса. Только для чтения. Допускается значение null.|
|calendarView|[bookingAppointment](bookingappointment.md) коллекции| Набор встреч в этом бизнеса в указанный диапазон дат. Только для чтения. Допускается значение null.|
|Клиенты|[bookingCustomer](bookingcustomer.md) коллекции| Все клиенты бизнеса. Только для чтения. Допускается значение null.|
|службы|[bookingService](bookingservice.md) коллекции| Всех служб, предоставляемых бизнеса. Только для чтения. Допускается значение null.|
|staffMembers|[bookingStaffMember](bookingstaffmember.md) коллекции| Все сотрудники, предоставляющие службы в этом бизнеса. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingBusiness"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}],
  "businessType": "String",
  "defaultCurrencyIso": "String",
  "displayName": "String",
  "email": "String",
  "id": "String (identifier)",
  "isPublished": true,
  "phone": "String",
  "publicUrl": "String",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "webSiteUrl": "String"
}

```

## <a name="see-also"></a>См. также


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->