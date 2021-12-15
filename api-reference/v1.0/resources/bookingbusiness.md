---
title: Тип ресурса bookingBusiness
description: Представляет бизнес в Microsoft Bookings.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c60010301bcc40083e7e30d1d3a286e1b773e1d5
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526761"
---
# <a name="bookingbusiness-resource-type"></a>Тип ресурса bookingBusiness

Пространство имен: microsoft.graph

Представляет бизнес в Microsoft Bookings. Это объект верхнего уровня в API Microsoft Bookings. Он содержит бизнес-информацию и связанные с ними бизнес-объекты, такие как встречи, клиенты, службы и сотрудники.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список bookingBusinesses](../api/bookingbusiness-list.md) | [коллекция bookingBusiness](bookingbusiness.md) |Получите коллекцию **объектов bookingBusiness** в клиенте. |
|[Создание bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | Создание нового бизнеса Microsoft Bookings. |
|[Get bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |Чтение свойств и связей объекта **bookingBusiness.**|
|[Обновление](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |Обновление свойств объекта **bookingBusiness.** |
|[удаление](../api/bookingbusiness-delete.md); | Нет |Удаление **объекта bookingBusiness.** |
|[Создание bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| Создайте новое **bookingAppointment,** разместив в коллекции встреч.|
|[Список встреч](../api/bookingbusiness-list-appointments.md) |[коллекция bookingAppointment](bookingappointment.md)| Получите **коллекцию объектов bookingAppointment.**|
|[Создание bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| Создайте новый **bookingCustomer,** разместив в коллекции клиентов.|
|[Список клиентов](../api/bookingbusiness-list-customers.md) |[коллекция bookingCustomer](bookingcustomer.md)| Получите **коллекцию объектов bookingCustomer.**|
|[Создание bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| Создайте новую **службу бронирования,** разместив ее в коллекции служб.|
|[Службы списка](../api/bookingbusiness-list-services.md) |[коллекция bookingService](bookingservice.md)| Получите **коллекцию объектов bookingService.**|
|[Создание bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| Создайте новое **bookingStaffMember,** разместив в коллекции staffMembers.|
|[Список staffMembers](../api/bookingbusiness-list-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md) collection| Получите **коллекцию объектов bookingStaffMember.**|
|[Список customQuestions](../api/bookingbusiness-list-customquestions.md)|[коллекция bookingCustomQuestion](../resources/bookingcustomquestion.md)|Получите ресурсы **bookingCustomQuestion** из свойства **навигации customQuestions.**|
|[Создание bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md)|[bookingCustomQuestion](../resources/bookingcustomquestion.md)|Создайте новый **объект bookingCustomQuestion.**|
|[Список calendarView](../api/bookingbusiness-list-calendarview.md)|[коллекция bookingAppointment](bookingappointment.md)|Получите коллекцию **объектов bookingAppointment,** которая происходит в указанном диапазоне дат.|
|[Публикация](../api/bookingbusiness-publish.md)|Нет|Сделайте страницу планирования этого бизнеса доступной для внешних клиентов. **Задай свойство isPublished** свойству `true` и **свойству publicUrl** URL-адрес страницы планирования.|
|[Неопубликовка](../api/bookingbusiness-unpublish.md)|Нет| Сделать страницу планирования этого бизнеса недоступным для внешних клиентов. Установите **свойство isPublished** `false` и **свойство publicUrl** `null` .|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|Адрес улицы бизнеса. Свойство **адресов** вместе с **телефоном** **и webSiteUrl** отображаются в подножке страницы планирования бизнеса. Тип **атрибута** physicalAddress не поддерживается в v1.0. Внутренне мы относям адреса к типу `others` .|
|businessHours|[коллекция bookingWorkHours](bookingworkhours.md)|Часы работы для бизнеса.|
|businessType|Строка|Тип бизнеса.|
|defaultCurrencyIso|Строка|Код валюты, в которую бизнес работает в Microsoft Bookings.|
|displayName|Строка|Имя бизнеса, которое взаимодействует с клиентами. Это имя отображается в верхней части страницы планирования бизнеса.|
|email|String|Адрес электронной почты для бизнеса.|
|id|Строка|Уникальный программный идентификатор для бизнеса. Только для чтения.|
|isPublished|Boolean|Страница планирования стала доступной для внешних клиентов. Для этого **свойства** используйте публикацию и неопубликованные действия.  Только для чтения.|
|phone|String|Номер телефона для бизнеса. Свойство **телефона** вместе с **адресом** **и webSiteUrl** отображаются в подножке страницы планирования бизнеса.|
|publicUrl|Строка|URL-адрес страницы планирования, заданный [](../api/bookingbusiness-publish.md) после публикации или публикации [страницы.](../api/bookingbusiness-unpublish.md) Только для чтения.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Указывает, как можно создавать заказы для этого бизнеса.|
|webSiteUrl|Строка|URL-адрес веб-сайта бизнеса. Свойство **webSiteUrl** вместе с **адресом** **и** телефоном отображаются в подножке страницы планирования бизнеса.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|appointments|[коллекция bookingAppointment](bookingappointment.md)| Все встречи этого бизнеса. Только для чтения. Допускается значение null.|
|calendarView|[коллекция bookingAppointment](bookingappointment.md)| Набор назначений этого бизнеса в указанном диапазоне дат. Только для чтения. Допускается значение null.|
|клиенты|[коллекция bookingCustomer](bookingcustomer.md)| Все клиенты этого бизнеса. Только для чтения. Допускается значение null.|
|customQuestions|[коллекция bookingCustomQuestion](../resources/bookingcustomquestion.md)| Все настраиваемые вопросы этого бизнеса. Только для чтения. Допускается значение null.|
|службы|[коллекция bookingService](bookingservice.md)| Все службы, предлагаемые этим бизнесом. Только для чтения. Допускается значение null.|
|staffMembers|[bookingStaffMember](bookingstaffmember.md) collection| Все сотрудники, которые предоставляют услуги в этом бизнесе. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


