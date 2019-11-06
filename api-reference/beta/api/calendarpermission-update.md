---
title: Обновление календарпермиссион
description: Обновление свойств объекта календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7aee071949fb5d7ded115f131e732b6d3626e6fd
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994851"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="21afb-103">Обновление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="21afb-103">Update calendarPermission</span></span>

<span data-ttu-id="21afb-104">Обновление свойств объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="21afb-104">Update the properties of calendarPermission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="21afb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21afb-105">Permissions</span></span>

<span data-ttu-id="21afb-106">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="21afb-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="21afb-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21afb-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21afb-108">Календарь</span><span class="sxs-lookup"><span data-stu-id="21afb-108">Calendar</span></span> | <span data-ttu-id="21afb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21afb-109">Delegated (work or school account)</span></span> | <span data-ttu-id="21afb-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21afb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21afb-111">Приложение</span><span class="sxs-lookup"><span data-stu-id="21afb-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="21afb-112">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="21afb-112">user calendar</span></span> | <span data-ttu-id="21afb-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21afb-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="21afb-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21afb-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="21afb-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21afb-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="21afb-116">календарь группы</span><span class="sxs-lookup"><span data-stu-id="21afb-116">group calendar</span></span> | <span data-ttu-id="21afb-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21afb-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="21afb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21afb-118">Not supported.</span></span> | <span data-ttu-id="21afb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21afb-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21afb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21afb-120">HTTP request</span></span>

<span data-ttu-id="21afb-121">Обновление указанных разрешений для основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="21afb-121">Update the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="21afb-122">Обновление указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="21afb-122">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="21afb-123">Обновление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="21afb-123">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="21afb-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21afb-124">Request headers</span></span>

| <span data-ttu-id="21afb-125">Имя</span><span class="sxs-lookup"><span data-stu-id="21afb-125">Name</span></span>       | <span data-ttu-id="21afb-126">Описание</span><span class="sxs-lookup"><span data-stu-id="21afb-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="21afb-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="21afb-127">Authorization</span></span> | <span data-ttu-id="21afb-128">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="21afb-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="21afb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21afb-129">Request body</span></span>

<span data-ttu-id="21afb-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="21afb-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="21afb-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="21afb-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="21afb-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="21afb-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="21afb-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="21afb-133">Property</span></span>     | <span data-ttu-id="21afb-134">Тип</span><span class="sxs-lookup"><span data-stu-id="21afb-134">Type</span></span>        | <span data-ttu-id="21afb-135">Описание</span><span class="sxs-lookup"><span data-stu-id="21afb-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21afb-136">алловедролес</span><span class="sxs-lookup"><span data-stu-id="21afb-136">allowedRoles</span></span>|<span data-ttu-id="21afb-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="21afb-137">string collection</span></span>| <span data-ttu-id="21afb-138">Список разрешенных для общего доступа уровней разрешений для календаря.</span><span class="sxs-lookup"><span data-stu-id="21afb-138">List of allowed sharing permission levels for the calendar.</span></span> <span data-ttu-id="21afb-139">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="21afb-139">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="21afb-140">emailAddress</span><span class="sxs-lookup"><span data-stu-id="21afb-140">emailAddress</span></span>|[<span data-ttu-id="21afb-141">emailAddress</span><span class="sxs-lookup"><span data-stu-id="21afb-141">emailAddress</span></span>](../resources/email.md)| <span data-ttu-id="21afb-142">Представляет общую папку, у которой есть доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="21afb-142">Represents a sharee who has access to the calendar.</span></span> <span data-ttu-id="21afb-143">Для общего доступа к общему ресурсу "Моя организация" свойство **Address** имеет значение null.</span><span class="sxs-lookup"><span data-stu-id="21afb-143">For the "My Organization" sharee, the **address** property is null.</span></span> |
|<span data-ttu-id="21afb-144">id</span><span class="sxs-lookup"><span data-stu-id="21afb-144">id</span></span>|<span data-ttu-id="21afb-145">String</span><span class="sxs-lookup"><span data-stu-id="21afb-145">String</span></span>| <span data-ttu-id="21afb-146">Уникальный идентификатор пользователя (общего доступа), с которым открыт общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="21afb-146">The unique identifier of the user (sharee) with whom the calendar has been shared.</span></span> <span data-ttu-id="21afb-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21afb-147">Read-only.</span></span>|
|<span data-ttu-id="21afb-148">исинсидеорганизатион</span><span class="sxs-lookup"><span data-stu-id="21afb-148">isInsideOrganization</span></span>|<span data-ttu-id="21afb-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="21afb-149">Boolean</span></span>| <span data-ttu-id="21afb-150">Значение true, если пользователь в контексте (Share) находится в той же организации, что и владелец календаря.</span><span class="sxs-lookup"><span data-stu-id="21afb-150">True if the user in context (sharee) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="21afb-151">"несъемный"</span><span class="sxs-lookup"><span data-stu-id="21afb-151">isRemovable</span></span>|<span data-ttu-id="21afb-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="21afb-152">Boolean</span></span>| <span data-ttu-id="21afb-153">`True`, если пользователь может быть удален из списка общих папок для указанного календаря, `false` в противном случае.</span><span class="sxs-lookup"><span data-stu-id="21afb-153">`True` if the user can be removed from the list of sharees for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="21afb-154">Пользователь "Моя организация" определяет разрешения, которые пользователи в организации имеют в указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="21afb-154">The “My organization” user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="21afb-155">Вы не можете удалить "Моя организация" как общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="21afb-155">You cannot remove  “My organization” as a sharee to a calendar.</span></span>|
|<span data-ttu-id="21afb-156">role</span><span class="sxs-lookup"><span data-stu-id="21afb-156">role</span></span>|<span data-ttu-id="21afb-157">календарролетипе</span><span class="sxs-lookup"><span data-stu-id="21afb-157">calendarRoleType</span></span>| <span data-ttu-id="21afb-158">Текущий уровень разрешений общего календаря.</span><span class="sxs-lookup"><span data-stu-id="21afb-158">Current permission level of the calendar sharee.</span></span> <span data-ttu-id="21afb-159">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="21afb-159">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="21afb-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="21afb-160">Response</span></span>

<span data-ttu-id="21afb-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [календарпермиссион](../resources/calendarpermission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="21afb-161">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21afb-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="21afb-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="21afb-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="21afb-163">Request</span></span>

<span data-ttu-id="21afb-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21afb-164">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="21afb-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="21afb-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="21afb-166">C#</span><span class="sxs-lookup"><span data-stu-id="21afb-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21afb-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21afb-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21afb-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21afb-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="21afb-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="21afb-169">Response</span></span>

<span data-ttu-id="21afb-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21afb-170">The following is an example of the response.</span></span>

> <span data-ttu-id="21afb-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21afb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
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
