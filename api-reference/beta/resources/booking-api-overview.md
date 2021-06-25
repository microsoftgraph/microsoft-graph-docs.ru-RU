---
title: Использование API Microsoft Bookings в Microsoft Graph
description: Microsoft Bookings позволяет крупным организациям и владельцам малого бизнеса управлять резервированиями и сведениями клиентов с минимальной настройкой.
localization_priority: Priority
author: arvindmicrosoft
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: c21cb95d140fa41711264ec0e6c71b7828b5a709
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118660"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="9979c-103">Использование API Microsoft Bookings в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9979c-103">Use the Microsoft Bookings API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="9979c-104">Microsoft Bookings позволяет крупным организациям и владельцам малого бизнеса управлять резервированиями и сведениями клиентов с минимальной настройкой.</span><span class="sxs-lookup"><span data-stu-id="9979c-104">Microsoft Bookings lets enterprise organization and small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="9979c-105">Владелец бизнеса можно создать одну или несколько компаний, каждая из которых предлагает набор услуг.</span><span class="sxs-lookup"><span data-stu-id="9979c-105">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="9979c-106">Владелец может настроить сотрудников и указать услуги, оказываемые каждым из них.</span><span class="sxs-lookup"><span data-stu-id="9979c-106">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="9979c-107">Клиент может зарезервировать встречу для определенной услуги в этой компании в сетевом или мобильном приложении.</span><span class="sxs-lookup"><span data-stu-id="9979c-107">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="9979c-108">Приложение Bookings обеспечивает обновление времени встречи для компании, сотрудников и соответствующих клиентов.</span><span class="sxs-lookup"><span data-stu-id="9979c-108">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="9979c-109">На программном уровне объект [bookingBusiness](bookingbusiness.md) в API Bookings включает указанные ниже объекты:</span><span class="sxs-lookup"><span data-stu-id="9979c-109">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="9979c-110">один или несколько объектов [bookingStaffMember](bookingstaffmember.md);</span><span class="sxs-lookup"><span data-stu-id="9979c-110">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="9979c-111">один или несколько объектов [bookingService](bookingservice.md);</span><span class="sxs-lookup"><span data-stu-id="9979c-111">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="9979c-112">набор экземпляров [bookingAppointment](bookingappointment.md);</span><span class="sxs-lookup"><span data-stu-id="9979c-112">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="9979c-113">набор объектов [bookingCustomer](bookingcustomer.md).</span><span class="sxs-lookup"><span data-stu-id="9979c-113">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="9979c-114">Использование REST API Bookings</span><span class="sxs-lookup"><span data-stu-id="9979c-114">Using the Bookings REST API</span></span>

<span data-ttu-id="9979c-115">Выполните указанные ниже действия перед первым резервированием встреч клиента с компанией.</span><span class="sxs-lookup"><span data-stu-id="9979c-115">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="9979c-116">Убедитесь, что предоставлены подходящие [маркеры доступа](/graph/auth-overview) для соответствующих операций.</span><span class="sxs-lookup"><span data-stu-id="9979c-116">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="9979c-117">Убедитесь, что у компании есть подписка на [Microsoft 365 бизнес премиум](https://products.office.com/ru-RU/business/office-365-business-premium).</span><span class="sxs-lookup"><span data-stu-id="9979c-117">Make sure the business has an [Microsoft 365 Business Premium](https://products.office.com/ru-RU/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="9979c-118">Создайте новый объект **bookingBusiness**, отправив операцию POST в набор объектов.</span><span class="sxs-lookup"><span data-stu-id="9979c-118">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="9979c-119">Как минимум, следует указать имя новой компании, отображаемое для клиентов:</span><span class="sxs-lookup"><span data-stu-id="9979c-119">At minimum, you should specify a name for the new business that customers will see:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="9979c-120">Используйте свойство **id** нового объекта **bookingBusiness**, возвращенного в отклике POST, чтобы продолжить [настройку](../api/bookingbusiness-update.md) бизнес-параметров и добавить сотрудников и услуги для компании.</span><span class="sxs-lookup"><span data-stu-id="9979c-120">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="9979c-121">Добавьте отдельных сотрудников для компании:</span><span class="sxs-lookup"><span data-stu-id="9979c-121">Add individual staff members for the business:</span></span>
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
4. <span data-ttu-id="9979c-122">Определите каждую услугу, предлагаемую компанией:</span><span class="sxs-lookup"><span data-stu-id="9979c-122">Define each service offered by the business:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="9979c-123">Опубликуйте страницу расписания для компании, чтобы у клиентов и бизнес-операторов была возможность начать резервирование встреч:</span><span class="sxs-lookup"><span data-stu-id="9979c-123">Publish the scheduling page for the business, to let customers and business operators start booking appointments:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="9979c-124">Как правило, можно указать список всех компаний для резервирования в клиенте Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="9979c-124">In general, to list all the booking businesses in the Microsoft 365 tenant:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="9979c-125">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="9979c-125">Common use cases</span></span> 

<span data-ttu-id="9979c-126">В таблице ниже перечислены распространенные операции для бизнеса в API Bookings.</span><span class="sxs-lookup"><span data-stu-id="9979c-126">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="9979c-127">Варианты использования</span><span class="sxs-lookup"><span data-stu-id="9979c-127">Use cases</span></span>        | <span data-ttu-id="9979c-128">Ресурсы REST</span><span class="sxs-lookup"><span data-stu-id="9979c-128">REST resources</span></span> | <span data-ttu-id="9979c-129">См. также</span><span class="sxs-lookup"><span data-stu-id="9979c-129">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="9979c-130">Создание, получение, обновление или удаление компании</span><span class="sxs-lookup"><span data-stu-id="9979c-130">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="9979c-131">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="9979c-131">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="9979c-132">Методы ресурса bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="9979c-132">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="9979c-133">Обновление политики планирования</span><span class="sxs-lookup"><span data-stu-id="9979c-133">Update the scheduling policy</span></span> | [<span data-ttu-id="9979c-134">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="9979c-134">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="9979c-135">Обновление bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="9979c-135">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="9979c-136">Добавление, получение, обновление или удаление сотрудников</span><span class="sxs-lookup"><span data-stu-id="9979c-136">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="9979c-137">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="9979c-137">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="9979c-138">Методы ресурса bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="9979c-138">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="9979c-139">Добавление, получение, обновление или удаление услуг</span><span class="sxs-lookup"><span data-stu-id="9979c-139">Add, get, update, or delete services</span></span> | [<span data-ttu-id="9979c-140">bookingService</span><span class="sxs-lookup"><span data-stu-id="9979c-140">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="9979c-141">Методы ресурса bookingService</span><span class="sxs-lookup"><span data-stu-id="9979c-141">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="9979c-142">Публикация или отмена публикации страницы расписания</span><span class="sxs-lookup"><span data-stu-id="9979c-142">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="9979c-143">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="9979c-143">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="9979c-144">publish</span><span class="sxs-lookup"><span data-stu-id="9979c-144">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="9979c-145">unpublish</span><span class="sxs-lookup"><span data-stu-id="9979c-145">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="9979c-146">Создание, получение, обновление, удаление или отмена встречи</span><span class="sxs-lookup"><span data-stu-id="9979c-146">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="9979c-147">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="9979c-147">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="9979c-148">Методы ресурса bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="9979c-148">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="9979c-149">Получение встреч в диапазоне дат</span><span class="sxs-lookup"><span data-stu-id="9979c-149">Get appointments in a date range</span></span> | [<span data-ttu-id="9979c-150">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="9979c-150">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="9979c-151">Представление календаря "Список резервирований"</span><span class="sxs-lookup"><span data-stu-id="9979c-151">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="9979c-152">Получение валюты</span><span class="sxs-lookup"><span data-stu-id="9979c-152">Get currency</span></span> | [<span data-ttu-id="9979c-153">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="9979c-153">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="9979c-154">Методы ресурса bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="9979c-154">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |

## <a name="whats-new"></a><span data-ttu-id="9979c-155">Новые возможности</span><span class="sxs-lookup"><span data-stu-id="9979c-155">What's new</span></span>
<span data-ttu-id="9979c-156">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="9979c-156">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="see-also"></a><span data-ttu-id="9979c-157">См. также</span><span class="sxs-lookup"><span data-stu-id="9979c-157">See also</span></span>

- <span data-ttu-id="9979c-158">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="9979c-158">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="9979c-159">Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/partners).</span><span class="sxs-lookup"><span data-stu-id="9979c-159">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/partners).</span></span>
- <span data-ttu-id="9979c-160">Узнайте, как выбрать [разрешения](/graph/permissions-reference) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9979c-160">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>


