---
title: Член servicePrincipal списка
description: Получите групп и ролей каталогов, которые эта служба участника принадлежит к прямой. Эта операция не транзитивное.
ms.openlocfilehash: 54376d80fdb3cc5084ac19aa331b94d40ac3103f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082875"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="3d866-104">Член servicePrincipal списка</span><span class="sxs-lookup"><span data-stu-id="3d866-104">List servicePrincipal memberOf</span></span>

> <span data-ttu-id="3d866-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3d866-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d866-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d866-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d866-107">Получите групп и ролей каталогов, которые эта служба участника принадлежит к прямой.</span><span class="sxs-lookup"><span data-stu-id="3d866-107">Get the groups and directory roles that this service principal is a direct member of.</span></span> <span data-ttu-id="3d866-108">Эта операция не транзитивное.</span><span class="sxs-lookup"><span data-stu-id="3d866-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d866-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d866-109">Permissions</span></span>

<span data-ttu-id="3d866-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d866-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d866-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d866-112">Permission type</span></span>      | <span data-ttu-id="3d866-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d866-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d866-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d866-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3d866-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3d866-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3d866-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d866-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d866-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d866-117">Not supported.</span></span>    |
|<span data-ttu-id="3d866-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d866-118">Application</span></span> | <span data-ttu-id="3d866-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d866-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d866-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d866-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d866-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3d866-121">Optional query parameters</span></span>

<span data-ttu-id="3d866-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3d866-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d866-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d866-123">Request headers</span></span>
| <span data-ttu-id="3d866-124">Имя</span><span class="sxs-lookup"><span data-stu-id="3d866-124">Name</span></span>       | <span data-ttu-id="3d866-125">Тип</span><span class="sxs-lookup"><span data-stu-id="3d866-125">Type</span></span> | <span data-ttu-id="3d866-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3d866-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3d866-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d866-127">Authorization</span></span>  | <span data-ttu-id="3d866-128">string</span><span class="sxs-lookup"><span data-stu-id="3d866-128">string</span></span>  | <span data-ttu-id="3d866-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d866-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d866-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d866-131">Request body</span></span>
<span data-ttu-id="3d866-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d866-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d866-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d866-133">Response</span></span>

<span data-ttu-id="3d866-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d866-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d866-135">Пример</span><span class="sxs-lookup"><span data-stu-id="3d866-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d866-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d866-136">Request</span></span>

<span data-ttu-id="3d866-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d866-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="3d866-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d866-138">Response</span></span>

<span data-ttu-id="3d866-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3d866-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->