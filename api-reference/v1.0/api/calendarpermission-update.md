---
title: Обновление календарпермиссион
description: Обновление свойств объекта календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b990b038960a97eb8ba8e86d6a338cebe4339fbb
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227880"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="b4074-103">Обновление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="b4074-103">Update calendarPermission</span></span>

<span data-ttu-id="b4074-104">Обновление разрешений, назначенных существующему общему ресурсу или представителю, с помощью соответствующего объекта [календарпермиссион](../resources/calendarpermission.md) для календаря.</span><span class="sxs-lookup"><span data-stu-id="b4074-104">Update the permissions assigned to an existing sharee or delegate, through the corresponding [calendarPermission](../resources/calendarpermission.md) object for a calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4074-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4074-105">Permissions</span></span>

<span data-ttu-id="b4074-106">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="b4074-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="b4074-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4074-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4074-108">Календарь</span><span class="sxs-lookup"><span data-stu-id="b4074-108">Calendar</span></span> | <span data-ttu-id="b4074-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4074-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b4074-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4074-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4074-111">Приложение</span><span class="sxs-lookup"><span data-stu-id="b4074-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="b4074-112">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="b4074-112">user calendar</span></span> | <span data-ttu-id="b4074-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4074-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="b4074-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4074-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="b4074-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4074-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="b4074-116">календарь группы</span><span class="sxs-lookup"><span data-stu-id="b4074-116">group calendar</span></span> | <span data-ttu-id="b4074-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4074-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="b4074-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4074-118">Not supported.</span></span> | <span data-ttu-id="b4074-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4074-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4074-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4074-120">HTTP request</span></span>

<span data-ttu-id="b4074-121">Обновление указанных разрешений для календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="b4074-121">Update the specified permissions of a user's calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="b4074-122">Обновление указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="b4074-122">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="b4074-123">Обновление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="b4074-123">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b4074-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4074-124">Request headers</span></span>

| <span data-ttu-id="b4074-125">Имя</span><span class="sxs-lookup"><span data-stu-id="b4074-125">Name</span></span>       | <span data-ttu-id="b4074-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b4074-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b4074-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4074-127">Authorization</span></span> | <span data-ttu-id="b4074-128">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b4074-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4074-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4074-129">Request body</span></span>

<span data-ttu-id="b4074-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b4074-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b4074-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="b4074-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b4074-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b4074-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4074-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4074-133">Property</span></span>     | <span data-ttu-id="b4074-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b4074-134">Type</span></span>        | <span data-ttu-id="b4074-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b4074-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4074-136">role</span><span class="sxs-lookup"><span data-stu-id="b4074-136">role</span></span>|[<span data-ttu-id="b4074-137">календарролетипе</span><span class="sxs-lookup"><span data-stu-id="b4074-137">calendarRoleType</span></span>](../resources/calendarpermission.md#calendarroletype-values)| <span data-ttu-id="b4074-138">Уровень разрешений, на который изменяется общий доступ к календарю или представитель.</span><span class="sxs-lookup"><span data-stu-id="b4074-138">The permission level to change to for the calendar sharee or delegate.</span></span> |

## <a name="response"></a><span data-ttu-id="b4074-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4074-139">Response</span></span>

<span data-ttu-id="b4074-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [календарпермиссион](../resources/calendarpermission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4074-140">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4074-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="b4074-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4074-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4074-142">Request</span></span>

<span data-ttu-id="b4074-143">В следующем примере изменяется уровень разрешений для объекта Share, Александра, на `write`.</span><span class="sxs-lookup"><span data-stu-id="b4074-143">The following example changes the permission level of the sharee, Adele, to `write`.</span></span>

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

### <a name="response"></a><span data-ttu-id="b4074-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4074-144">Response</span></span>

<span data-ttu-id="b4074-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b4074-145">The following is an example of the response.</span></span>

> <span data-ttu-id="b4074-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4074-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
