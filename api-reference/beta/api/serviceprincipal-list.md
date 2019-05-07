---
title: Перечисление servicePrincipals
description: Получение списка объектов servicePrincipal.
localization_priority: Normal
ms.openlocfilehash: d431f2cd91fd1e2e27071bba92239b1984f630ab
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638679"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="bdf94-103">Перечисление servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="bdf94-103">List servicePrincipals</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdf94-104">Получение списка объектов servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="bdf94-104">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdf94-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdf94-105">Permissions</span></span>

<span data-ttu-id="bdf94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdf94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bdf94-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdf94-108">Permission type</span></span>      | <span data-ttu-id="bdf94-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdf94-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdf94-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdf94-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bdf94-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bdf94-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bdf94-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdf94-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdf94-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdf94-113">Not supported.</span></span>    |
|<span data-ttu-id="bdf94-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdf94-114">Application</span></span> | <span data-ttu-id="bdf94-115">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdf94-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdf94-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdf94-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bdf94-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bdf94-117">Optional query parameters</span></span>

<span data-ttu-id="bdf94-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bdf94-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bdf94-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdf94-119">Request headers</span></span>
| <span data-ttu-id="bdf94-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bdf94-120">Name</span></span> | <span data-ttu-id="bdf94-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf94-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="bdf94-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdf94-122">Authorization</span></span>  | <span data-ttu-id="bdf94-123">string</span><span class="sxs-lookup"><span data-stu-id="bdf94-123">string</span></span>  | <span data-ttu-id="bdf94-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdf94-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdf94-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdf94-126">Request body</span></span>

<span data-ttu-id="bdf94-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bdf94-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdf94-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdf94-128">Response</span></span>

<span data-ttu-id="bdf94-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdf94-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdf94-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bdf94-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bdf94-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdf94-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="bdf94-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdf94-132">Response</span></span>

<span data-ttu-id="bdf94-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdf94-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 488

{
  "value": [
    {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bdf94-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="bdf94-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bdf94-136">Языках</span><span class="sxs-lookup"><span data-stu-id="bdf94-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_serviceprincipals-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bdf94-137">Язык</span><span class="sxs-lookup"><span data-stu-id="bdf94-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_serviceprincipals-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
