---
title: 'Пользователь: Репроцесслиценсеассигнмент'
description: Повторно обработайте все назначения лицензий на основе группы для пользователя.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e4243e927ead9a282fd4e897b0d93ab612bf4459
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582242"
---
# <a name="user-reprocesslicenseassignment"></a><span data-ttu-id="de9ad-103">Пользователь: Репроцесслиценсеассигнмент</span><span class="sxs-lookup"><span data-stu-id="de9ad-103">user: reprocessLicenseAssignment</span></span>

<span data-ttu-id="de9ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de9ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de9ad-105">Повторно обработайте все назначения лицензий на основе группы для пользователя.</span><span class="sxs-lookup"><span data-stu-id="de9ad-105">Reprocess all group-based license assignments for the user.</span></span> <span data-ttu-id="de9ad-106">Чтобы узнать больше о лицензировании на основе групп, ознакомьтесь со статьей " [Лицензирование на основе групп" в Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="de9ad-106">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span> <span data-ttu-id="de9ad-107">Кроме того, для получения дополнительных сведений ознакомьтесь с [разрешениями проблем назначения лицензий для группы в Azure Active Directory](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) .</span><span class="sxs-lookup"><span data-stu-id="de9ad-107">Also see [Identify and resolve license assignment problems for a group in Azure Active Directory](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) for more details.</span></span>


## <a name="permissions"></a><span data-ttu-id="de9ad-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de9ad-108">Permissions</span></span>
<span data-ttu-id="de9ad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de9ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de9ad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de9ad-111">Permission type</span></span>      | <span data-ttu-id="de9ad-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de9ad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de9ad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de9ad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="de9ad-114">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de9ad-114">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="de9ad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de9ad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de9ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de9ad-116">Not supported.</span></span>    |
|<span data-ttu-id="de9ad-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de9ad-117">Application</span></span> | <span data-ttu-id="de9ad-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de9ad-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de9ad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de9ad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/reprocessLicenseAssignment

```
## <a name="request-headers"></a><span data-ttu-id="de9ad-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de9ad-120">Request headers</span></span>
| <span data-ttu-id="de9ad-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de9ad-121">Header</span></span>       | <span data-ttu-id="de9ad-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de9ad-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de9ad-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de9ad-123">Authorization</span></span>  | <span data-ttu-id="de9ad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de9ad-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de9ad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de9ad-126">Request body</span></span>
<span data-ttu-id="de9ad-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de9ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de9ad-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="de9ad-128">Response</span></span>

<span data-ttu-id="de9ad-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [User](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de9ad-129">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de9ad-130">Пример</span><span class="sxs-lookup"><span data-stu-id="de9ad-130">Example</span></span>
<span data-ttu-id="de9ad-131">В приведенном ниже примере показано, как повторно обработать назначения лицензий для пользователя.</span><span class="sxs-lookup"><span data-stu-id="de9ad-131">The following example shows how to reprocess license assignments for the user.</span></span>
### <a name="request"></a><span data-ttu-id="de9ad-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="de9ad-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="de9ad-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="de9ad-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reprocessLicenseAssignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment

```
# <a name="c"></a>[<span data-ttu-id="de9ad-134">C#</span><span class="sxs-lookup"><span data-stu-id="de9ad-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-reprocesslicenseassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de9ad-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de9ad-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-reprocesslicenseassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de9ad-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de9ad-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-reprocesslicenseassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de9ad-137">Java</span><span class="sxs-lookup"><span data-stu-id="de9ad-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-reprocesslicenseassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="de9ad-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="de9ad-138">Response</span></span>

<span data-ttu-id="de9ad-139">Отклик — обновленный объект User.</span><span class="sxs-lookup"><span data-stu-id="de9ad-139">The response is the updated user object.</span></span>

><span data-ttu-id="de9ad-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de9ad-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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