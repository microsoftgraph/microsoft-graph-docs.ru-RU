---
title: Получение privilegedRoleSettings
description: Получение параметров роли для заданной роли. Будет возвращен объект Привилежедролесеттингс.
localization_priority: Normal
ms.openlocfilehash: f3287939d14b54dfc3218802ae48049db8512cd1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337195"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="6827c-104">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6827c-104">Get privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6827c-105">Получение параметров роли для заданной роли.</span><span class="sxs-lookup"><span data-stu-id="6827c-105">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="6827c-106">Будет возвращен объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="6827c-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="6827c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6827c-107">Permissions</span></span>

<span data-ttu-id="6827c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6827c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6827c-110">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="6827c-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="6827c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6827c-111">Permission type</span></span>      | <span data-ttu-id="6827c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6827c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6827c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6827c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6827c-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6827c-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6827c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6827c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6827c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6827c-116">Not supported.</span></span>    |
|<span data-ttu-id="6827c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6827c-117">Application</span></span> | <span data-ttu-id="6827c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6827c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6827c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6827c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6827c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6827c-120">Optional query parameters</span></span>
<span data-ttu-id="6827c-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6827c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6827c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6827c-122">Request headers</span></span>
| <span data-ttu-id="6827c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6827c-123">Name</span></span>      |<span data-ttu-id="6827c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6827c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6827c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6827c-125">Authorization</span></span>  | <span data-ttu-id="6827c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6827c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6827c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6827c-128">Request body</span></span>
<span data-ttu-id="6827c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6827c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6827c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6827c-130">Response</span></span>

<span data-ttu-id="6827c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6827c-131">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="6827c-132">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="6827c-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6827c-133">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="6827c-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="6827c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6827c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6827c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6827c-135">Request</span></span>
<span data-ttu-id="6827c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6827c-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="6827c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6827c-137">Response</span></span>
<span data-ttu-id="6827c-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6827c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
