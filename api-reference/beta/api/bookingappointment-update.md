---
title: Обновление букингаппоинтмент
description: Обновление свойств объекта Букингаппоинтмент в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 8ab344d0f1336e3013fd44f97806e1c96958f322
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415647"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="36fc3-103">Обновление букингаппоинтмент</span><span class="sxs-lookup"><span data-stu-id="36fc3-103">Update bookingappointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36fc3-104">Обновление свойств объекта [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="36fc3-104">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="36fc3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36fc3-105">Permissions</span></span>
<span data-ttu-id="36fc3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36fc3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36fc3-108">Permission type</span></span>      | <span data-ttu-id="36fc3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36fc3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36fc3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36fc3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="36fc3-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="36fc3-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="36fc3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36fc3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36fc3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36fc3-113">Not supported.</span></span>   |
|<span data-ttu-id="36fc3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36fc3-114">Application</span></span> | <span data-ttu-id="36fc3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36fc3-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="36fc3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36fc3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="36fc3-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36fc3-117">Optional request headers</span></span>
| <span data-ttu-id="36fc3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="36fc3-118">Name</span></span>       | <span data-ttu-id="36fc3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="36fc3-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="36fc3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36fc3-120">Authorization</span></span>  | <span data-ttu-id="36fc3-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="36fc3-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="36fc3-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36fc3-122">Request body</span></span>
<span data-ttu-id="36fc3-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="36fc3-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="36fc3-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="36fc3-126">Property</span></span>     | <span data-ttu-id="36fc3-127">Тип</span><span class="sxs-lookup"><span data-stu-id="36fc3-127">Type</span></span>   |<span data-ttu-id="36fc3-128">Описание</span><span class="sxs-lookup"><span data-stu-id="36fc3-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36fc3-129">кустомеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="36fc3-129">customerEmailAddress</span></span>|<span data-ttu-id="36fc3-130">String</span><span class="sxs-lookup"><span data-stu-id="36fc3-130">String</span></span>|<span data-ttu-id="36fc3-131">SMTP-адрес [букингкустомер](../resources/bookingcustomer.md) , который зарезервировано встречу.</span><span class="sxs-lookup"><span data-stu-id="36fc3-131">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="36fc3-132">customerId</span><span class="sxs-lookup"><span data-stu-id="36fc3-132">customerId</span></span>|<span data-ttu-id="36fc3-133">String</span><span class="sxs-lookup"><span data-stu-id="36fc3-133">String</span></span>|<span data-ttu-id="36fc3-134">Идентификатор [букингкустомер](../resources/bookingcustomer.md) для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="36fc3-134">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="36fc3-135">Если при создании встречи не указан идентификатор, создается новый объект **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="36fc3-135">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="36fc3-136">После установки необходимо учесть неизменность **customerId** .</span><span class="sxs-lookup"><span data-stu-id="36fc3-136">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="36fc3-137">кустомерлокатион</span><span class="sxs-lookup"><span data-stu-id="36fc3-137">customerLocation</span></span>|[<span data-ttu-id="36fc3-138">location</span><span class="sxs-lookup"><span data-stu-id="36fc3-138">location</span></span>](../resources/location.md)|<span data-ttu-id="36fc3-139">Представляет сведения о расположении для [букингкустомер](../resources/bookingcustomer.md) , который зарезервировано встречу.</span><span class="sxs-lookup"><span data-stu-id="36fc3-139">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="36fc3-140">customerName</span><span class="sxs-lookup"><span data-stu-id="36fc3-140">customerName</span></span>|<span data-ttu-id="36fc3-141">String</span><span class="sxs-lookup"><span data-stu-id="36fc3-141">String</span></span>|<span data-ttu-id="36fc3-142">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="36fc3-142">The customer's name.</span></span>|
|<span data-ttu-id="36fc3-143">кустомернотес</span><span class="sxs-lookup"><span data-stu-id="36fc3-143">customerNotes</span></span>|<span data-ttu-id="36fc3-144">String</span><span class="sxs-lookup"><span data-stu-id="36fc3-144">String</span></span>|<span data-ttu-id="36fc3-145">Примечания от клиента, связанного с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="36fc3-145">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="36fc3-146">Значение можно получить только при чтении этого **букингаппоинтмент** по его идентификатору.</span><span class="sxs-lookup"><span data-stu-id="36fc3-146">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="36fc3-147">Это свойство можно задать только при первоначальном создании встречи с новым клиентом.</span><span class="sxs-lookup"><span data-stu-id="36fc3-147">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="36fc3-148">После этой точки значение вычисляется от клиента, представленного **customerId**.</span><span class="sxs-lookup"><span data-stu-id="36fc3-148">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="36fc3-149">кустомерфоне</span><span class="sxs-lookup"><span data-stu-id="36fc3-149">customerPhone</span></span>|<span data-ttu-id="36fc3-150">String</span><span class="sxs-lookup"><span data-stu-id="36fc3-150">String</span></span>|<span data-ttu-id="36fc3-151">Номер телефона клиента.</span><span class="sxs-lookup"><span data-stu-id="36fc3-151">The customer's phone number.</span></span>|
|<span data-ttu-id="36fc3-152">duration</span><span class="sxs-lookup"><span data-stu-id="36fc3-152">duration</span></span>|<span data-ttu-id="36fc3-153">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="36fc3-153">Duration</span></span>|<span data-ttu-id="36fc3-154">Длительность встречи, обозначенная в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="36fc3-154">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="36fc3-155">end</span><span class="sxs-lookup"><span data-stu-id="36fc3-155">end</span></span>|[<span data-ttu-id="36fc3-156">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="36fc3-156">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="36fc3-157">Дата, время и часовой пояс, в котором заканчивается встреча.</span><span class="sxs-lookup"><span data-stu-id="36fc3-157">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="36fc3-158">инвоицеамаунт</span><span class="sxs-lookup"><span data-stu-id="36fc3-158">invoiceAmount</span></span>|<span data-ttu-id="36fc3-159">Двойное</span><span class="sxs-lookup"><span data-stu-id="36fc3-159">Double</span></span>|<span data-ttu-id="36fc3-160">Сумма счета в счете.</span><span class="sxs-lookup"><span data-stu-id="36fc3-160">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="36fc3-161">инвоицедате</span><span class="sxs-lookup"><span data-stu-id="36fc3-161">invoiceDate</span></span>|[<span data-ttu-id="36fc3-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="36fc3-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="36fc3-163">Дата, время и часовой пояс накладной для данной встречи.</span><span class="sxs-lookup"><span data-stu-id="36fc3-163">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="36fc3-164">инвоицеид</span><span class="sxs-lookup"><span data-stu-id="36fc3-164">invoiceId</span></span>|<span data-ttu-id="36fc3-165">String</span><span class="sxs-lookup"><span data-stu-id="36fc3-165">String</span></span>|<span data-ttu-id="36fc3-166">Идентификатор счета.</span><span class="sxs-lookup"><span data-stu-id="36fc3-166">The ID of the invoice.</span></span>|
|<span data-ttu-id="36fc3-167">инвоицестатус</span><span class="sxs-lookup"><span data-stu-id="36fc3-167">invoiceStatus</span></span>|<span data-ttu-id="36fc3-168">string</span><span class="sxs-lookup"><span data-stu-id="36fc3-168">string</span></span>| <span data-ttu-id="36fc3-169">Статус счета.</span><span class="sxs-lookup"><span data-stu-id="36fc3-169">The status of the invoice.</span></span> <span data-ttu-id="36fc3-170">Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span><span class="sxs-lookup"><span data-stu-id="36fc3-170">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="36fc3-171">инвоицеурл</span><span class="sxs-lookup"><span data-stu-id="36fc3-171">invoiceUrl</span></span>|<span data-ttu-id="36fc3-172">String</span><span class="sxs-lookup"><span data-stu-id="36fc3-172">String</span></span>|<span data-ttu-id="36fc3-173">URL-адрес счета в книгах корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="36fc3-173">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="36fc3-174">оптаутофкустомеремаил</span><span class="sxs-lookup"><span data-stu-id="36fc3-174">optOutOfCustomerEmail</span></span>|<span data-ttu-id="36fc3-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="36fc3-175">Boolean</span></span>|<span data-ttu-id="36fc3-176">Значение true указывает, что [букингкустомер](../resources/bookingcustomer.md) для этой встречи не хочет получать подтверждение для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="36fc3-176">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="36fc3-177">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="36fc3-177">postBuffer</span></span>|<span data-ttu-id="36fc3-178">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="36fc3-178">Duration</span></span>|<span data-ttu-id="36fc3-179">Количество времени, которое необходимо зарезервировать после окончания встречи, для очистки в качестве примера.</span><span class="sxs-lookup"><span data-stu-id="36fc3-179">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="36fc3-180">Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="36fc3-180">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="36fc3-181">пребуфер</span><span class="sxs-lookup"><span data-stu-id="36fc3-181">preBuffer</span></span>|<span data-ttu-id="36fc3-182">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="36fc3-182">Duration</span></span>|<span data-ttu-id="36fc3-183">Количество времени, которое необходимо зарезервировать до начала встречи, в качестве примера для подготовки.</span><span class="sxs-lookup"><span data-stu-id="36fc3-183">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="36fc3-184">Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="36fc3-184">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="36fc3-185">Цена</span><span class="sxs-lookup"><span data-stu-id="36fc3-185">price</span></span>|<span data-ttu-id="36fc3-186">Двойное</span><span class="sxs-lookup"><span data-stu-id="36fc3-186">Double</span></span>|<span data-ttu-id="36fc3-187">Обычная цена для встречи с указанным [букингсервице](../resources/bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="36fc3-187">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="36fc3-188">прицетипе</span><span class="sxs-lookup"><span data-stu-id="36fc3-188">priceType</span></span>|<span data-ttu-id="36fc3-189">string</span><span class="sxs-lookup"><span data-stu-id="36fc3-189">string</span></span>| <span data-ttu-id="36fc3-190">Параметр, обеспечивающий гибкость для структуры ценообразования служб.</span><span class="sxs-lookup"><span data-stu-id="36fc3-190">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="36fc3-191">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="36fc3-191">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="36fc3-192">напоминания</span><span class="sxs-lookup"><span data-stu-id="36fc3-192">reminders</span></span>|<span data-ttu-id="36fc3-193">Коллекция [букингреминдер](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="36fc3-193">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="36fc3-194">Коллекция напоминаний о клиентах, отправленных для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="36fc3-194">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="36fc3-195">Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="36fc3-195">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="36fc3-196">селфсервицеаппоинтментид</span><span class="sxs-lookup"><span data-stu-id="36fc3-196">selfServiceAppointmentId</span></span>|<span data-ttu-id="36fc3-197">String</span><span class="sxs-lookup"><span data-stu-id="36fc3-197">String</span></span>|<span data-ttu-id="36fc3-198">Дополнительный идентификатор отслеживания для встречи, если встреча создана непосредственно клиентом на странице планирования, в отличие от сотрудника от имени клиента;.</span><span class="sxs-lookup"><span data-stu-id="36fc3-198">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="36fc3-199">serviceId</span><span class="sxs-lookup"><span data-stu-id="36fc3-199">serviceId</span></span>|<span data-ttu-id="36fc3-200">String</span><span class="sxs-lookup"><span data-stu-id="36fc3-200">String</span></span>|<span data-ttu-id="36fc3-201">Идентификатор [букингсервице](../resources/bookingservice.md) , связанный с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="36fc3-201">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="36fc3-202">сервицелокатион</span><span class="sxs-lookup"><span data-stu-id="36fc3-202">serviceLocation</span></span>|[<span data-ttu-id="36fc3-203">location</span><span class="sxs-lookup"><span data-stu-id="36fc3-203">location</span></span>](../resources/location.md)|<span data-ttu-id="36fc3-204">Место доставки службы.</span><span class="sxs-lookup"><span data-stu-id="36fc3-204">The location where the service is delivered.</span></span>|
|<span data-ttu-id="36fc3-205">Служба</span><span class="sxs-lookup"><span data-stu-id="36fc3-205">serviceName</span></span>|<span data-ttu-id="36fc3-206">String</span><span class="sxs-lookup"><span data-stu-id="36fc3-206">String</span></span>|<span data-ttu-id="36fc3-207">Имя **букингсервице** , связанного с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="36fc3-207">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="36fc3-208">Это свойство является необязательным при создании новой встречи.</span><span class="sxs-lookup"><span data-stu-id="36fc3-208">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="36fc3-209">Если он не указан, то он вычисляется из службы, связанной с встречей, с помощью свойства **serviceId** .</span><span class="sxs-lookup"><span data-stu-id="36fc3-209">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="36fc3-210">сервиценотес</span><span class="sxs-lookup"><span data-stu-id="36fc3-210">serviceNotes</span></span>|<span data-ttu-id="36fc3-211">String</span><span class="sxs-lookup"><span data-stu-id="36fc3-211">String</span></span>|<span data-ttu-id="36fc3-212">Заметки из [букингстаффмембер](../resources/bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="36fc3-212">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="36fc3-213">Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="36fc3-213">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="36fc3-214">стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="36fc3-214">staffMemberIds</span></span>|<span data-ttu-id="36fc3-215">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="36fc3-215">String collection</span></span>|<span data-ttu-id="36fc3-216">Идентификатор каждого [букингстаффмембер](../resources/bookingstaffmember.md) , запланированного в этой встрече.</span><span class="sxs-lookup"><span data-stu-id="36fc3-216">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="36fc3-217">начать</span><span class="sxs-lookup"><span data-stu-id="36fc3-217">start</span></span>|[<span data-ttu-id="36fc3-218">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="36fc3-218">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="36fc3-219">Дата, время и часовой пояс, с которого начинается встреча.</span><span class="sxs-lookup"><span data-stu-id="36fc3-219">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="36fc3-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="36fc3-220">Response</span></span>
<span data-ttu-id="36fc3-p113">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="36fc3-p113">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36fc3-223">Пример</span><span class="sxs-lookup"><span data-stu-id="36fc3-223">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36fc3-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="36fc3-224">Request</span></span>
<span data-ttu-id="36fc3-225">В следующем примере дата обслуживания изменяется на день, а также обновляется и Дата выставления счета.</span><span class="sxs-lookup"><span data-stu-id="36fc3-225">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36fc3-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="36fc3-226">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="36fc3-227">C#</span><span class="sxs-lookup"><span data-stu-id="36fc3-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36fc3-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36fc3-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36fc3-229">Цель — C</span><span class="sxs-lookup"><span data-stu-id="36fc3-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="36fc3-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="36fc3-230">Response</span></span>
<span data-ttu-id="36fc3-231">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="36fc3-231">The following is an example of the response.</span></span>
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
