---
title: Обновление календарпермиссион
description: Обновление свойств объекта календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e69a1b4cdc66e9c591d060bed6600c4383e14a63
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936792"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="f026b-103">Обновление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="f026b-103">Update calendarPermission</span></span>

<span data-ttu-id="f026b-104">Обновление свойств объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="f026b-104">Update the properties of calendarPermission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f026b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f026b-105">Permissions</span></span>

<span data-ttu-id="f026b-106">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="f026b-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="f026b-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f026b-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f026b-108">Календарь</span><span class="sxs-lookup"><span data-stu-id="f026b-108">Calendar</span></span> | <span data-ttu-id="f026b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f026b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f026b-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f026b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f026b-111">Приложение</span><span class="sxs-lookup"><span data-stu-id="f026b-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="f026b-112">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="f026b-112">user calendar</span></span> | <span data-ttu-id="f026b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f026b-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="f026b-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f026b-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="f026b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f026b-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="f026b-116">календарь группы</span><span class="sxs-lookup"><span data-stu-id="f026b-116">group calendar</span></span> | <span data-ttu-id="f026b-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f026b-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="f026b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f026b-118">Not supported.</span></span> | <span data-ttu-id="f026b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f026b-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f026b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f026b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
PATCH /groups/{id}/calendar/calendarPermissions/{id}
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f026b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f026b-121">Request headers</span></span>

| <span data-ttu-id="f026b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f026b-122">Name</span></span>       | <span data-ttu-id="f026b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f026b-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f026b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f026b-124">Authorization</span></span> | <span data-ttu-id="f026b-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f026b-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f026b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f026b-126">Request body</span></span>

<span data-ttu-id="f026b-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f026b-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f026b-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="f026b-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f026b-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f026b-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f026b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f026b-130">Property</span></span>     | <span data-ttu-id="f026b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f026b-131">Type</span></span>        | <span data-ttu-id="f026b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f026b-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f026b-133">алловедролес</span><span class="sxs-lookup"><span data-stu-id="f026b-133">allowedRoles</span></span>|<span data-ttu-id="f026b-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f026b-134">string collection</span></span>| <span data-ttu-id="f026b-135">Список разрешенных для общего доступа уровней разрешений для календаря.</span><span class="sxs-lookup"><span data-stu-id="f026b-135">List of allowed sharing permission levels for the calendar.</span></span> <span data-ttu-id="f026b-136">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="f026b-136">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="f026b-137">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f026b-137">emailAddress</span></span>|[<span data-ttu-id="f026b-138">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f026b-138">emailAddress</span></span>](../resources/email.md)| <span data-ttu-id="f026b-139">Представляет общую папку, у которой есть доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="f026b-139">Represents a sharee who has access to the calendar.</span></span> <span data-ttu-id="f026b-140">Для общего доступа к общему ресурсу "Моя организация" свойство **Address** имеет значение null.</span><span class="sxs-lookup"><span data-stu-id="f026b-140">For the "My Organization" sharee, the **address** property is null.</span></span> |
|<span data-ttu-id="f026b-141">id</span><span class="sxs-lookup"><span data-stu-id="f026b-141">id</span></span>|<span data-ttu-id="f026b-142">Строка</span><span class="sxs-lookup"><span data-stu-id="f026b-142">String</span></span>| <span data-ttu-id="f026b-143">Уникальный идентификатор пользователя (общего доступа), с которым открыт общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="f026b-143">The unique identifier of the user (sharee) with whom the calendar has been shared.</span></span> <span data-ttu-id="f026b-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f026b-144">Read-only.</span></span>|
|<span data-ttu-id="f026b-145">исинсидеорганизатион</span><span class="sxs-lookup"><span data-stu-id="f026b-145">isInsideOrganization</span></span>|<span data-ttu-id="f026b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f026b-146">Boolean</span></span>| <span data-ttu-id="f026b-147">Значение true, если пользователь в контексте (Share) находится в той же организации, что и владелец календаря.</span><span class="sxs-lookup"><span data-stu-id="f026b-147">True if the user in context (sharee) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="f026b-148">"несъемный"</span><span class="sxs-lookup"><span data-stu-id="f026b-148">isRemovable</span></span>|<span data-ttu-id="f026b-149">Логический</span><span class="sxs-lookup"><span data-stu-id="f026b-149">Boolean</span></span>| <span data-ttu-id="f026b-150">`True`, если пользователь может быть удален из списка общих папок для указанного календаря, `false` в противном случае.</span><span class="sxs-lookup"><span data-stu-id="f026b-150">`True` if the user can be removed from the list of sharees for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="f026b-151">Пользователь "Моя организация" определяет разрешения, которые пользователи в организации имеют в указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="f026b-151">The “My organization” user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="f026b-152">Вы не можете удалить "Моя организация" как общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="f026b-152">You cannot remove  “My organization” as a sharee to a calendar.</span></span>|
|<span data-ttu-id="f026b-153">role</span><span class="sxs-lookup"><span data-stu-id="f026b-153">role</span></span>|<span data-ttu-id="f026b-154">календарролетипе</span><span class="sxs-lookup"><span data-stu-id="f026b-154">calendarRoleType</span></span>| <span data-ttu-id="f026b-155">Текущий уровень разрешений общего календаря.</span><span class="sxs-lookup"><span data-stu-id="f026b-155">Current permission level of the calendar sharee.</span></span> <span data-ttu-id="f026b-156">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="f026b-156">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="f026b-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="f026b-157">Response</span></span>

<span data-ttu-id="f026b-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [календарпермиссион](../resources/calendarpermission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f026b-158">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f026b-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="f026b-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f026b-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="f026b-160">Request</span></span>

<span data-ttu-id="f026b-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f026b-161">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f026b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="f026b-162">Response</span></span>

<span data-ttu-id="f026b-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f026b-163">The following is an example of the response.</span></span>

> <span data-ttu-id="f026b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f026b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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