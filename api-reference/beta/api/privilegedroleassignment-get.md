---
title: Получение privilegedRoleAssignment
description: Извлечение свойств и связи объекта privilegedRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 220001f523971adadd80a406b54f16d22f2ef48e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520321"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="f6cd3-103">Получение privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f6cd3-103">Get privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6cd3-104">Извлечение свойств и связи объекта privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="f6cd3-104">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6cd3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6cd3-105">Permissions</span></span>
<span data-ttu-id="f6cd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6cd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f6cd3-108">Запросившая сторона должен иметь одно из следующих ролей: _Привилегированной роль администратора_, _Глобального администратора_, _Администратора безопасности_или _Безопасности чтения_.</span><span class="sxs-lookup"><span data-stu-id="f6cd3-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="f6cd3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6cd3-109">Permission type</span></span>      | <span data-ttu-id="f6cd3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6cd3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6cd3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6cd3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6cd3-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6cd3-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6cd3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6cd3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6cd3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6cd3-114">Not supported.</span></span>    |
|<span data-ttu-id="f6cd3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6cd3-115">Application</span></span> | <span data-ttu-id="f6cd3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6cd3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6cd3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6cd3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6cd3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6cd3-118">Optional query parameters</span></span>
<span data-ttu-id="f6cd3-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f6cd3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6cd3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6cd3-120">Request headers</span></span>
| <span data-ttu-id="f6cd3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f6cd3-121">Name</span></span>      |<span data-ttu-id="f6cd3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f6cd3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f6cd3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6cd3-123">Authorization</span></span>  | <span data-ttu-id="f6cd3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6cd3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6cd3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6cd3-126">Request body</span></span>
<span data-ttu-id="f6cd3-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6cd3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6cd3-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6cd3-128">Response</span></span>

<span data-ttu-id="f6cd3-129">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedRoleAssignment](../resources/privilegedroleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f6cd3-129">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="f6cd3-130">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="f6cd3-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f6cd3-131">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="f6cd3-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="f6cd3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f6cd3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6cd3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6cd3-133">Request</span></span>
<span data-ttu-id="f6cd3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6cd3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="f6cd3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6cd3-135">Response</span></span>
<span data-ttu-id="f6cd3-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f6cd3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
