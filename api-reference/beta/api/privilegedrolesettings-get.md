---
title: Получение privilegedRoleSettings
description: Извлечь параметры роли для данной роли. Объект privilegedRoleSettings будут возвращены.
ms.openlocfilehash: c064e2eb11a4e91247894338c43c7c6dd9f9dcc3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076097"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="4a0f9-104">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="4a0f9-104">Get privilegedRoleSettings</span></span>

> <span data-ttu-id="4a0f9-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a0f9-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a0f9-107">Извлечь параметры роли для данной роли.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-107">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="4a0f9-108">Объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-108">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a0f9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a0f9-109">Permissions</span></span>

<span data-ttu-id="4a0f9-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a0f9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4a0f9-112">Запросившая сторона должен иметь одно из следующих ролей: _Привилегированной роль администратора_, _Глобального администратора_, _Администратора безопасности_или _Безопасности чтения_.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-112">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="4a0f9-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a0f9-113">Permission type</span></span>      | <span data-ttu-id="4a0f9-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a0f9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a0f9-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a0f9-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4a0f9-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a0f9-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4a0f9-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a0f9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a0f9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-118">Not supported.</span></span>    |
|<span data-ttu-id="4a0f9-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a0f9-119">Application</span></span> | <span data-ttu-id="4a0f9-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a0f9-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a0f9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4a0f9-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4a0f9-122">Optional query parameters</span></span>
<span data-ttu-id="4a0f9-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a0f9-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a0f9-124">Request headers</span></span>
| <span data-ttu-id="4a0f9-125">Имя</span><span class="sxs-lookup"><span data-stu-id="4a0f9-125">Name</span></span>      |<span data-ttu-id="4a0f9-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4a0f9-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a0f9-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a0f9-127">Authorization</span></span>  | <span data-ttu-id="4a0f9-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a0f9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a0f9-130">Request body</span></span>
<span data-ttu-id="4a0f9-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a0f9-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a0f9-132">Response</span></span>

<span data-ttu-id="4a0f9-133">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-133">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="4a0f9-134">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4a0f9-135">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="4a0f9-136">Пример</span><span class="sxs-lookup"><span data-stu-id="4a0f9-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a0f9-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a0f9-137">Request</span></span>
<span data-ttu-id="4a0f9-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="4a0f9-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a0f9-139">Response</span></span>
<span data-ttu-id="4a0f9-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4a0f9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 228

{
  "minElevationDuration": "2016-10-19T10:37:00Z",
  "maxElavationDuration": "2016-10-19T10:37:00Z",
  "elevationDuration": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->