---
title: Обновление календарной комиссии
description: Обновление свойств объекта calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a91c174a9830494d6e44463aaaea8217c57849a8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051615"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="a3461-103">Обновление calendarPermission</span><span class="sxs-lookup"><span data-stu-id="a3461-103">Update calendarPermission</span></span>

<span data-ttu-id="a3461-104">Обновление разрешений, присвоенных существующему sharee или делегированию, с помощью соответствующего [объекта calendarPermission](../resources/calendarpermission.md) для календаря.</span><span class="sxs-lookup"><span data-stu-id="a3461-104">Update the permissions assigned to an existing sharee or delegate, through the corresponding [calendarPermission](../resources/calendarpermission.md) object for a calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3461-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3461-105">Permissions</span></span>

<span data-ttu-id="a3461-106">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="a3461-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="a3461-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3461-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3461-108">Календарь</span><span class="sxs-lookup"><span data-stu-id="a3461-108">Calendar</span></span> | <span data-ttu-id="a3461-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3461-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a3461-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3461-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3461-111">Приложение</span><span class="sxs-lookup"><span data-stu-id="a3461-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="a3461-112">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="a3461-112">user calendar</span></span> | <span data-ttu-id="a3461-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3461-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="a3461-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3461-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="a3461-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3461-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="a3461-116">календарь группы</span><span class="sxs-lookup"><span data-stu-id="a3461-116">group calendar</span></span> | <span data-ttu-id="a3461-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3461-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="a3461-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3461-118">Not supported.</span></span> | <span data-ttu-id="a3461-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3461-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3461-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3461-120">HTTP request</span></span>

<span data-ttu-id="a3461-121">Обновление указанных разрешений календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="a3461-121">Update the specified permissions of a user's calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="a3461-122">Обновление указанных разрешений группового календаря:</span><span class="sxs-lookup"><span data-stu-id="a3461-122">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="a3461-123">Обнови указанные разрешения пользовательского календаря, который содержит указанное событие:</span><span class="sxs-lookup"><span data-stu-id="a3461-123">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a3461-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3461-124">Request headers</span></span>

| <span data-ttu-id="a3461-125">Имя</span><span class="sxs-lookup"><span data-stu-id="a3461-125">Name</span></span>       | <span data-ttu-id="a3461-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a3461-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a3461-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3461-127">Authorization</span></span> | <span data-ttu-id="a3461-128">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a3461-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3461-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3461-129">Request body</span></span>

<span data-ttu-id="a3461-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a3461-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a3461-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a3461-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a3461-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a3461-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a3461-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3461-133">Property</span></span>     | <span data-ttu-id="a3461-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a3461-134">Type</span></span>        | <span data-ttu-id="a3461-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a3461-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a3461-136">role</span><span class="sxs-lookup"><span data-stu-id="a3461-136">role</span></span>|[<span data-ttu-id="a3461-137">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="a3461-137">calendarRoleType</span></span>](../resources/calendarpermission.md#calendarroletype-values)| <span data-ttu-id="a3461-138">Уровень разрешений для изменения для обмена календарем или делегирования.</span><span class="sxs-lookup"><span data-stu-id="a3461-138">The permission level to change to for the calendar sharee or delegate.</span></span> |

## <a name="response"></a><span data-ttu-id="a3461-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3461-139">Response</span></span>

<span data-ttu-id="a3461-140">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект calendarPermission](../resources/calendarpermission.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a3461-140">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3461-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="a3461-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3461-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3461-142">Request</span></span>

<span data-ttu-id="a3461-143">В следующем примере изменяется уровень разрешений sharee, Adele, на `write` .</span><span class="sxs-lookup"><span data-stu-id="a3461-143">The following example changes the permission level of the sharee, Adele, to `write`.</span></span>


# <a name="http"></a>[<span data-ttu-id="a3461-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3461-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a3461-145">C#</span><span class="sxs-lookup"><span data-stu-id="a3461-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3461-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3461-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3461-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3461-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3461-148">Java</span><span class="sxs-lookup"><span data-stu-id="a3461-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a3461-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3461-149">Response</span></span>

<span data-ttu-id="a3461-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a3461-150">The following is an example of the response.</span></span>

> <span data-ttu-id="a3461-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a3461-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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

