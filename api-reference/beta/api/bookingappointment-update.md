---
title: Обновление букингаппоинтмент
description: Обновление свойств объекта Букингаппоинтмент в указанном букингбусинесс.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 58b6ce47cedca752cbbe151805a0ba1fd9c78cdf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43367540"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="80602-103">Обновление букингаппоинтмент</span><span class="sxs-lookup"><span data-stu-id="80602-103">Update bookingappointment</span></span>

<span data-ttu-id="80602-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80602-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80602-105">Обновление свойств объекта [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="80602-105">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="80602-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80602-106">Permissions</span></span>
<span data-ttu-id="80602-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80602-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80602-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80602-109">Permission type</span></span>      | <span data-ttu-id="80602-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80602-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80602-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80602-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="80602-112">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="80602-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="80602-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80602-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80602-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80602-114">Not supported.</span></span>   |
|<span data-ttu-id="80602-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80602-115">Application</span></span> | <span data-ttu-id="80602-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80602-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="80602-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80602-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="80602-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80602-118">Optional request headers</span></span>
| <span data-ttu-id="80602-119">Имя</span><span class="sxs-lookup"><span data-stu-id="80602-119">Name</span></span>       | <span data-ttu-id="80602-120">Описание</span><span class="sxs-lookup"><span data-stu-id="80602-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="80602-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80602-121">Authorization</span></span>  | <span data-ttu-id="80602-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="80602-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="80602-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80602-123">Request body</span></span>
<span data-ttu-id="80602-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="80602-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="80602-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="80602-127">Property</span></span>     | <span data-ttu-id="80602-128">Тип</span><span class="sxs-lookup"><span data-stu-id="80602-128">Type</span></span>   |<span data-ttu-id="80602-129">Описание</span><span class="sxs-lookup"><span data-stu-id="80602-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80602-130">кустомеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="80602-130">customerEmailAddress</span></span>|<span data-ttu-id="80602-131">String</span><span class="sxs-lookup"><span data-stu-id="80602-131">String</span></span>|<span data-ttu-id="80602-132">SMTP-адрес [букингкустомер](../resources/bookingcustomer.md) , который зарезервировано встречу.</span><span class="sxs-lookup"><span data-stu-id="80602-132">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="80602-133">customerId</span><span class="sxs-lookup"><span data-stu-id="80602-133">customerId</span></span>|<span data-ttu-id="80602-134">String</span><span class="sxs-lookup"><span data-stu-id="80602-134">String</span></span>|<span data-ttu-id="80602-135">Идентификатор [букингкустомер](../resources/bookingcustomer.md) для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="80602-135">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="80602-136">Если при создании встречи не указан идентификатор, создается новый объект **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="80602-136">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="80602-137">После установки необходимо учесть неизменность **customerId** .</span><span class="sxs-lookup"><span data-stu-id="80602-137">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="80602-138">кустомерлокатион</span><span class="sxs-lookup"><span data-stu-id="80602-138">customerLocation</span></span>|[<span data-ttu-id="80602-139">location</span><span class="sxs-lookup"><span data-stu-id="80602-139">location</span></span>](../resources/location.md)|<span data-ttu-id="80602-140">Представляет сведения о расположении для [букингкустомер](../resources/bookingcustomer.md) , который зарезервировано встречу.</span><span class="sxs-lookup"><span data-stu-id="80602-140">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="80602-141">customerName</span><span class="sxs-lookup"><span data-stu-id="80602-141">customerName</span></span>|<span data-ttu-id="80602-142">String</span><span class="sxs-lookup"><span data-stu-id="80602-142">String</span></span>|<span data-ttu-id="80602-143">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="80602-143">The customer's name.</span></span>|
|<span data-ttu-id="80602-144">кустомернотес</span><span class="sxs-lookup"><span data-stu-id="80602-144">customerNotes</span></span>|<span data-ttu-id="80602-145">String</span><span class="sxs-lookup"><span data-stu-id="80602-145">String</span></span>|<span data-ttu-id="80602-146">Примечания от клиента, связанного с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="80602-146">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="80602-147">Значение можно получить только при чтении этого **букингаппоинтмент** по его идентификатору.</span><span class="sxs-lookup"><span data-stu-id="80602-147">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="80602-148">Это свойство можно задать только при первоначальном создании встречи с новым клиентом.</span><span class="sxs-lookup"><span data-stu-id="80602-148">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="80602-149">После этой точки значение вычисляется от клиента, представленного **customerId**.</span><span class="sxs-lookup"><span data-stu-id="80602-149">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="80602-150">кустомерфоне</span><span class="sxs-lookup"><span data-stu-id="80602-150">customerPhone</span></span>|<span data-ttu-id="80602-151">String</span><span class="sxs-lookup"><span data-stu-id="80602-151">String</span></span>|<span data-ttu-id="80602-152">Номер телефона клиента.</span><span class="sxs-lookup"><span data-stu-id="80602-152">The customer's phone number.</span></span>|
|<span data-ttu-id="80602-153">duration</span><span class="sxs-lookup"><span data-stu-id="80602-153">duration</span></span>|<span data-ttu-id="80602-154">Длительность</span><span class="sxs-lookup"><span data-stu-id="80602-154">Duration</span></span>|<span data-ttu-id="80602-155">Длительность встречи, обозначенная в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="80602-155">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="80602-156">end</span><span class="sxs-lookup"><span data-stu-id="80602-156">end</span></span>|[<span data-ttu-id="80602-157">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="80602-157">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="80602-158">Дата, время и часовой пояс, в котором заканчивается встреча.</span><span class="sxs-lookup"><span data-stu-id="80602-158">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="80602-159">инвоицеамаунт</span><span class="sxs-lookup"><span data-stu-id="80602-159">invoiceAmount</span></span>|<span data-ttu-id="80602-160">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="80602-160">Double</span></span>|<span data-ttu-id="80602-161">Сумма счета в счете.</span><span class="sxs-lookup"><span data-stu-id="80602-161">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="80602-162">инвоицедате</span><span class="sxs-lookup"><span data-stu-id="80602-162">invoiceDate</span></span>|[<span data-ttu-id="80602-163">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="80602-163">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="80602-164">Дата, время и часовой пояс накладной для данной встречи.</span><span class="sxs-lookup"><span data-stu-id="80602-164">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="80602-165">инвоицеид</span><span class="sxs-lookup"><span data-stu-id="80602-165">invoiceId</span></span>|<span data-ttu-id="80602-166">String</span><span class="sxs-lookup"><span data-stu-id="80602-166">String</span></span>|<span data-ttu-id="80602-167">Идентификатор счета.</span><span class="sxs-lookup"><span data-stu-id="80602-167">The ID of the invoice.</span></span>|
|<span data-ttu-id="80602-168">инвоицестатус</span><span class="sxs-lookup"><span data-stu-id="80602-168">invoiceStatus</span></span>|<span data-ttu-id="80602-169">string</span><span class="sxs-lookup"><span data-stu-id="80602-169">string</span></span>| <span data-ttu-id="80602-170">Статус счета.</span><span class="sxs-lookup"><span data-stu-id="80602-170">The status of the invoice.</span></span> <span data-ttu-id="80602-171">Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span><span class="sxs-lookup"><span data-stu-id="80602-171">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="80602-172">инвоицеурл</span><span class="sxs-lookup"><span data-stu-id="80602-172">invoiceUrl</span></span>|<span data-ttu-id="80602-173">String</span><span class="sxs-lookup"><span data-stu-id="80602-173">String</span></span>|<span data-ttu-id="80602-174">URL-адрес счета в книгах корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="80602-174">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="80602-175">оптаутофкустомеремаил</span><span class="sxs-lookup"><span data-stu-id="80602-175">optOutOfCustomerEmail</span></span>|<span data-ttu-id="80602-176">Логическое</span><span class="sxs-lookup"><span data-stu-id="80602-176">Boolean</span></span>|<span data-ttu-id="80602-177">Значение true указывает, что [букингкустомер](../resources/bookingcustomer.md) для этой встречи не хочет получать подтверждение для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="80602-177">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="80602-178">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="80602-178">postBuffer</span></span>|<span data-ttu-id="80602-179">Длительность</span><span class="sxs-lookup"><span data-stu-id="80602-179">Duration</span></span>|<span data-ttu-id="80602-180">Количество времени, которое необходимо зарезервировать после окончания встречи, для очистки в качестве примера.</span><span class="sxs-lookup"><span data-stu-id="80602-180">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="80602-181">Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="80602-181">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="80602-182">пребуфер</span><span class="sxs-lookup"><span data-stu-id="80602-182">preBuffer</span></span>|<span data-ttu-id="80602-183">Длительность</span><span class="sxs-lookup"><span data-stu-id="80602-183">Duration</span></span>|<span data-ttu-id="80602-184">Количество времени, которое необходимо зарезервировать до начала встречи, в качестве примера для подготовки.</span><span class="sxs-lookup"><span data-stu-id="80602-184">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="80602-185">Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="80602-185">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="80602-186">Цена</span><span class="sxs-lookup"><span data-stu-id="80602-186">price</span></span>|<span data-ttu-id="80602-187">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="80602-187">Double</span></span>|<span data-ttu-id="80602-188">Обычная цена для встречи с указанным [букингсервице](../resources/bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="80602-188">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="80602-189">прицетипе</span><span class="sxs-lookup"><span data-stu-id="80602-189">priceType</span></span>|<span data-ttu-id="80602-190">string</span><span class="sxs-lookup"><span data-stu-id="80602-190">string</span></span>| <span data-ttu-id="80602-191">Параметр, обеспечивающий гибкость для структуры ценообразования служб.</span><span class="sxs-lookup"><span data-stu-id="80602-191">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="80602-192">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="80602-192">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="80602-193">напоминания</span><span class="sxs-lookup"><span data-stu-id="80602-193">reminders</span></span>|<span data-ttu-id="80602-194">Коллекция [букингреминдер](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="80602-194">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="80602-195">Коллекция напоминаний о клиентах, отправленных для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="80602-195">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="80602-196">Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="80602-196">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="80602-197">селфсервицеаппоинтментид</span><span class="sxs-lookup"><span data-stu-id="80602-197">selfServiceAppointmentId</span></span>|<span data-ttu-id="80602-198">String</span><span class="sxs-lookup"><span data-stu-id="80602-198">String</span></span>|<span data-ttu-id="80602-199">Дополнительный идентификатор отслеживания для встречи, если встреча создана непосредственно клиентом на странице планирования, в отличие от сотрудника от имени клиента;.</span><span class="sxs-lookup"><span data-stu-id="80602-199">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="80602-200">serviceId</span><span class="sxs-lookup"><span data-stu-id="80602-200">serviceId</span></span>|<span data-ttu-id="80602-201">String</span><span class="sxs-lookup"><span data-stu-id="80602-201">String</span></span>|<span data-ttu-id="80602-202">Идентификатор [букингсервице](../resources/bookingservice.md) , связанный с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="80602-202">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="80602-203">сервицелокатион</span><span class="sxs-lookup"><span data-stu-id="80602-203">serviceLocation</span></span>|[<span data-ttu-id="80602-204">location</span><span class="sxs-lookup"><span data-stu-id="80602-204">location</span></span>](../resources/location.md)|<span data-ttu-id="80602-205">Место доставки службы.</span><span class="sxs-lookup"><span data-stu-id="80602-205">The location where the service is delivered.</span></span>|
|<span data-ttu-id="80602-206">Служба</span><span class="sxs-lookup"><span data-stu-id="80602-206">serviceName</span></span>|<span data-ttu-id="80602-207">String</span><span class="sxs-lookup"><span data-stu-id="80602-207">String</span></span>|<span data-ttu-id="80602-208">Имя **букингсервице** , связанного с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="80602-208">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="80602-209">Это свойство является необязательным при создании новой встречи.</span><span class="sxs-lookup"><span data-stu-id="80602-209">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="80602-210">Если он не указан, то он вычисляется из службы, связанной с встречей, с помощью свойства **serviceId** .</span><span class="sxs-lookup"><span data-stu-id="80602-210">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="80602-211">сервиценотес</span><span class="sxs-lookup"><span data-stu-id="80602-211">serviceNotes</span></span>|<span data-ttu-id="80602-212">String</span><span class="sxs-lookup"><span data-stu-id="80602-212">String</span></span>|<span data-ttu-id="80602-213">Заметки из [букингстаффмембер](../resources/bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="80602-213">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="80602-214">Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="80602-214">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="80602-215">стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="80602-215">staffMemberIds</span></span>|<span data-ttu-id="80602-216">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="80602-216">String collection</span></span>|<span data-ttu-id="80602-217">Идентификатор каждого [букингстаффмембер](../resources/bookingstaffmember.md) , запланированного в этой встрече.</span><span class="sxs-lookup"><span data-stu-id="80602-217">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="80602-218">начать</span><span class="sxs-lookup"><span data-stu-id="80602-218">start</span></span>|[<span data-ttu-id="80602-219">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="80602-219">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="80602-220">Дата, время и часовой пояс, с которого начинается встреча.</span><span class="sxs-lookup"><span data-stu-id="80602-220">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="80602-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="80602-221">Response</span></span>
<span data-ttu-id="80602-p113">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="80602-p113">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="80602-224">Пример</span><span class="sxs-lookup"><span data-stu-id="80602-224">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80602-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="80602-225">Request</span></span>
<span data-ttu-id="80602-226">В следующем примере дата обслуживания изменяется на день, а также обновляется и Дата выставления счета.</span><span class="sxs-lookup"><span data-stu-id="80602-226">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>

# <a name="http"></a>[<span data-ttu-id="80602-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="80602-227">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="80602-228">C#</span><span class="sxs-lookup"><span data-stu-id="80602-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80602-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80602-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80602-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80602-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="80602-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="80602-231">Response</span></span>
<span data-ttu-id="80602-232">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="80602-232">The following is an example of the response.</span></span>
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
