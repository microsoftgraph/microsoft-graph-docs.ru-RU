---
title: Тип ресурса Букингбусинесс
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 314228247131386363da89272d459eb68e022e6c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508012"
---
# <a name="bookingbusiness-resource-type"></a>Тип ресурса Букингбусинесс

Пространство имен: Microsoft. Graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет бизнес в книгах корпорации Майкрософт. Это объект верхнего уровня в API Microsoft Books. Он содержит деловые сведения и связанные бизнес-объекты, такие как встречи, клиенты, службы и сотрудники.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список Букингбусинессес](../api/bookingbusiness-list.md) | Коллекция [букингбусинесс](bookingbusiness.md) |Получение коллекции объектов букингбусинесс в клиенте. |
|[Создание Букингбусинесс](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | Создание новой книги Майкрософт для бизнеса. |
|[Получение Букингбусинесс](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |Чтение свойств и связей объекта Букингбусинесс.|
|[обновление](../api/bookingbusiness-update.md). | [bookingBusiness](bookingbusiness.md) |Обновление свойств объекта **букингбусинесс** . |
|[удаление](../api/bookingbusiness-delete.md); | Нет |Удаление объекта **букингбусинесс** . |
|[Создание Букингаппоинтмент](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| Создание нового Букингаппоинтмент путем публикации в коллекции встреч.|
|[Список встреч](../api/bookingbusiness-list-appointments.md) |Коллекция [букингаппоинтмент](bookingappointment.md)| Получение коллекции объектов Букингаппоинтмент.|
|[Создание Букингкустомер](../api/bookingbusiness-post-customers.md) |[букингкустомер](bookingcustomer.md)| Создание нового Букингкустомер путем публикации в коллекции Customers.|
|[Перечисление клиентов](../api/bookingbusiness-list-customers.md) |Коллекция [букингкустомер](bookingcustomer.md)| Получение коллекции объектов Букингкустомер.|
|[Создание Букингсервице](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| Создание нового Букингсервице путем публикации в коллекции служб.|
|[Список служб](../api/bookingbusiness-list-services.md) |Коллекция [букингсервице](bookingservice.md)| Получение коллекции объектов Букингсервице.|
|[Создание Букингстаффмембер](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| Создание нового Букингстаффмембер путем отправки в коллекцию Стаффмемберс.|
|[Список Стаффмемберс](../api/bookingbusiness-list-staffmembers.md) |Коллекция [букингстаффмембер](bookingstaffmember.md)| Получение коллекции объектов Букингстаффмембер.|
|[Список calendarView](../api/bookingbusiness-list-calendarview.md)|Коллекция [букингаппоинтмент](bookingappointment.md)|Получение коллекции объектов **букингаппоинтмент** , выполняемых в указанном диапазоне дат.|
|[publish](../api/bookingbusiness-publish.md)|Нет|Сделайте страницу планирования для этого бизнеса доступной внешним клиентам. Задайте для свойства **публикации** значение true, а свойству **публикурл** — URL-адрес страницы планирования.|
|[unpublish](../api/bookingbusiness-unpublish.md)|Нет| Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов. Задайте для свойства **publishs** значение false, а свойству **публикурл** — значение null.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|Адрес в почтовом ящике организации. Свойство **Address** вместе с **телефоном** и **вебситеурл**отображается в нижнем колонтитуле страницы бизнес-планирования.|
|businessHours|Коллекция [букингворкхаурс](bookingworkhours.md)|Количество часов работы для бизнеса.|
|бусинесстипе|String|Тип бизнеса.|
|дефаулткурренциисо|String|Код валюты, в которой работает предприятие, в Microsoft Books.|
|displayName|Строка|Название организации, которая взаимодействует с клиентами. Это имя отображается в верхней части страницы "планирование бизнеса".|
|email|String|Адрес электронной почты для бизнеса.|
|id|Строка|Уникальный программный идентификатор для бизнеса. Только для чтения.|
|Публикации|Логический|Страница планирования стала доступна внешним клиентам. Для задания этого свойства используйте действия " **опубликовать** " и " **отменить публикацию** ". Только для чтения.|
|phone|String|Номер телефона для бизнеса. Свойство **Phone** вместе с **адресами** и **вебситеурл**отображается в нижнем колонтитуле страницы бизнес-планирования.|
|публикурл|String|URL-адрес страницы расписания, который задается после [публикации](../api/bookingbusiness-publish.md) или [отмены публикации](../api/bookingbusiness-unpublish.md) страницы. Только для чтения.|
|счедулингполици|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Указывает, как можно создавать резервирования для этого бизнеса.|
|вебситеурл|String|URL-адрес веб-сайта компании. Свойство **вебситеурл** вместе с параметром **Address**( **Телефон**) отображается в нижнем колонтитуле страницы бизнес-планирования.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|appointments|Коллекция [букингаппоинтмент](bookingappointment.md)| Все встречи этого бизнеса. Только для чтения. Допускается значение null.|
|calendarView|Коллекция [букингаппоинтмент](bookingappointment.md)| Набор встреч этого бизнеса в указанном диапазоне дат. Только для чтения. Допускается значение null.|
|TAP|Коллекция [букингкустомер](bookingcustomer.md)| Все клиенты этого предприятия. Только для чтения. Допускается значение null.|
|служб|Коллекция [букингсервице](bookingservice.md)| Все службы, предлагаемые этим бизнесом. Только для чтения. Допускается значение null.|
|стаффмемберс|Коллекция [букингстаффмембер](bookingstaffmember.md)| Все сотрудники, которые предоставляют услуги в этом бизнесе. Только для чтения. Допускается значение null.|

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

## <a name="see-also"></a>См. также


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
