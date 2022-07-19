---
title: Тип ресурса bookingBusiness
description: Представляет бизнес в Microsoft Bookings.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: ccafc23fc8a1276ec7ffa9df4b0b2c8769142e32
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856297"
---
# <a name="bookingbusiness-resource-type"></a>Тип ресурса bookingBusiness

Пространство имен: microsoft.graph

Представляет бизнес в Microsoft Bookings. Это объект верхнего уровня в Microsoft Bookings API. Он содержит бизнес-информацию и связанные бизнес-объекты, такие как встречи, клиенты, службы и сотрудники.

## <a name="methods"></a>Методы

| Метод  | Возвращаемый тип |Описание|
|:---------------|:--------|:----------|
|[Перечисление bookingBusinesses](../api/bookingbusiness-list.md) | [Коллекция bookingBusiness](bookingbusiness.md) |Получение коллекции объектов **bookingBusiness** в клиенте. |
|[Создание bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | Создайте новую Microsoft Bookings бизнеса. |
|[Получение bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |Чтение свойств и связей объекта **bookingBusiness** .|
|[Обновление](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |Обновление свойств в **объекте bookingBusiness** . |
|[удаление](../api/bookingbusiness-delete.md); | Нет |Удаление объекта **bookingBusiness** . |
|[Создание bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| Создайте новый **bookingAppointment** , выполнив публикацию в коллекции встреч.|
|[Список встреч](../api/bookingbusiness-list-appointments.md) |[Коллекция bookingAppointment](bookingappointment.md)| Получение коллекции **объектов bookingAppointment** .|
|[Создание bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| Создайте объект **bookingCustomer** , выполнив публикацию в коллекции клиентов.|
|[Перечисление клиентов](../api/bookingbusiness-list-customers.md) |[Коллекция bookingCustomer](bookingcustomer.md)| Получение коллекции **объектов bookingCustomer** .|
|[Создание bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| Создайте новую **службу bookingService** , выполнив публикацию в коллекции служб.|
|[Перечисление служб](../api/bookingbusiness-list-services.md) |[Коллекция bookingService](bookingservice.md)| Получение коллекции **объектов bookingService** .|
|[Создание bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| Создайте **объект bookingStaffMember** , выполнив публикацию в коллекции staffMembers.|
|[Перечисление staffMembers](../api/bookingbusiness-list-staffmembers.md) |[Коллекция bookingStaffMember](bookingstaffmember.md)| Получение коллекции **объектов bookingStaffMember** .|
|[Перечисление customQuestions](../api/bookingbusiness-list-customquestions.md)|[Коллекция bookingCustomQuestion](../resources/bookingcustomquestion.md)|Получите ресурсы **bookingCustomQuestion** из **свойства навигации customQuestions** .|
|[Создание bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md)|[bookingCustomQuestion](../resources/bookingcustomquestion.md)|Создайте объект **bookingCustomQuestion** .|
|[Список calendarView](../api/bookingbusiness-list-calendarview.md)|[Коллекция bookingAppointment](bookingappointment.md)|Получение коллекции объектов **bookingAppointment** , которые происходят в указанном диапазоне дат.|
|[публикация](../api/bookingbusiness-publish.md);|Нет|Сделайте страницу планирования этого бизнеса доступной внешним клиентам. **Задайте для свойства isPublished** `true`значение , а свойству **publicUrl** — URL-адрес страницы планирования.|
|[Отмена публикации](../api/bookingbusiness-unpublish.md)|Нет| Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов. **Задайте для свойства isPublished** значение `false`, а **свойству publicUrl** — значение `null`.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|Почтовый адрес компании. Свойство **адреса** вместе с **телефоном** **и webSiteUrl** отображается в нижнем колонтитуле страницы планирования бизнеса. Тип **атрибута** physicalAddress не поддерживается в версии 1.0. Внутренне мы сопоставляем адреса с типом `others`.|
|businessHours|[Коллекция bookingWorkHours](bookingworkhours.md)|Часы работы для бизнеса.|
|businessType|Строка|Тип бизнеса.|
|defaultCurrencyIso|Строка|Код валюты, в которую бизнес использует Microsoft Bookings.|
|displayName|String|Имя компании, которая интерфейсирует с клиентами. Это имя отображается в верхней части страницы планирования бизнеса.|
|email|String|Адрес электронной почты для бизнеса.|
|id|String|Уникальный программный идентификатор для бизнеса. Только для чтения.|
|isPublished|Логический|Страница планирования была доступна внешним клиентам. Используйте действия **публикации** **и отмены публикации** , чтобы задать это свойство. Только для чтения.|
|phone|String|Номер телефона для бизнеса. Свойство **телефона** вместе с **адресом** **и webSiteUrl** отображается в нижнем колонтитуле страницы планирования бизнеса.|
|publicUrl|Строка|URL-адрес страницы планирования, который задается после [публикации](../api/bookingbusiness-publish.md) или отмены [публикации](../api/bookingbusiness-unpublish.md) страницы. Только для чтения.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Указывает, как можно создавать резервирования для этого бизнеса.|
|webSiteUrl|Строка|URL-адрес бизнес-сайта. Свойство **webSiteUrl** вместе с **адресом** **и** телефоном отображается в нижнем колонтитуле страницы планирования бизнеса.|

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|appointments|[Коллекция bookingAppointment](bookingappointment.md)| Все встречи этого бизнеса. Только для чтения. Допускается значение null.|
|calendarView|[Коллекция bookingAppointment](bookingappointment.md)| Набор встреч этого бизнеса в указанном диапазоне дат. Только для чтения. Допускается значение null.|
|Клиентов|[Коллекция bookingCustomer](bookingcustomer.md)| Все клиенты этого бизнеса. Только для чтения. Допускается значение null.|
|customQuestions|[Коллекция bookingCustomQuestion](../resources/bookingcustomquestion.md)| Все пользовательские вопросы этого бизнеса. Только для чтения. Допускается значение null.|
|Услуги|[Коллекция bookingService](bookingservice.md)| Все службы, предлагаемые этим бизнесом. Только для чтения. Допускается значение null.|
|staffMembers|[Коллекция bookingStaffMember](bookingstaffmember.md)| Все сотрудники, предоставляющие услуги в этом бизнесе. Только для чтения. Допускается значение null.|

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


