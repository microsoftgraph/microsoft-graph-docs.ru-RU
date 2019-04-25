---
title: Получение privilegedRoleSettings
description: Получение параметров роли для заданной роли. Будет возвращен объект Привилежедролесеттингс.
localization_priority: Normal
ms.openlocfilehash: 7ecebad77acf2e090263878aacc29f00a9215fc7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546472"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="9e091-104">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9e091-104">Get privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e091-105">Получение параметров роли для заданной роли.</span><span class="sxs-lookup"><span data-stu-id="9e091-105">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="9e091-106">Будет возвращен объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="9e091-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e091-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e091-107">Permissions</span></span>

<span data-ttu-id="9e091-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e091-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9e091-110">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="9e091-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="9e091-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e091-111">Permission type</span></span>      | <span data-ttu-id="9e091-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e091-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e091-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e091-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9e091-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e091-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e091-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e091-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e091-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e091-116">Not supported.</span></span>    |
|<span data-ttu-id="9e091-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e091-117">Application</span></span> | <span data-ttu-id="9e091-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e091-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e091-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e091-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e091-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9e091-120">Optional query parameters</span></span>
<span data-ttu-id="9e091-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9e091-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e091-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e091-122">Request headers</span></span>
| <span data-ttu-id="9e091-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9e091-123">Name</span></span>      |<span data-ttu-id="9e091-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9e091-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e091-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e091-125">Authorization</span></span>  | <span data-ttu-id="9e091-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e091-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e091-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e091-128">Request body</span></span>
<span data-ttu-id="9e091-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e091-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e091-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e091-130">Response</span></span>

<span data-ttu-id="9e091-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e091-131">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="9e091-132">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="9e091-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="9e091-133">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="9e091-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="9e091-134">Пример</span><span class="sxs-lookup"><span data-stu-id="9e091-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e091-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e091-135">Request</span></span>
<span data-ttu-id="9e091-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e091-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="9e091-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e091-137">Response</span></span>
<span data-ttu-id="9e091-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e091-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
