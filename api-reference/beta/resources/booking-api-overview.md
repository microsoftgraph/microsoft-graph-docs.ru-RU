---
title: Использование Microsoft резервирования API в Microsoft Graph
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 5e553e2814c6e5554ea7bb2f4daef8c62057aff3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079426"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="80ccc-104">Использование Microsoft резервирования API в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="80ccc-104">Use the Microsoft Bookings API in Microsoft Graph</span></span>

 > <span data-ttu-id="80ccc-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="80ccc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80ccc-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80ccc-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="80ccc-107">Microsoft резервирования позволяет управлять резервирования клиента и данных с помощью минимальной установки владельцев для малого бизнеса.</span><span class="sxs-lookup"><span data-stu-id="80ccc-107">Microsoft Bookings lets small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="80ccc-108">Владелец business можно создать один или несколько организаций, с каждой бизнеса, предоставляющая набор служб.</span><span class="sxs-lookup"><span data-stu-id="80ccc-108">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="80ccc-109">Владелец можно настроить персонал и укажите службы, которые выполняет каждый сотрудник.</span><span class="sxs-lookup"><span data-stu-id="80ccc-109">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="80ccc-110">В этой организации в приложении online или мобильного клиента можно книги встречи для определенной службы.</span><span class="sxs-lookup"><span data-stu-id="80ccc-110">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="80ccc-111">Резервирования гарантирует, что, время встречи актуальность для бизнеса, сотрудниками и клиентами участвующие.</span><span class="sxs-lookup"><span data-stu-id="80ccc-111">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="80ccc-112">Программным способом, [bookingBusiness](bookingbusiness.md) в интерфейсе API резервирования состоит из следующих объектов:</span><span class="sxs-lookup"><span data-stu-id="80ccc-112">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="80ccc-113">Один или несколько объектов [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="80ccc-113">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="80ccc-114">Один или несколько объектов [bookingService](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="80ccc-114">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="80ccc-115">Набор экземпляров [bookingAppointment](bookingappointment.md)</span><span class="sxs-lookup"><span data-stu-id="80ccc-115">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="80ccc-116">Набор объектов [bookingCustomer](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="80ccc-116">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="80ccc-117">С помощью API-Интерфейс REST резервирования</span><span class="sxs-lookup"><span data-stu-id="80ccc-117">Using the Bookings REST API</span></span>

<span data-ttu-id="80ccc-118">Познакомьтесь с помощью следующих действий перед резервирования встречи для бизнеса в первый раз.</span><span class="sxs-lookup"><span data-stu-id="80ccc-118">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="80ccc-119">Убедитесь, что соответствующие [маркеры доступа](/graph/auth-overview) обеспечения соответствующие операции.</span><span class="sxs-lookup"><span data-stu-id="80ccc-119">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="80ccc-120">Убедитесь в том, что подписка на [Office 365 бизнеса расширенный](https://products.office.com/en-us/business/office-365-business-premium) для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="80ccc-120">Make sure the business has an [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="80ccc-121">Создание нового **bookingBusiness** , отправив операция POST набора сущностей.</span><span class="sxs-lookup"><span data-stu-id="80ccc-121">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="80ccc-122">Как минимум необходимо указать имя для нового предприятия, которое клиенты будут видеть:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="80ccc-122">At minimum, you should specify a name for the new business that customers will see: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="80ccc-123">Свойство **id** нового **bookingBusiness** , возвращаемого в ответе POST для продолжения [Настройка](../api/bookingbusiness-update.md) параметров business и добавьте персонал и службы для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="80ccc-123">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="80ccc-124">Добавление отдельных сотрудников для бизнеса:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="80ccc-124">Add individual staff members for the business: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. <span data-ttu-id="80ccc-125">Определение каждой службы, предлагаемыми бизнеса:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="80ccc-125">Define each service offered by the business: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="80ccc-126">Опубликуйте страницу планирования для бизнеса, чтобы позволить клиентам и операторы business начать назначения встреч:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="80ccc-126">Publish the scheduling page for the business, to let customers and business operators start booking appointments: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="80ccc-127">Как правило чтобы получить список всех резервирование бизнеса в Office 365 клиентов:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="80ccc-127">In general, to list all the booking businesses in the Office 365 tenant: <!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="80ccc-128">Основные сценарии выполнения</span><span class="sxs-lookup"><span data-stu-id="80ccc-128">Common use cases</span></span> 

<span data-ttu-id="80ccc-129">В следующей таблице перечислены типичные операции для бизнеса в API резервирования.</span><span class="sxs-lookup"><span data-stu-id="80ccc-129">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="80ccc-130">Варианты использования</span><span class="sxs-lookup"><span data-stu-id="80ccc-130">Use cases</span></span>        | <span data-ttu-id="80ccc-131">Ресурсы REST</span><span class="sxs-lookup"><span data-stu-id="80ccc-131">REST resources</span></span> | <span data-ttu-id="80ccc-132">См. также</span><span class="sxs-lookup"><span data-stu-id="80ccc-132">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="80ccc-133">Создание, получение, обновление и удаление предприятие</span><span class="sxs-lookup"><span data-stu-id="80ccc-133">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="80ccc-134">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="80ccc-134">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="80ccc-135">Методы bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="80ccc-135">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="80ccc-136">Обновление политики планирования</span><span class="sxs-lookup"><span data-stu-id="80ccc-136">Update the scheduling policy</span></span> | [<span data-ttu-id="80ccc-137">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="80ccc-137">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="80ccc-138">Обновление bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="80ccc-138">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="80ccc-139">Добавление, получение, обновление и удаление сотрудников</span><span class="sxs-lookup"><span data-stu-id="80ccc-139">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="80ccc-140">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="80ccc-140">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="80ccc-141">Методы bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="80ccc-141">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="80ccc-142">Добавление, получение, обновление и удаление служб</span><span class="sxs-lookup"><span data-stu-id="80ccc-142">Add, get, update, or delete services</span></span> | [<span data-ttu-id="80ccc-143">bookingService</span><span class="sxs-lookup"><span data-stu-id="80ccc-143">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="80ccc-144">Методы bookingService</span><span class="sxs-lookup"><span data-stu-id="80ccc-144">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="80ccc-145">Публикации или отмены публикации планирования страницы</span><span class="sxs-lookup"><span data-stu-id="80ccc-145">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="80ccc-146">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="80ccc-146">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="80ccc-147">Публикация</span><span class="sxs-lookup"><span data-stu-id="80ccc-147">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="80ccc-148">Отмена публикации</span><span class="sxs-lookup"><span data-stu-id="80ccc-148">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="80ccc-149">Создание, получение, обновление, удаление или Отмена встречи</span><span class="sxs-lookup"><span data-stu-id="80ccc-149">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="80ccc-150">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="80ccc-150">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="80ccc-151">Методы bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="80ccc-151">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="80ccc-152">Получение встреч в диапазон дат</span><span class="sxs-lookup"><span data-stu-id="80ccc-152">Get appointments in a date range</span></span> | [<span data-ttu-id="80ccc-153">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="80ccc-153">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="80ccc-154">Список резервирования представления календаря</span><span class="sxs-lookup"><span data-stu-id="80ccc-154">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="80ccc-155">Получение валюты</span><span class="sxs-lookup"><span data-stu-id="80ccc-155">Get currency</span></span> | [<span data-ttu-id="80ccc-156">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="80ccc-156">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="80ccc-157">Методы bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="80ccc-157">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |


## <a name="see-also"></a><span data-ttu-id="80ccc-158">См. также</span><span class="sxs-lookup"><span data-stu-id="80ccc-158">See also</span></span>

- <span data-ttu-id="80ccc-159">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="80ccc-159">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="80ccc-160">В разделе [как партнеров используется Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span><span class="sxs-lookup"><span data-stu-id="80ccc-160">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
- <span data-ttu-id="80ccc-161">Узнайте, как выбрать [разрешения](/graph/permissions-reference) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="80ccc-161">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>