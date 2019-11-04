---
title: Удаление Акцесспаккажеассигнментполици
description: Удаление Акцесспаккажеассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 07fb2f0139774e22b1e4f380c18ee91161254714
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936094"
---
# <a name="delete-accesspackageassignmentpolicy"></a><span data-ttu-id="8978b-103">Удаление Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="8978b-103">Delete accessPackageAssignmentPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8978b-104">В [управлении обслуживанием Azure AD](../resources/entitlementmanagement-root.md)удалите [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8978b-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), delete an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8978b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8978b-105">Permissions</span></span>

<span data-ttu-id="8978b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8978b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8978b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8978b-108">Permission type</span></span>                        | <span data-ttu-id="8978b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8978b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8978b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8978b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8978b-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8978b-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="8978b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8978b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8978b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8978b-113">Not supported.</span></span> |
| <span data-ttu-id="8978b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8978b-114">Application</span></span>                            | <span data-ttu-id="8978b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8978b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8978b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8978b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8978b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8978b-117">Request headers</span></span>

| <span data-ttu-id="8978b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8978b-118">Name</span></span>          | <span data-ttu-id="8978b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8978b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8978b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8978b-120">Authorization</span></span> | <span data-ttu-id="8978b-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="8978b-121">Bearer \{token\}.</span></span> <span data-ttu-id="8978b-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="8978b-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8978b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8978b-123">Request body</span></span>

<span data-ttu-id="8978b-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8978b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8978b-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="8978b-125">Response</span></span>

<span data-ttu-id="8978b-126">В случае успешного выполнения этот метод возвращает код ответа "нет содержимого" (204).</span><span class="sxs-lookup"><span data-stu-id="8978b-126">If successful, this method returns a 204 No Content response code.</span></span> <span data-ttu-id="8978b-127">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8978b-127">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8978b-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8978b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8978b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8978b-129">Request</span></span>

<span data-ttu-id="8978b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8978b-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accesspackageassignmentpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="8978b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8978b-131">Response</span></span>

<span data-ttu-id="8978b-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8978b-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
