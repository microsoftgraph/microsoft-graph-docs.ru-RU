---
title: Обновление букингаппоинтмент
description: Обновление свойств объекта Букингаппоинтмент в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 2c6660ca580423483cd9bc3b200f1176e92544df
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258270"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="5d9de-103">Обновление букингаппоинтмент</span><span class="sxs-lookup"><span data-stu-id="5d9de-103">Update bookingappointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d9de-104">Обновление свойств объекта [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="5d9de-104">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5d9de-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d9de-105">Permissions</span></span>
<span data-ttu-id="5d9de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d9de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d9de-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d9de-108">Permission type</span></span>      | <span data-ttu-id="5d9de-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d9de-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d9de-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d9de-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5d9de-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="5d9de-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5d9de-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d9de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d9de-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d9de-113">Not supported.</span></span>   |
|<span data-ttu-id="5d9de-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d9de-114">Application</span></span> | <span data-ttu-id="5d9de-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d9de-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5d9de-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d9de-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="5d9de-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d9de-117">Optional request headers</span></span>
| <span data-ttu-id="5d9de-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5d9de-118">Name</span></span>       | <span data-ttu-id="5d9de-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5d9de-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5d9de-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d9de-120">Authorization</span></span>  | <span data-ttu-id="5d9de-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5d9de-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d9de-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d9de-122">Request body</span></span>
<span data-ttu-id="5d9de-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5d9de-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5d9de-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d9de-126">Property</span></span>     | <span data-ttu-id="5d9de-127">Тип</span><span class="sxs-lookup"><span data-stu-id="5d9de-127">Type</span></span>   |<span data-ttu-id="5d9de-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5d9de-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d9de-129">Кустомеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="5d9de-129">customerEmailAddress</span></span>|<span data-ttu-id="5d9de-130">String</span><span class="sxs-lookup"><span data-stu-id="5d9de-130">String</span></span>|<span data-ttu-id="5d9de-131">SMTP-адрес [букингкустомер](../resources/bookingcustomer.md) , который зарезервировано встречу.</span><span class="sxs-lookup"><span data-stu-id="5d9de-131">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="5d9de-132">customerId</span><span class="sxs-lookup"><span data-stu-id="5d9de-132">customerId</span></span>|<span data-ttu-id="5d9de-133">String</span><span class="sxs-lookup"><span data-stu-id="5d9de-133">String</span></span>|<span data-ttu-id="5d9de-134">Идентификатор [букингкустомер](../resources/bookingcustomer.md) для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="5d9de-134">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="5d9de-135">Если при создании встречи не указан идентификатор, создается новый объект **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="5d9de-135">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="5d9de-136">После установки необходимо учесть неизменность **customerId** .</span><span class="sxs-lookup"><span data-stu-id="5d9de-136">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="5d9de-137">Кустомерлокатион</span><span class="sxs-lookup"><span data-stu-id="5d9de-137">customerLocation</span></span>|[<span data-ttu-id="5d9de-138">location</span><span class="sxs-lookup"><span data-stu-id="5d9de-138">location</span></span>](../resources/location.md)|<span data-ttu-id="5d9de-139">Представляет сведения о расположении для [букингкустомер](../resources/bookingcustomer.md) , который зарезервировано встречу.</span><span class="sxs-lookup"><span data-stu-id="5d9de-139">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="5d9de-140">customerName</span><span class="sxs-lookup"><span data-stu-id="5d9de-140">customerName</span></span>|<span data-ttu-id="5d9de-141">String</span><span class="sxs-lookup"><span data-stu-id="5d9de-141">String</span></span>|<span data-ttu-id="5d9de-142">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="5d9de-142">The customer's name.</span></span>|
|<span data-ttu-id="5d9de-143">Кустомернотес</span><span class="sxs-lookup"><span data-stu-id="5d9de-143">customerNotes</span></span>|<span data-ttu-id="5d9de-144">String</span><span class="sxs-lookup"><span data-stu-id="5d9de-144">String</span></span>|<span data-ttu-id="5d9de-145">Примечания от клиента, связанного с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="5d9de-145">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="5d9de-146">Значение можно получить только при чтении этого **букингаппоинтмент** по его идентификатору.</span><span class="sxs-lookup"><span data-stu-id="5d9de-146">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="5d9de-147">Это свойство можно задать только при первоначальном создании встречи с новым клиентом.</span><span class="sxs-lookup"><span data-stu-id="5d9de-147">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="5d9de-148">После этой точки значение вычисляется от клиента, представленного **customerId**.</span><span class="sxs-lookup"><span data-stu-id="5d9de-148">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="5d9de-149">Кустомерфоне</span><span class="sxs-lookup"><span data-stu-id="5d9de-149">customerPhone</span></span>|<span data-ttu-id="5d9de-150">String</span><span class="sxs-lookup"><span data-stu-id="5d9de-150">String</span></span>|<span data-ttu-id="5d9de-151">Номер телефона клиента.</span><span class="sxs-lookup"><span data-stu-id="5d9de-151">The customer's phone number.</span></span>|
|<span data-ttu-id="5d9de-152">duration</span><span class="sxs-lookup"><span data-stu-id="5d9de-152">duration</span></span>|<span data-ttu-id="5d9de-153">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="5d9de-153">Duration</span></span>|<span data-ttu-id="5d9de-154">Длительность встречи, обозначенная в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="5d9de-154">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="5d9de-155">end</span><span class="sxs-lookup"><span data-stu-id="5d9de-155">end</span></span>|[<span data-ttu-id="5d9de-156">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5d9de-156">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="5d9de-157">Дата, время и часовой пояс, в котором заканчивается встреча.</span><span class="sxs-lookup"><span data-stu-id="5d9de-157">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="5d9de-158">Инвоицеамаунт</span><span class="sxs-lookup"><span data-stu-id="5d9de-158">invoiceAmount</span></span>|<span data-ttu-id="5d9de-159">Двойное</span><span class="sxs-lookup"><span data-stu-id="5d9de-159">Double</span></span>|<span data-ttu-id="5d9de-160">Сумма счета в счете.</span><span class="sxs-lookup"><span data-stu-id="5d9de-160">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="5d9de-161">Инвоицедате</span><span class="sxs-lookup"><span data-stu-id="5d9de-161">invoiceDate</span></span>|[<span data-ttu-id="5d9de-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5d9de-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="5d9de-163">Дата, время и часовой пояс накладной для данной встречи.</span><span class="sxs-lookup"><span data-stu-id="5d9de-163">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="5d9de-164">Инвоицеид</span><span class="sxs-lookup"><span data-stu-id="5d9de-164">invoiceId</span></span>|<span data-ttu-id="5d9de-165">String</span><span class="sxs-lookup"><span data-stu-id="5d9de-165">String</span></span>|<span data-ttu-id="5d9de-166">Идентификатор счета.</span><span class="sxs-lookup"><span data-stu-id="5d9de-166">The ID of the invoice.</span></span>|
|<span data-ttu-id="5d9de-167">Инвоицестатус</span><span class="sxs-lookup"><span data-stu-id="5d9de-167">invoiceStatus</span></span>|<span data-ttu-id="5d9de-168">string</span><span class="sxs-lookup"><span data-stu-id="5d9de-168">string</span></span>| <span data-ttu-id="5d9de-169">Статус счета.</span><span class="sxs-lookup"><span data-stu-id="5d9de-169">The status of the invoice.</span></span> <span data-ttu-id="5d9de-170">Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span><span class="sxs-lookup"><span data-stu-id="5d9de-170">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="5d9de-171">Инвоицеурл</span><span class="sxs-lookup"><span data-stu-id="5d9de-171">invoiceUrl</span></span>|<span data-ttu-id="5d9de-172">String</span><span class="sxs-lookup"><span data-stu-id="5d9de-172">String</span></span>|<span data-ttu-id="5d9de-173">URL-адрес счета в книгах корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5d9de-173">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="5d9de-174">Оптаутофкустомеремаил</span><span class="sxs-lookup"><span data-stu-id="5d9de-174">optOutOfCustomerEmail</span></span>|<span data-ttu-id="5d9de-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d9de-175">Boolean</span></span>|<span data-ttu-id="5d9de-176">Значение true указывает, что [букингкустомер](../resources/bookingcustomer.md) для этой встречи не хочет получать подтверждение для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="5d9de-176">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="5d9de-177">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="5d9de-177">postBuffer</span></span>|<span data-ttu-id="5d9de-178">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="5d9de-178">Duration</span></span>|<span data-ttu-id="5d9de-179">Количество времени, которое необходимо зарезервировать после окончания встречи, для очистки в качестве примера.</span><span class="sxs-lookup"><span data-stu-id="5d9de-179">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="5d9de-180">Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="5d9de-180">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="5d9de-181">пребуфер</span><span class="sxs-lookup"><span data-stu-id="5d9de-181">preBuffer</span></span>|<span data-ttu-id="5d9de-182">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="5d9de-182">Duration</span></span>|<span data-ttu-id="5d9de-183">Количество времени, которое необходимо зарезервировать до начала встречи, в качестве примера для подготовки.</span><span class="sxs-lookup"><span data-stu-id="5d9de-183">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="5d9de-184">Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="5d9de-184">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="5d9de-185">Цена</span><span class="sxs-lookup"><span data-stu-id="5d9de-185">price</span></span>|<span data-ttu-id="5d9de-186">Двойное</span><span class="sxs-lookup"><span data-stu-id="5d9de-186">Double</span></span>|<span data-ttu-id="5d9de-187">Обычная цена для встречи с указанным [букингсервице](../resources/bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="5d9de-187">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="5d9de-188">Прицетипе</span><span class="sxs-lookup"><span data-stu-id="5d9de-188">priceType</span></span>|<span data-ttu-id="5d9de-189">string</span><span class="sxs-lookup"><span data-stu-id="5d9de-189">string</span></span>| <span data-ttu-id="5d9de-190">Параметр, обеспечивающий гибкость для структуры ценообразования служб.</span><span class="sxs-lookup"><span data-stu-id="5d9de-190">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="5d9de-191">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5d9de-191">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="5d9de-192">напоминания</span><span class="sxs-lookup"><span data-stu-id="5d9de-192">reminders</span></span>|<span data-ttu-id="5d9de-193">Коллекция [букингреминдер](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="5d9de-193">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="5d9de-194">Коллекция напоминаний о клиентах, отправленных для этой встречи.</span><span class="sxs-lookup"><span data-stu-id="5d9de-194">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="5d9de-195">Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="5d9de-195">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="5d9de-196">Селфсервицеаппоинтментид</span><span class="sxs-lookup"><span data-stu-id="5d9de-196">selfServiceAppointmentId</span></span>|<span data-ttu-id="5d9de-197">String</span><span class="sxs-lookup"><span data-stu-id="5d9de-197">String</span></span>|<span data-ttu-id="5d9de-198">Дополнительный идентификатор отслеживания для встречи, если встреча создана непосредственно клиентом на странице планирования, в отличие от сотрудника от имени клиента;.</span><span class="sxs-lookup"><span data-stu-id="5d9de-198">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="5d9de-199">serviceId</span><span class="sxs-lookup"><span data-stu-id="5d9de-199">serviceId</span></span>|<span data-ttu-id="5d9de-200">String</span><span class="sxs-lookup"><span data-stu-id="5d9de-200">String</span></span>|<span data-ttu-id="5d9de-201">Идентификатор [букингсервице](../resources/bookingservice.md) , связанный с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="5d9de-201">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="5d9de-202">Сервицелокатион</span><span class="sxs-lookup"><span data-stu-id="5d9de-202">serviceLocation</span></span>|[<span data-ttu-id="5d9de-203">location</span><span class="sxs-lookup"><span data-stu-id="5d9de-203">location</span></span>](../resources/location.md)|<span data-ttu-id="5d9de-204">Место доставки службы.</span><span class="sxs-lookup"><span data-stu-id="5d9de-204">The location where the service is delivered.</span></span>|
|<span data-ttu-id="5d9de-205">Служба</span><span class="sxs-lookup"><span data-stu-id="5d9de-205">serviceName</span></span>|<span data-ttu-id="5d9de-206">String</span><span class="sxs-lookup"><span data-stu-id="5d9de-206">String</span></span>|<span data-ttu-id="5d9de-207">Имя **букингсервице** , связанного с этой встречей.</span><span class="sxs-lookup"><span data-stu-id="5d9de-207">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="5d9de-208">Это свойство является необязательным при создании новой встречи.</span><span class="sxs-lookup"><span data-stu-id="5d9de-208">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="5d9de-209">Если он не указан, то он вычисляется из службы, связанной с встречей, с помощью свойства **serviceId** .</span><span class="sxs-lookup"><span data-stu-id="5d9de-209">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="5d9de-210">Сервиценотес</span><span class="sxs-lookup"><span data-stu-id="5d9de-210">serviceNotes</span></span>|<span data-ttu-id="5d9de-211">String</span><span class="sxs-lookup"><span data-stu-id="5d9de-211">String</span></span>|<span data-ttu-id="5d9de-212">Заметки из [букингстаффмембер](../resources/bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="5d9de-212">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="5d9de-213">Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="5d9de-213">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="5d9de-214">Стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="5d9de-214">staffMemberIds</span></span>|<span data-ttu-id="5d9de-215">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5d9de-215">String collection</span></span>|<span data-ttu-id="5d9de-216">Идентификатор каждого [букингстаффмембер](../resources/bookingstaffmember.md) , запланированного в этой встрече.</span><span class="sxs-lookup"><span data-stu-id="5d9de-216">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="5d9de-217">начать</span><span class="sxs-lookup"><span data-stu-id="5d9de-217">start</span></span>|[<span data-ttu-id="5d9de-218">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5d9de-218">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="5d9de-219">Дата, время и часовой пояс, с которого начинается встреча.</span><span class="sxs-lookup"><span data-stu-id="5d9de-219">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="5d9de-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d9de-220">Response</span></span>
<span data-ttu-id="5d9de-p113">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5d9de-p113">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d9de-223">Пример</span><span class="sxs-lookup"><span data-stu-id="5d9de-223">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d9de-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d9de-224">Request</span></span>
<span data-ttu-id="5d9de-225">В следующем примере дата обслуживания изменяется на день, а также обновляется и Дата выставления счета.</span><span class="sxs-lookup"><span data-stu-id="5d9de-225">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5d9de-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d9de-226">Response</span></span>
<span data-ttu-id="5d9de-227">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5d9de-227">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5d9de-228">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5d9de-228">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5d9de-229">C#</span><span class="sxs-lookup"><span data-stu-id="5d9de-229">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_bookingappointment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d9de-230">Javascript</span><span class="sxs-lookup"><span data-stu-id="5d9de-230">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_bookingappointment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5d9de-231">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5d9de-231">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_bookingappointment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
