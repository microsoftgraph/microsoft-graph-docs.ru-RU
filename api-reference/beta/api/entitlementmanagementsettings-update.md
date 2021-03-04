---
title: Обновление entitlementManagementSettings
description: Обновление объекта entitlementManagementSettings, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8799edcb1eba5d88837916bc086b7238002889e7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436290"
---
# <a name="update-entitlementmanagementsettings"></a><span data-ttu-id="cc18f-103">Обновление entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="cc18f-103">Update entitlementManagementSettings</span></span>

<span data-ttu-id="cc18f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc18f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc18f-105">Обновим [существующий объект entitlementManagementSettings,](../resources/entitlementmanagementsettings.md) чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="cc18f-105">Update an existing [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object to change one or more of its properties.</span></span>


## <a name="permissions"></a><span data-ttu-id="cc18f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc18f-106">Permissions</span></span>
<span data-ttu-id="cc18f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc18f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc18f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc18f-109">Permission type</span></span>                        | <span data-ttu-id="cc18f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc18f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc18f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc18f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc18f-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc18f-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="cc18f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc18f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc18f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc18f-114">Not supported.</span></span> |
|<span data-ttu-id="cc18f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="cc18f-115">Application</span></span>                            | <span data-ttu-id="cc18f-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc18f-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc18f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc18f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/entitlementManagement/settings
```
## <a name="request-headers"></a><span data-ttu-id="cc18f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc18f-118">Request headers</span></span>
| <span data-ttu-id="cc18f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cc18f-119">Name</span></span>         | <span data-ttu-id="cc18f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cc18f-120">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="cc18f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc18f-121">Authorization</span></span> | <span data-ttu-id="cc18f-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="cc18f-122">Bearer \{token\}.</span></span> <span data-ttu-id="cc18f-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="cc18f-123">Required.</span></span> |
| <span data-ttu-id="cc18f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc18f-124">Content-Type</span></span>  | <span data-ttu-id="cc18f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc18f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc18f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc18f-127">Request body</span></span>
<span data-ttu-id="cc18f-128">В теле запроса поставляем представление JSON параметров объекта [entitlementManagementSettings.](../resources/entitlementmanagementsettings.md)</span><span class="sxs-lookup"><span data-stu-id="cc18f-128">In the request body, supply a JSON representation of the parameters of an [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cc18f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc18f-129">Response</span></span>
<span data-ttu-id="cc18f-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cc18f-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cc18f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cc18f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc18f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc18f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cc18f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc18f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_entitlementManagementSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
Content-type: application/json

{
  "externalUserLifecycleAction": "None"
}
```
# <a name="c"></a>[<span data-ttu-id="cc18f-134">C#</span><span class="sxs-lookup"><span data-stu-id="cc18f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc18f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc18f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc18f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc18f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc18f-137">Java</span><span class="sxs-lookup"><span data-stu-id="cc18f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-entitlementmanagementsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cc18f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc18f-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entitlementManagementSettings"
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update entitlementManagementSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


