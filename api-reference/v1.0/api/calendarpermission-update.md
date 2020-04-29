---
title: Обновление календарпермиссион
description: Обновление свойств объекта календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2a9b3c5889023ebef22e9c3bec6004fbba2b46dd
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806538"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="b23bc-103">Обновление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="b23bc-103">Update calendarPermission</span></span>

<span data-ttu-id="b23bc-104">Обновление разрешений, назначенных существующему общему ресурсу или представителю, с помощью соответствующего объекта [календарпермиссион](../resources/calendarpermission.md) для календаря.</span><span class="sxs-lookup"><span data-stu-id="b23bc-104">Update the permissions assigned to an existing sharee or delegate, through the corresponding [calendarPermission](../resources/calendarpermission.md) object for a calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="b23bc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b23bc-105">Permissions</span></span>

<span data-ttu-id="b23bc-106">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="b23bc-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="b23bc-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b23bc-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b23bc-108">Календарь</span><span class="sxs-lookup"><span data-stu-id="b23bc-108">Calendar</span></span> | <span data-ttu-id="b23bc-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b23bc-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b23bc-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b23bc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b23bc-111">Приложение</span><span class="sxs-lookup"><span data-stu-id="b23bc-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="b23bc-112">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="b23bc-112">user calendar</span></span> | <span data-ttu-id="b23bc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b23bc-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="b23bc-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b23bc-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="b23bc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b23bc-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="b23bc-116">календарь группы</span><span class="sxs-lookup"><span data-stu-id="b23bc-116">group calendar</span></span> | <span data-ttu-id="b23bc-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b23bc-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="b23bc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b23bc-118">Not supported.</span></span> | <span data-ttu-id="b23bc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b23bc-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b23bc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b23bc-120">HTTP request</span></span>

<span data-ttu-id="b23bc-121">Обновление указанных разрешений для календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="b23bc-121">Update the specified permissions of a user's calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="b23bc-122">Обновление указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="b23bc-122">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="b23bc-123">Обновление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="b23bc-123">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b23bc-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b23bc-124">Request headers</span></span>

| <span data-ttu-id="b23bc-125">Имя</span><span class="sxs-lookup"><span data-stu-id="b23bc-125">Name</span></span>       | <span data-ttu-id="b23bc-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b23bc-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b23bc-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b23bc-127">Authorization</span></span> | <span data-ttu-id="b23bc-128">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b23bc-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b23bc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b23bc-129">Request body</span></span>

<span data-ttu-id="b23bc-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b23bc-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b23bc-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="b23bc-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b23bc-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b23bc-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b23bc-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="b23bc-133">Property</span></span>     | <span data-ttu-id="b23bc-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b23bc-134">Type</span></span>        | <span data-ttu-id="b23bc-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b23bc-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b23bc-136">role</span><span class="sxs-lookup"><span data-stu-id="b23bc-136">role</span></span>|[<span data-ttu-id="b23bc-137">календарролетипе</span><span class="sxs-lookup"><span data-stu-id="b23bc-137">calendarRoleType</span></span>](../resources/calendarpermission.md#calendarroletype-values)| <span data-ttu-id="b23bc-138">Уровень разрешений, на который изменяется общий доступ к календарю или представитель.</span><span class="sxs-lookup"><span data-stu-id="b23bc-138">The permission level to change to for the calendar sharee or delegate.</span></span> |

## <a name="response"></a><span data-ttu-id="b23bc-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="b23bc-139">Response</span></span>

<span data-ttu-id="b23bc-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [календарпермиссион](../resources/calendarpermission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b23bc-140">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b23bc-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="b23bc-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b23bc-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b23bc-142">Request</span></span>

<span data-ttu-id="b23bc-143">В следующем примере изменяется уровень разрешений для объекта Share, Александра, на `write`.</span><span class="sxs-lookup"><span data-stu-id="b23bc-143">The following example changes the permission level of the sharee, Adele, to `write`.</span></span>


# <a name="http"></a>[<span data-ttu-id="b23bc-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="b23bc-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["RGVmYXVsdA=="],
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/RGVmYXVsdA==
Content-type: application/json

{
  "role": "write"
}
```
# <a name="c"></a>[<span data-ttu-id="b23bc-145">C#</span><span class="sxs-lookup"><span data-stu-id="b23bc-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b23bc-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b23bc-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b23bc-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b23bc-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b23bc-148">Java</span><span class="sxs-lookup"><span data-stu-id="b23bc-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b23bc-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b23bc-149">Response</span></span>

<span data-ttu-id="b23bc-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b23bc-150">The following is an example of the response.</span></span>

> <span data-ttu-id="b23bc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b23bc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "update_calendarpermission",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "L289RXhlbGVW",
    "isRemovable": true,
    "isInsideOrganization": true,
    "role": "write",
    "allowedRoles": [
        "freeBusyRead",
        "limitedRead",
        "read",
        "write"
    ],
    "emailAddress": {
        "name": "Adele Vance",
        "address": "AdeleV@contoso.OnMicrosoft.com"
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendarpermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
