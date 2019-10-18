---
title: Использование API Microsoft Bookings в Microsoft Graph
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Priority
author: angelgolfer-ms
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: 171f75d35812176202263659185bd4dca94e06de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974201"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="f8c74-104">Использование API Microsoft Bookings в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f8c74-104">Use the Microsoft Bookings API in Microsoft Graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="f8c74-105">Microsoft Bookings позволяет владельцам малого бизнеса управлять резервированиями и сведениями клиентов с минимальной настройкой.</span><span class="sxs-lookup"><span data-stu-id="f8c74-105">Microsoft Bookings lets small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="f8c74-106">Владелец бизнеса можно создать одну или несколько компаний, каждая из которых предлагает набор услуг.</span><span class="sxs-lookup"><span data-stu-id="f8c74-106">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="f8c74-107">Владелец может настроить сотрудников и указать услуги, оказываемые каждым из них.</span><span class="sxs-lookup"><span data-stu-id="f8c74-107">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="f8c74-108">Клиент может зарезервировать встречу для определенной услуги в этой компании в сетевом или мобильном приложении.</span><span class="sxs-lookup"><span data-stu-id="f8c74-108">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="f8c74-109">Приложение Bookings обеспечивает обновление времени встречи для компании, сотрудников и соответствующих клиентов.</span><span class="sxs-lookup"><span data-stu-id="f8c74-109">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="f8c74-110">На программном уровне объект [bookingBusiness](bookingbusiness.md) в API Bookings включает указанные ниже объекты:</span><span class="sxs-lookup"><span data-stu-id="f8c74-110">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="f8c74-111">один или несколько объектов [bookingStaffMember](bookingstaffmember.md);</span><span class="sxs-lookup"><span data-stu-id="f8c74-111">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="f8c74-112">один или несколько объектов [bookingService](bookingservice.md);</span><span class="sxs-lookup"><span data-stu-id="f8c74-112">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="f8c74-113">набор экземпляров [bookingAppointment](bookingappointment.md);</span><span class="sxs-lookup"><span data-stu-id="f8c74-113">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="f8c74-114">набор объектов [bookingCustomer](bookingcustomer.md).</span><span class="sxs-lookup"><span data-stu-id="f8c74-114">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="f8c74-115">Использование REST API Bookings</span><span class="sxs-lookup"><span data-stu-id="f8c74-115">Using the Bookings REST API</span></span>

<span data-ttu-id="f8c74-116">Выполните указанные ниже действия перед первым резервированием встреч клиента с компанией.</span><span class="sxs-lookup"><span data-stu-id="f8c74-116">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="f8c74-117">Убедитесь, что предоставлены подходящие [маркеры доступа](/graph/auth-overview) для соответствующих операций.</span><span class="sxs-lookup"><span data-stu-id="f8c74-117">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="f8c74-118">Убедитесь, что у компании есть подписка на [Office 365 бизнес премиум](https://products.office.com/en-us/business/office-365-business-premium).</span><span class="sxs-lookup"><span data-stu-id="f8c74-118">Make sure the business has an [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="f8c74-119">Создайте новый объект **bookingBusiness**, отправив операцию POST в набор объектов.</span><span class="sxs-lookup"><span data-stu-id="f8c74-119">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="f8c74-120">Как минимум, следует указать имя новой компании, отображаемое для клиентов:</span><span class="sxs-lookup"><span data-stu-id="f8c74-120">At minimum, you should specify a name for the new business that customers will see:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="f8c74-121">Используйте свойство **id** нового объекта **bookingBusiness**, возвращенного в отклике POST, чтобы продолжить [настройку](../api/bookingbusiness-update.md) бизнес-параметров и добавить сотрудников и услуги для компании.</span><span class="sxs-lookup"><span data-stu-id="f8c74-121">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="f8c74-122">Добавьте отдельных сотрудников для компании:</span><span class="sxs-lookup"><span data-stu-id="f8c74-122">Add individual staff members for the business:</span></span>
<!-- { "blockType": "ignored" } -->
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
4. <span data-ttu-id="f8c74-123">Определите каждую услугу, предлагаемую компанией:</span><span class="sxs-lookup"><span data-stu-id="f8c74-123">Define each service offered by the business:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="f8c74-124">Опубликуйте страницу расписания для компании, чтобы у клиентов и бизнес-операторов была возможность начать резервирование встреч:</span><span class="sxs-lookup"><span data-stu-id="f8c74-124">Publish the scheduling page for the business, to let customers and business operators start booking appointments:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="f8c74-125">Как правило, можно указать список всех компаний для резервирования в клиенте Office 365:</span><span class="sxs-lookup"><span data-stu-id="f8c74-125">In general, to list all the booking businesses in the Office 365 tenant:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="f8c74-126">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="f8c74-126">Common use cases</span></span> 

<span data-ttu-id="f8c74-127">В таблице ниже перечислены распространенные операции для бизнеса в API Bookings.</span><span class="sxs-lookup"><span data-stu-id="f8c74-127">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="f8c74-128">Варианты использования</span><span class="sxs-lookup"><span data-stu-id="f8c74-128">Use cases</span></span>        | <span data-ttu-id="f8c74-129">Ресурсы REST</span><span class="sxs-lookup"><span data-stu-id="f8c74-129">REST resources</span></span> | <span data-ttu-id="f8c74-130">См. также</span><span class="sxs-lookup"><span data-stu-id="f8c74-130">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="f8c74-131">Создание, получение, обновление или удаление компании</span><span class="sxs-lookup"><span data-stu-id="f8c74-131">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="f8c74-132">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f8c74-132">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="f8c74-133">Методы ресурса bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f8c74-133">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="f8c74-134">Обновление политики планирования</span><span class="sxs-lookup"><span data-stu-id="f8c74-134">Update the scheduling policy</span></span> | [<span data-ttu-id="f8c74-135">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="f8c74-135">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="f8c74-136">Обновление bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f8c74-136">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="f8c74-137">Добавление, получение, обновление или удаление сотрудников</span><span class="sxs-lookup"><span data-stu-id="f8c74-137">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="f8c74-138">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="f8c74-138">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="f8c74-139">Методы ресурса bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="f8c74-139">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="f8c74-140">Добавление, получение, обновление или удаление услуг</span><span class="sxs-lookup"><span data-stu-id="f8c74-140">Add, get, update, or delete services</span></span> | [<span data-ttu-id="f8c74-141">bookingService</span><span class="sxs-lookup"><span data-stu-id="f8c74-141">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="f8c74-142">Методы ресурса bookingService</span><span class="sxs-lookup"><span data-stu-id="f8c74-142">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="f8c74-143">Публикация или отмена публикации страницы расписания</span><span class="sxs-lookup"><span data-stu-id="f8c74-143">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="f8c74-144">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f8c74-144">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="f8c74-145">publish</span><span class="sxs-lookup"><span data-stu-id="f8c74-145">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="f8c74-146">unpublish</span><span class="sxs-lookup"><span data-stu-id="f8c74-146">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="f8c74-147">Создание, получение, обновление, удаление или отмена встречи</span><span class="sxs-lookup"><span data-stu-id="f8c74-147">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="f8c74-148">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="f8c74-148">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="f8c74-149">Методы ресурса bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="f8c74-149">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="f8c74-150">Получение встреч в диапазоне дат</span><span class="sxs-lookup"><span data-stu-id="f8c74-150">Get appointments in a date range</span></span> | [<span data-ttu-id="f8c74-151">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f8c74-151">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="f8c74-152">Представление календаря "Список резервирований"</span><span class="sxs-lookup"><span data-stu-id="f8c74-152">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="f8c74-153">Получение валюты</span><span class="sxs-lookup"><span data-stu-id="f8c74-153">Get currency</span></span> | [<span data-ttu-id="f8c74-154">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="f8c74-154">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="f8c74-155">Методы ресурса bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="f8c74-155">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |


## <a name="see-also"></a><span data-ttu-id="f8c74-156">См. также</span><span class="sxs-lookup"><span data-stu-id="f8c74-156">See also</span></span>

- <span data-ttu-id="f8c74-157">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="f8c74-157">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="f8c74-158">Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span><span class="sxs-lookup"><span data-stu-id="f8c74-158">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
- <span data-ttu-id="f8c74-159">Узнайте, как выбрать [разрешения](/graph/permissions-reference) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f8c74-159">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>
