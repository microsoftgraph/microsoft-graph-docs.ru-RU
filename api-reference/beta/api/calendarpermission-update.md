---
title: Обновление календарпермиссион
description: Обновление свойств объекта календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d1cd959c4ee083ff6ec26914c5f99ccd3d8c3c8f
ms.sourcegitcommit: 1a3ca53422fc9a8254e78af7c058e876fc9f9ef8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2019
ms.locfileid: "37942643"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="40c98-103">Обновление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="40c98-103">Update calendarPermission</span></span>

<span data-ttu-id="40c98-104">Обновление свойств объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="40c98-104">Update the properties of calendarPermission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40c98-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40c98-105">Permissions</span></span>

<span data-ttu-id="40c98-106">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="40c98-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="40c98-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40c98-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40c98-108">Календарь</span><span class="sxs-lookup"><span data-stu-id="40c98-108">Calendar</span></span> | <span data-ttu-id="40c98-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40c98-109">Delegated (work or school account)</span></span> | <span data-ttu-id="40c98-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40c98-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40c98-111">Приложение</span><span class="sxs-lookup"><span data-stu-id="40c98-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="40c98-112">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="40c98-112">user calendar</span></span> | <span data-ttu-id="40c98-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40c98-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="40c98-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40c98-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="40c98-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40c98-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="40c98-116">календарь группы</span><span class="sxs-lookup"><span data-stu-id="40c98-116">group calendar</span></span> | <span data-ttu-id="40c98-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40c98-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="40c98-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40c98-118">Not supported.</span></span> | <span data-ttu-id="40c98-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40c98-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40c98-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40c98-120">HTTP request</span></span>

<span data-ttu-id="40c98-121">Обновление указанных разрешений для основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="40c98-121">Update the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="40c98-122">Обновление указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="40c98-122">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="40c98-123">Обновление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="40c98-123">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="40c98-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40c98-124">Request headers</span></span>

| <span data-ttu-id="40c98-125">Имя</span><span class="sxs-lookup"><span data-stu-id="40c98-125">Name</span></span>       | <span data-ttu-id="40c98-126">Описание</span><span class="sxs-lookup"><span data-stu-id="40c98-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="40c98-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40c98-127">Authorization</span></span> | <span data-ttu-id="40c98-128">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="40c98-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="40c98-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40c98-129">Request body</span></span>

<span data-ttu-id="40c98-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="40c98-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="40c98-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="40c98-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="40c98-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="40c98-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="40c98-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="40c98-133">Property</span></span>     | <span data-ttu-id="40c98-134">Тип</span><span class="sxs-lookup"><span data-stu-id="40c98-134">Type</span></span>        | <span data-ttu-id="40c98-135">Описание</span><span class="sxs-lookup"><span data-stu-id="40c98-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="40c98-136">алловедролес</span><span class="sxs-lookup"><span data-stu-id="40c98-136">allowedRoles</span></span>|<span data-ttu-id="40c98-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="40c98-137">string collection</span></span>| <span data-ttu-id="40c98-138">Список разрешенных для общего доступа уровней разрешений для календаря.</span><span class="sxs-lookup"><span data-stu-id="40c98-138">List of allowed sharing permission levels for the calendar.</span></span> <span data-ttu-id="40c98-139">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="40c98-139">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="40c98-140">emailAddress</span><span class="sxs-lookup"><span data-stu-id="40c98-140">emailAddress</span></span>|[<span data-ttu-id="40c98-141">emailAddress</span><span class="sxs-lookup"><span data-stu-id="40c98-141">emailAddress</span></span>](../resources/email.md)| <span data-ttu-id="40c98-142">Представляет общую папку, у которой есть доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="40c98-142">Represents a sharee who has access to the calendar.</span></span> <span data-ttu-id="40c98-143">Для общего доступа к общему ресурсу "Моя организация" свойство **Address** имеет значение null.</span><span class="sxs-lookup"><span data-stu-id="40c98-143">For the "My Organization" sharee, the **address** property is null.</span></span> |
|<span data-ttu-id="40c98-144">id</span><span class="sxs-lookup"><span data-stu-id="40c98-144">id</span></span>|<span data-ttu-id="40c98-145">String</span><span class="sxs-lookup"><span data-stu-id="40c98-145">String</span></span>| <span data-ttu-id="40c98-146">Уникальный идентификатор пользователя (общего доступа), с которым открыт общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="40c98-146">The unique identifier of the user (sharee) with whom the calendar has been shared.</span></span> <span data-ttu-id="40c98-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40c98-147">Read-only.</span></span>|
|<span data-ttu-id="40c98-148">исинсидеорганизатион</span><span class="sxs-lookup"><span data-stu-id="40c98-148">isInsideOrganization</span></span>|<span data-ttu-id="40c98-149">Логический</span><span class="sxs-lookup"><span data-stu-id="40c98-149">Boolean</span></span>| <span data-ttu-id="40c98-150">Значение true, если пользователь в контексте (Share) находится в той же организации, что и владелец календаря.</span><span class="sxs-lookup"><span data-stu-id="40c98-150">True if the user in context (sharee) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="40c98-151">"несъемный"</span><span class="sxs-lookup"><span data-stu-id="40c98-151">isRemovable</span></span>|<span data-ttu-id="40c98-152">Логический</span><span class="sxs-lookup"><span data-stu-id="40c98-152">Boolean</span></span>| <span data-ttu-id="40c98-153">`True`, если пользователь может быть удален из списка общих папок для указанного календаря, `false` в противном случае.</span><span class="sxs-lookup"><span data-stu-id="40c98-153">`True` if the user can be removed from the list of sharees for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="40c98-154">Пользователь "Моя организация" определяет разрешения, которые пользователи в организации имеют в указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="40c98-154">The “My organization” user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="40c98-155">Вы не можете удалить "Моя организация" как общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="40c98-155">You cannot remove  “My organization” as a sharee to a calendar.</span></span>|
|<span data-ttu-id="40c98-156">role</span><span class="sxs-lookup"><span data-stu-id="40c98-156">role</span></span>|<span data-ttu-id="40c98-157">календарролетипе</span><span class="sxs-lookup"><span data-stu-id="40c98-157">calendarRoleType</span></span>| <span data-ttu-id="40c98-158">Текущий уровень разрешений общего календаря.</span><span class="sxs-lookup"><span data-stu-id="40c98-158">Current permission level of the calendar sharee.</span></span> <span data-ttu-id="40c98-159">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="40c98-159">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="40c98-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="40c98-160">Response</span></span>

<span data-ttu-id="40c98-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [календарпермиссион](../resources/calendarpermission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40c98-161">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40c98-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="40c98-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40c98-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="40c98-163">Request</span></span>

<span data-ttu-id="40c98-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40c98-164">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="40c98-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="40c98-165">Response</span></span>

<span data-ttu-id="40c98-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40c98-166">The following is an example of the response.</span></span>

> <span data-ttu-id="40c98-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40c98-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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