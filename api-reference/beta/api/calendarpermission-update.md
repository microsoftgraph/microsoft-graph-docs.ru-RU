---
title: Обновление календарпермиссион
description: Обновление свойств объекта календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 970edd0479798fc07e505476b24796b890221396
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440894"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="08b6f-103">Обновление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="08b6f-103">Update calendarPermission</span></span>

<span data-ttu-id="08b6f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="08b6f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08b6f-105">Обновление разрешений, назначенных существующему общему ресурсу или представителю, с помощью соответствующего объекта [календарпермиссион](../resources/calendarpermission.md) для календаря.</span><span class="sxs-lookup"><span data-stu-id="08b6f-105">Update the permissions assigned to an existing sharee or delegate, through the corresponding [calendarPermission](../resources/calendarpermission.md) object for a calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="08b6f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08b6f-106">Permissions</span></span>

<span data-ttu-id="08b6f-107">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="08b6f-107">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="08b6f-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08b6f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08b6f-109">Календарь</span><span class="sxs-lookup"><span data-stu-id="08b6f-109">Calendar</span></span> | <span data-ttu-id="08b6f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08b6f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08b6f-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08b6f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08b6f-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="08b6f-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="08b6f-113">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="08b6f-113">user calendar</span></span> | <span data-ttu-id="08b6f-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08b6f-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="08b6f-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08b6f-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="08b6f-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08b6f-116">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="08b6f-117">календарь группы</span><span class="sxs-lookup"><span data-stu-id="08b6f-117">group calendar</span></span> | <span data-ttu-id="08b6f-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08b6f-118">Group.ReadWrite.All</span></span> | <span data-ttu-id="08b6f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08b6f-119">Not supported.</span></span> | <span data-ttu-id="08b6f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08b6f-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08b6f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08b6f-121">HTTP request</span></span>

<span data-ttu-id="08b6f-122">Обновление указанных разрешений для календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="08b6f-122">Update the specified permissions of a user's calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="08b6f-123">Обновление указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="08b6f-123">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="08b6f-124">Обновление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="08b6f-124">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="08b6f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08b6f-125">Request headers</span></span>

| <span data-ttu-id="08b6f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="08b6f-126">Name</span></span>       | <span data-ttu-id="08b6f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="08b6f-127">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="08b6f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="08b6f-128">Authorization</span></span> | <span data-ttu-id="08b6f-129">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="08b6f-129">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="08b6f-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08b6f-130">Request body</span></span>

<span data-ttu-id="08b6f-131">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="08b6f-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="08b6f-132">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="08b6f-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="08b6f-133">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="08b6f-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="08b6f-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="08b6f-134">Property</span></span>     | <span data-ttu-id="08b6f-135">Тип</span><span class="sxs-lookup"><span data-stu-id="08b6f-135">Type</span></span>        | <span data-ttu-id="08b6f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="08b6f-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08b6f-137">role</span><span class="sxs-lookup"><span data-stu-id="08b6f-137">role</span></span>|[<span data-ttu-id="08b6f-138">календарролетипе</span><span class="sxs-lookup"><span data-stu-id="08b6f-138">calendarRoleType</span></span>](../resources/calendarpermission.md#calendarroletype-values)| <span data-ttu-id="08b6f-139">Уровень разрешений, на который изменяется общий доступ к календарю или представитель.</span><span class="sxs-lookup"><span data-stu-id="08b6f-139">The permission level to change to for the calendar sharee or delegate.</span></span> |

## <a name="response"></a><span data-ttu-id="08b6f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="08b6f-140">Response</span></span>

<span data-ttu-id="08b6f-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [календарпермиссион](../resources/calendarpermission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08b6f-141">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08b6f-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="08b6f-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="08b6f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="08b6f-143">Request</span></span>

<span data-ttu-id="08b6f-144">В следующем примере изменяется уровень разрешений для объекта Share, Александра, на `write`.</span><span class="sxs-lookup"><span data-stu-id="08b6f-144">The following example changes the permission level of the sharee, Adele, to `write`.</span></span>

# <a name="http"></a>[<span data-ttu-id="08b6f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="08b6f-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["RGVmYXVsdA=="],
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/RGVmYXVsdA==
Content-type: application/json

{
  "role": "write"
}
```
# <a name="c"></a>[<span data-ttu-id="08b6f-146">C#</span><span class="sxs-lookup"><span data-stu-id="08b6f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08b6f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08b6f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08b6f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08b6f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08b6f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="08b6f-149">Response</span></span>

<span data-ttu-id="08b6f-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08b6f-150">The following is an example of the response.</span></span>

> <span data-ttu-id="08b6f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08b6f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
