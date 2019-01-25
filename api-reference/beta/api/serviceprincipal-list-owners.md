---
title: 'servicePrincipals: список владельцев'
description: Получение списка владельцев servicePrincipal.
localization_priority: Normal
ms.openlocfilehash: ee591818db1183cee03079754ebf5d6278dcb9a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520286"
---
# <a name="serviceprincipals-list-owners"></a><span data-ttu-id="cb6db-103">servicePrincipals: список владельцев</span><span class="sxs-lookup"><span data-stu-id="cb6db-103">servicePrincipals: List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb6db-104">Получение списка владельцев servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="cb6db-104">Retrieve a list of owners of the servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb6db-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb6db-105">Permissions</span></span>
<span data-ttu-id="cb6db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb6db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb6db-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb6db-108">Permission type</span></span>      | <span data-ttu-id="cb6db-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb6db-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb6db-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb6db-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb6db-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb6db-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cb6db-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb6db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb6db-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb6db-113">Not supported.</span></span>    |
|<span data-ttu-id="cb6db-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb6db-114">Application</span></span> | <span data-ttu-id="cb6db-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb6db-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb6db-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb6db-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cb6db-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cb6db-117">Optional query parameters</span></span>
<span data-ttu-id="cb6db-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cb6db-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb6db-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb6db-119">Request headers</span></span>
| <span data-ttu-id="cb6db-120">Имя</span><span class="sxs-lookup"><span data-stu-id="cb6db-120">Name</span></span>       | <span data-ttu-id="cb6db-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cb6db-121">Type</span></span> | <span data-ttu-id="cb6db-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cb6db-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cb6db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb6db-123">Authorization</span></span>  | <span data-ttu-id="cb6db-124">string</span><span class="sxs-lookup"><span data-stu-id="cb6db-124">string</span></span>  | <span data-ttu-id="cb6db-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb6db-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb6db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb6db-127">Request body</span></span>
<span data-ttu-id="cb6db-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb6db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb6db-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb6db-129">Response</span></span>

<span data-ttu-id="cb6db-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb6db-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cb6db-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cb6db-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb6db-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb6db-132">Request</span></span>
<span data-ttu-id="cb6db-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb6db-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/owners
```
##### <a name="response"></a><span data-ttu-id="cb6db-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb6db-134">Response</span></span>
<span data-ttu-id="cb6db-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cb6db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
