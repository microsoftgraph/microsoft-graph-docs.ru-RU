---
title: Получение privilegedRoleSettings
description: Извлечь параметры роли для данной роли. Объект privilegedRoleSettings будут возвращены.
localization_priority: Normal
ms.openlocfilehash: 7ecebad77acf2e090263878aacc29f00a9215fc7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508106"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="aa69b-104">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="aa69b-104">Get privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa69b-105">Извлечь параметры роли для данной роли.</span><span class="sxs-lookup"><span data-stu-id="aa69b-105">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="aa69b-106">Объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="aa69b-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa69b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa69b-107">Permissions</span></span>

<span data-ttu-id="aa69b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa69b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="aa69b-110">Запросившая сторона должен иметь одно из следующих ролей: _Привилегированной роль администратора_, _Глобального администратора_, _Администратора безопасности_или _Безопасности чтения_.</span><span class="sxs-lookup"><span data-stu-id="aa69b-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="aa69b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa69b-111">Permission type</span></span>      | <span data-ttu-id="aa69b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa69b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa69b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa69b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="aa69b-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aa69b-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aa69b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa69b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa69b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa69b-116">Not supported.</span></span>    |
|<span data-ttu-id="aa69b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa69b-117">Application</span></span> | <span data-ttu-id="aa69b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa69b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa69b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa69b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa69b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aa69b-120">Optional query parameters</span></span>
<span data-ttu-id="aa69b-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aa69b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa69b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa69b-122">Request headers</span></span>
| <span data-ttu-id="aa69b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="aa69b-123">Name</span></span>      |<span data-ttu-id="aa69b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="aa69b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa69b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa69b-125">Authorization</span></span>  | <span data-ttu-id="aa69b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa69b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa69b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa69b-128">Request body</span></span>
<span data-ttu-id="aa69b-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa69b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa69b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa69b-130">Response</span></span>

<span data-ttu-id="aa69b-131">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="aa69b-131">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="aa69b-132">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="aa69b-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="aa69b-133">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="aa69b-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="aa69b-134">Пример</span><span class="sxs-lookup"><span data-stu-id="aa69b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa69b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa69b-135">Request</span></span>
<span data-ttu-id="aa69b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa69b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="aa69b-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa69b-137">Response</span></span>
<span data-ttu-id="aa69b-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="aa69b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesettings-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
