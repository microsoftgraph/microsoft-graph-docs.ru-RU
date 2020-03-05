---
title: Обновление букингстаффмембер
description: Обновление свойств объекта Букингстаффмембер в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e710d98ffd287e2c763608d899f74ddf2e6ce82c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441069"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="f5942-103">Обновление букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="f5942-103">Update bookingstaffmember</span></span>

<span data-ttu-id="f5942-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f5942-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5942-105">Обновление свойств объекта [букингстаффмембер](../resources/bookingstaffmember.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="f5942-105">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="f5942-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5942-106">Permissions</span></span>
<span data-ttu-id="f5942-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5942-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5942-109">Permission type</span></span>      | <span data-ttu-id="f5942-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5942-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5942-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5942-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="f5942-112">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="f5942-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f5942-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5942-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5942-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5942-114">Not supported.</span></span>   |
|<span data-ttu-id="f5942-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5942-115">Application</span></span> | <span data-ttu-id="f5942-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5942-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f5942-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5942-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f5942-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5942-118">Optional request headers</span></span>
| <span data-ttu-id="f5942-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f5942-119">Name</span></span>       | <span data-ttu-id="f5942-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f5942-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f5942-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5942-121">Authorization</span></span>  | <span data-ttu-id="f5942-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f5942-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5942-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5942-123">Request body</span></span>
<span data-ttu-id="f5942-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f5942-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f5942-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5942-127">Property</span></span>     | <span data-ttu-id="f5942-128">Тип</span><span class="sxs-lookup"><span data-stu-id="f5942-128">Type</span></span>   |<span data-ttu-id="f5942-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f5942-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5942-130">аваилабилитисаффектедбиперсоналкалендар</span><span class="sxs-lookup"><span data-stu-id="f5942-130">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="f5942-131">Логический</span><span class="sxs-lookup"><span data-stu-id="f5942-131">Boolean</span></span>|<span data-ttu-id="f5942-132">True означает, что если сотрудник является пользователем Office 365, то в API учета используется личный календарь сотрудника в Office 365, а свойство **воркингхаурс** для определения доступности.</span><span class="sxs-lookup"><span data-stu-id="f5942-132">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="f5942-133">colorIndex</span><span class="sxs-lookup"><span data-stu-id="f5942-133">colorIndex</span></span>|<span data-ttu-id="f5942-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f5942-134">Int32</span></span>|<span data-ttu-id="f5942-135">Определяет цвет для представления сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f5942-135">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="f5942-136">Цвет соответствует цветовой палитре на странице " **сведения о персонале** " в приложении "книги".</span><span class="sxs-lookup"><span data-stu-id="f5942-136">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="f5942-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f5942-137">displayName</span></span>|<span data-ttu-id="f5942-138">String</span><span class="sxs-lookup"><span data-stu-id="f5942-138">String</span></span>|<span data-ttu-id="f5942-139">Имя сотрудника, отображаемое для клиентов.</span><span class="sxs-lookup"><span data-stu-id="f5942-139">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="f5942-140">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f5942-140">emailAddress</span></span>|<span data-ttu-id="f5942-141">String</span><span class="sxs-lookup"><span data-stu-id="f5942-141">String</span></span>|<span data-ttu-id="f5942-142">Адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f5942-142">The email address of the staff member.</span></span> <span data-ttu-id="f5942-143">Это может быть тот же клиент Office 365, что и в Организации, или в другом домене электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f5942-143">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="f5942-144">Этот адрес электронной почты используется, если для свойства **сендконфирматионстувнер** в политике планирования бизнеса задано значение true.</span><span class="sxs-lookup"><span data-stu-id="f5942-144">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="f5942-145">role</span><span class="sxs-lookup"><span data-stu-id="f5942-145">role</span></span>|<span data-ttu-id="f5942-146">строка</span><span class="sxs-lookup"><span data-stu-id="f5942-146">string</span></span>| <span data-ttu-id="f5942-147">Роль сотрудника в Организации.</span><span class="sxs-lookup"><span data-stu-id="f5942-147">The role of the staff member in the business.</span></span> <span data-ttu-id="f5942-148">Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="f5942-148">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="f5942-149">усебусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="f5942-149">useBusinessHours</span></span>|<span data-ttu-id="f5942-150">Логический</span><span class="sxs-lookup"><span data-stu-id="f5942-150">Boolean</span></span>|<span data-ttu-id="f5942-151">Значение true означает, что доступность сотрудника определяется свойством **businessHours** предприятия.</span><span class="sxs-lookup"><span data-stu-id="f5942-151">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="f5942-152">Значение false означает, что доступность определяется значением свойства **воркингхаусе** сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f5942-152">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="f5942-153">workingHours</span><span class="sxs-lookup"><span data-stu-id="f5942-153">workingHours</span></span>|<span data-ttu-id="f5942-154">Коллекция [букингворкхаурс](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="f5942-154">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="f5942-155">Диапазон часов на каждый день недели, когда сотрудник становится доступен для резервирования.</span><span class="sxs-lookup"><span data-stu-id="f5942-155">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="f5942-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5942-156">Response</span></span>
<span data-ttu-id="f5942-p107">При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f5942-p107">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5942-159">Пример</span><span class="sxs-lookup"><span data-stu-id="f5942-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5942-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5942-160">Request</span></span>
<span data-ttu-id="f5942-161">В следующем примере для сотрудника в календарном плане изменяется понедельник.</span><span class="sxs-lookup"><span data-stu-id="f5942-161">The following example changes the staff member's schedule to have Mondays off.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5942-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5942-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingstaffmember"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148
Content-type: application/json

{
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[

            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"tuesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"wednesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"thursday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"friday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="f5942-163">C#</span><span class="sxs-lookup"><span data-stu-id="f5942-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5942-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5942-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5942-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5942-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f5942-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5942-166">Response</span></span>
<span data-ttu-id="f5942-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5942-167">The following is an example of the response.</span></span>
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
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
