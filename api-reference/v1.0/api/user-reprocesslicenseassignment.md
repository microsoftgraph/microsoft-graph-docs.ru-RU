---
title: 'Пользователь: Репроцесслиценсеассигнмент'
description: Повторно обработайте все назначения лицензий на основе группы для пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3d4da6d5998f55496e0c726fa015164307325f17
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953652"
---
# <a name="user-reprocesslicenseassignment"></a><span data-ttu-id="2191b-103">Пользователь: Репроцесслиценсеассигнмент</span><span class="sxs-lookup"><span data-stu-id="2191b-103">user: reprocessLicenseAssignment</span></span>

<span data-ttu-id="2191b-104">Повторно обработайте все назначения лицензий на основе группы для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2191b-104">Reprocess all group-based license assignments for the user.</span></span> <span data-ttu-id="2191b-105">Чтобы узнать больше о лицензировании на основе групп, ознакомьтесь со статьей " [Лицензирование на основе групп" в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="2191b-105">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span> <span data-ttu-id="2191b-106">Кроме того, для получения дополнительных сведений ознакомьтесь с [разрешениями проблем назначения лицензий для группы в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) .</span><span class="sxs-lookup"><span data-stu-id="2191b-106">Also see [Identify and resolve license assignment problems for a group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) for more details.</span></span>


## <a name="permissions"></a><span data-ttu-id="2191b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2191b-107">Permissions</span></span>
<span data-ttu-id="2191b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2191b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2191b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2191b-110">Permission type</span></span>      | <span data-ttu-id="2191b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2191b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2191b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2191b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2191b-113">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2191b-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="2191b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2191b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2191b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2191b-115">Not supported.</span></span>    |
|<span data-ttu-id="2191b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2191b-116">Application</span></span> | <span data-ttu-id="2191b-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2191b-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2191b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2191b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/reprocessLicenseAssignment

```
## <a name="request-headers"></a><span data-ttu-id="2191b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2191b-119">Request headers</span></span>
| <span data-ttu-id="2191b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2191b-120">Header</span></span>       | <span data-ttu-id="2191b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2191b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2191b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2191b-122">Authorization</span></span>  | <span data-ttu-id="2191b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2191b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2191b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2191b-125">Request body</span></span>
<span data-ttu-id="2191b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2191b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2191b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="2191b-127">Response</span></span>

<span data-ttu-id="2191b-128">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и обновленный объект [User](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2191b-128">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2191b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2191b-129">Example</span></span>
<span data-ttu-id="2191b-130">В приведенном ниже примере показано, как повторно обработать назначения лицензий для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2191b-130">The following example shows how to reprocess license assignments for the user.</span></span>
### <a name="request"></a><span data-ttu-id="2191b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2191b-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2191b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2191b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reprocessLicenseAssignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2191b-133">C#</span><span class="sxs-lookup"><span data-stu-id="2191b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-reprocesslicenseassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2191b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2191b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-reprocesslicenseassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2191b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2191b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-reprocesslicenseassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2191b-136">Java</span><span class="sxs-lookup"><span data-stu-id="2191b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-reprocesslicenseassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2191b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2191b-137">Response</span></span>

<span data-ttu-id="2191b-138">Отклик — обновленный объект User.</span><span class="sxs-lookup"><span data-stu-id="2191b-138">The response is the updated user object.</span></span>

><span data-ttu-id="2191b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2191b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: reprocessLicenseAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
