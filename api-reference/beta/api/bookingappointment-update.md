---
title: Обновление букингаппоинтмент
description: Обновление свойств объекта Букингаппоинтмент в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: aac9ae93e1a333bdf06f439ee3fddeca39dd4ade
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439345"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="2978f-103">Обновление букингаппоинтмент</span><span class="sxs-lookup"><span data-stu-id="2978f-103">Update bookingappointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2978f-104">Обновление свойств объекта [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="2978f-104">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2978f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2978f-105">Permissions</span></span>
<span data-ttu-id="2978f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2978f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2978f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2978f-108">Permission type</span></span>      | <span data-ttu-id="2978f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2978f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2978f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2978f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2978f-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="2978f-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2978f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2978f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2978f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2978f-113">Not supported.</span></span>   |
|<span data-ttu-id="2978f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2978f-114">Application</span></span> | <span data-ttu-id="2978f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2978f-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2978f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2978f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="2978f-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2978f-117">Optional request headers</span></span>
| <span data-ttu-id="2978f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2978f-118">Name</span></span>       | <span data-ttu-id="2978f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2978f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2978f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2978f-120">Authorization</span></span>  | <span data-ttu-id="2978f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2978f-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2978f-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2978f-122">Request body</span></span>
<span data-ttu-id="2978f-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2978f-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2978f-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2978f-126">Property</span></span>     | <span data-ttu-id="2978f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2978f-127">Type</span></span>   |<span data-ttu-id="2978f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2978f-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2978f-129">Кустомеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="2978f-129">customerEmailAddress</span></span>|<span data-ttu-id="2978f-130">String</span><span class="sxs-lookup"><span data-stu-id="2978f-130">String</span></span>|<span data-ttu-id="2978f-131">SMTP-адрес [букингкустомер](../resources/bookingcustomer.md) , который зарезервировано встречу.</span><span class="sxs-lookup"><span data-stu-id="2978f-131">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="2978f-132">customerId</span><span class="sxs-lookup"><span data-stu-id="2978f-132">customerId</span></span>|<span data-ttu-id="2978f-133">String</span><span class="sxs-lookup"><span data-stu-id="2978f-133">String</span></span>|<span data-ttu-id="2978f-134">Идентификатор [букингкустомер](../resources/bookingcustomer.md) для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="2978f-134">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="2978f-135">Если при создании встречи не указан идентификатор, создается новый объект **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="2978f-135">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="2978f-136">После установки необходимо учесть неизменность **customerId** .</span><span class="sxs-lookup"><span data-stu-id="2978f-136">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="2978f-137">Кустомерлокатион</span><span class="sxs-lookup"><span data-stu-id="2978f-137">customerLocation</span></span>|[<span data-ttu-id="2978f-138">location</span><span class="sxs-lookup"><span data-stu-id="2978f-138">location</span></span>](../resources/location.md)|<span data-ttu-id="2978f-139">Представляет сведения о расположении для [букингкустомер](../resources/bookingcustomer.md) , который зарезервировано встречу.</span><span class="sxs-lookup"><span data-stu-id="2978f-139">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="2978f-140">customerName</span><span class="sxs-lookup"><span data-stu-id="2978f-140">customerName</span></span>|<span data-ttu-id="2978f-141">String</span><span class="sxs-lookup"><span data-stu-id="2978f-141">String</span></span>|<span data-ttu-id="2978f-142">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="2978f-142">The customer's name.</span></span>|
|<span data-ttu-id="2978f-143">Кустомернотес</span><span class="sxs-lookup"><span data-stu-id="2978f-143">customerNotes</span></span>|<span data-ttu-id="2978f-144">String</span><span class="sxs-lookup"><span data-stu-id="2978f-144">String</span></span>|<span data-ttu-id="2978f-145">Примечания от клиента, связанного с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="2978f-145">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="2978f-146">Значение можно получить только при чтении этого **букингаппоинтмент** по его идентификатору.</span><span class="sxs-lookup"><span data-stu-id="2978f-146">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="2978f-147">Это свойство можно задать только при первоначальном создании встречи с новым клиентом.</span><span class="sxs-lookup"><span data-stu-id="2978f-147">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="2978f-148">После этой точки значение вычисляется от клиента, представленного **customerId**.</span><span class="sxs-lookup"><span data-stu-id="2978f-148">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="2978f-149">Кустомерфоне</span><span class="sxs-lookup"><span data-stu-id="2978f-149">customerPhone</span></span>|<span data-ttu-id="2978f-150">String</span><span class="sxs-lookup"><span data-stu-id="2978f-150">String</span></span>|<span data-ttu-id="2978f-151">Номер телефона клиента.</span><span class="sxs-lookup"><span data-stu-id="2978f-151">The customer's phone number.</span></span>|
|<span data-ttu-id="2978f-152">duration</span><span class="sxs-lookup"><span data-stu-id="2978f-152">duration</span></span>|<span data-ttu-id="2978f-153">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="2978f-153">Duration</span></span>|<span data-ttu-id="2978f-154">Длительность встречи, обозначенная в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="2978f-154">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="2978f-155">end</span><span class="sxs-lookup"><span data-stu-id="2978f-155">end</span></span>|[<span data-ttu-id="2978f-156">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2978f-156">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="2978f-157">Дата, время и часовой пояс, в котором заканчивается встреча.</span><span class="sxs-lookup"><span data-stu-id="2978f-157">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="2978f-158">Инвоицеамаунт</span><span class="sxs-lookup"><span data-stu-id="2978f-158">invoiceAmount</span></span>|<span data-ttu-id="2978f-159">Двойное</span><span class="sxs-lookup"><span data-stu-id="2978f-159">Double</span></span>|<span data-ttu-id="2978f-160">Сумма счета в счете.</span><span class="sxs-lookup"><span data-stu-id="2978f-160">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="2978f-161">Инвоицедате</span><span class="sxs-lookup"><span data-stu-id="2978f-161">invoiceDate</span></span>|[<span data-ttu-id="2978f-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2978f-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="2978f-163">Дата, время и часовой пояс накладной для данной встречи.</span><span class="sxs-lookup"><span data-stu-id="2978f-163">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="2978f-164">Инвоицеид</span><span class="sxs-lookup"><span data-stu-id="2978f-164">invoiceId</span></span>|<span data-ttu-id="2978f-165">String</span><span class="sxs-lookup"><span data-stu-id="2978f-165">String</span></span>|<span data-ttu-id="2978f-166">Идентификатор счета.</span><span class="sxs-lookup"><span data-stu-id="2978f-166">The ID of the invoice.</span></span>|
|<span data-ttu-id="2978f-167">Инвоицестатус</span><span class="sxs-lookup"><span data-stu-id="2978f-167">invoiceStatus</span></span>|<span data-ttu-id="2978f-168">string</span><span class="sxs-lookup"><span data-stu-id="2978f-168">string</span></span>| <span data-ttu-id="2978f-169">Статус счета.</span><span class="sxs-lookup"><span data-stu-id="2978f-169">The status of the invoice.</span></span> <span data-ttu-id="2978f-170">Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span><span class="sxs-lookup"><span data-stu-id="2978f-170">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="2978f-171">Инвоицеурл</span><span class="sxs-lookup"><span data-stu-id="2978f-171">invoiceUrl</span></span>|<span data-ttu-id="2978f-172">String</span><span class="sxs-lookup"><span data-stu-id="2978f-172">String</span></span>|<span data-ttu-id="2978f-173">URL-адрес счета в книгах корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="2978f-173">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="2978f-174">Оптаутофкустомеремаил</span><span class="sxs-lookup"><span data-stu-id="2978f-174">optOutOfCustomerEmail</span></span>|<span data-ttu-id="2978f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="2978f-175">Boolean</span></span>|<span data-ttu-id="2978f-176">Значение true указывает, что [букингкустомер](../resources/bookingcustomer.md) для этой встречи не хочет получать подтверждение для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="2978f-176">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="2978f-177">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="2978f-177">postBuffer</span></span>|<span data-ttu-id="2978f-178">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="2978f-178">Duration</span></span>|<span data-ttu-id="2978f-179">Количество времени, которое необходимо зарезервировать после окончания встречи, для очистки в качестве примера.</span><span class="sxs-lookup"><span data-stu-id="2978f-179">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="2978f-180">Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="2978f-180">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="2978f-181">пребуфер</span><span class="sxs-lookup"><span data-stu-id="2978f-181">preBuffer</span></span>|<span data-ttu-id="2978f-182">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="2978f-182">Duration</span></span>|<span data-ttu-id="2978f-183">Количество времени, которое необходимо зарезервировать до начала встречи, в качестве примера для подготовки.</span><span class="sxs-lookup"><span data-stu-id="2978f-183">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="2978f-184">Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="2978f-184">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="2978f-185">Цена</span><span class="sxs-lookup"><span data-stu-id="2978f-185">price</span></span>|<span data-ttu-id="2978f-186">Двойное</span><span class="sxs-lookup"><span data-stu-id="2978f-186">Double</span></span>|<span data-ttu-id="2978f-187">Обычная цена для встречи с указанным [букингсервице](../resources/bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="2978f-187">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="2978f-188">Прицетипе</span><span class="sxs-lookup"><span data-stu-id="2978f-188">priceType</span></span>|<span data-ttu-id="2978f-189">string</span><span class="sxs-lookup"><span data-stu-id="2978f-189">string</span></span>| <span data-ttu-id="2978f-190">Параметр, обеспечивающий гибкость для структуры ценообразования служб.</span><span class="sxs-lookup"><span data-stu-id="2978f-190">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="2978f-191">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="2978f-191">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="2978f-192">напоминания</span><span class="sxs-lookup"><span data-stu-id="2978f-192">reminders</span></span>|<span data-ttu-id="2978f-193">Коллекция [букингреминдер](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="2978f-193">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="2978f-194">Коллекция напоминаний о клиентах, отправленных для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="2978f-194">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="2978f-195">Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="2978f-195">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="2978f-196">Селфсервицеаппоинтментид</span><span class="sxs-lookup"><span data-stu-id="2978f-196">selfServiceAppointmentId</span></span>|<span data-ttu-id="2978f-197">String</span><span class="sxs-lookup"><span data-stu-id="2978f-197">String</span></span>|<span data-ttu-id="2978f-198">Дополнительный идентификатор отслеживания для встречи, если встреча создана непосредственно клиентом на странице планирования, в отличие от сотрудника от имени клиента;.</span><span class="sxs-lookup"><span data-stu-id="2978f-198">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="2978f-199">serviceId</span><span class="sxs-lookup"><span data-stu-id="2978f-199">serviceId</span></span>|<span data-ttu-id="2978f-200">String</span><span class="sxs-lookup"><span data-stu-id="2978f-200">String</span></span>|<span data-ttu-id="2978f-201">Идентификатор [букингсервице](../resources/bookingservice.md) , связанный с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="2978f-201">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="2978f-202">Сервицелокатион</span><span class="sxs-lookup"><span data-stu-id="2978f-202">serviceLocation</span></span>|[<span data-ttu-id="2978f-203">location</span><span class="sxs-lookup"><span data-stu-id="2978f-203">location</span></span>](../resources/location.md)|<span data-ttu-id="2978f-204">Место доставки службы.</span><span class="sxs-lookup"><span data-stu-id="2978f-204">The location where the service is delivered.</span></span>|
|<span data-ttu-id="2978f-205">Служба</span><span class="sxs-lookup"><span data-stu-id="2978f-205">serviceName</span></span>|<span data-ttu-id="2978f-206">String</span><span class="sxs-lookup"><span data-stu-id="2978f-206">String</span></span>|<span data-ttu-id="2978f-207">Имя **букингсервице** , связанного с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="2978f-207">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="2978f-208">Это свойство является необязательным при создании новой встречи.</span><span class="sxs-lookup"><span data-stu-id="2978f-208">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="2978f-209">Если он не указан, то он вычисляется из службы, связанной с встречей, с помощью свойства **serviceId** .</span><span class="sxs-lookup"><span data-stu-id="2978f-209">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="2978f-210">Сервиценотес</span><span class="sxs-lookup"><span data-stu-id="2978f-210">serviceNotes</span></span>|<span data-ttu-id="2978f-211">String</span><span class="sxs-lookup"><span data-stu-id="2978f-211">String</span></span>|<span data-ttu-id="2978f-212">Заметки из [букингстаффмембер](../resources/bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="2978f-212">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="2978f-213">Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="2978f-213">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="2978f-214">Стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="2978f-214">staffMemberIds</span></span>|<span data-ttu-id="2978f-215">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2978f-215">String collection</span></span>|<span data-ttu-id="2978f-216">Идентификатор каждого [букингстаффмембер](../resources/bookingstaffmember.md) , запланированного в этой встрече.</span><span class="sxs-lookup"><span data-stu-id="2978f-216">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="2978f-217">начать</span><span class="sxs-lookup"><span data-stu-id="2978f-217">start</span></span>|[<span data-ttu-id="2978f-218">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2978f-218">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="2978f-219">Дата, время и часовой пояс, с которого начинается встреча.</span><span class="sxs-lookup"><span data-stu-id="2978f-219">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="2978f-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="2978f-220">Response</span></span>
<span data-ttu-id="2978f-p113">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2978f-p113">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2978f-223">Пример</span><span class="sxs-lookup"><span data-stu-id="2978f-223">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2978f-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="2978f-224">Request</span></span>
<span data-ttu-id="2978f-225">В следующем примере дата обслуживания изменяется на день, а также обновляется и Дата выставления счета.</span><span class="sxs-lookup"><span data-stu-id="2978f-225">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2978f-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="2978f-226">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2978f-227">C#</span><span class="sxs-lookup"><span data-stu-id="2978f-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2978f-228">Javascript</span><span class="sxs-lookup"><span data-stu-id="2978f-228">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2978f-229">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2978f-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2978f-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="2978f-230">Response</span></span>
<span data-ttu-id="2978f-231">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2978f-231">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
