---
title: Обновление entitlementManagementSettings
description: Обновление объекта entitlementManagementSettings, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f1b95cf9fdeb38d998fcd153d36611e5e0d43328
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787016"
---
# <a name="update-entitlementmanagementsettings"></a><span data-ttu-id="e4b42-103">Обновление entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="e4b42-103">Update entitlementManagementSettings</span></span>

<span data-ttu-id="e4b42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4b42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4b42-105">Обновим [существующий объект entitlementManagementSettings,](../resources/entitlementmanagementsettings.md) чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="e4b42-105">Update an existing [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object to change one or more of its properties.</span></span>


## <a name="permissions"></a><span data-ttu-id="e4b42-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4b42-106">Permissions</span></span>
<span data-ttu-id="e4b42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4b42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4b42-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4b42-109">Permission type</span></span>                        | <span data-ttu-id="e4b42-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4b42-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4b42-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4b42-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4b42-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4b42-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="e4b42-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4b42-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4b42-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4b42-114">Not supported.</span></span> |
|<span data-ttu-id="e4b42-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e4b42-115">Application</span></span>                            | <span data-ttu-id="e4b42-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4b42-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4b42-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4b42-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/entitlementManagement/settings
```
## <a name="request-headers"></a><span data-ttu-id="e4b42-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4b42-118">Request headers</span></span>
| <span data-ttu-id="e4b42-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e4b42-119">Name</span></span>         | <span data-ttu-id="e4b42-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e4b42-120">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="e4b42-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4b42-121">Authorization</span></span> | <span data-ttu-id="e4b42-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4b42-p102">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="e4b42-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4b42-124">Content-Type</span></span>  | <span data-ttu-id="e4b42-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4b42-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4b42-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4b42-127">Request body</span></span>
<span data-ttu-id="e4b42-128">В теле запроса поставляем представление JSON параметров объекта [entitlementManagementSettings.](../resources/entitlementmanagementsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e4b42-128">In the request body, supply a JSON representation of the parameters of an [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e4b42-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4b42-129">Response</span></span>
<span data-ttu-id="e4b42-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4b42-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4b42-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e4b42-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4b42-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4b42-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e4b42-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4b42-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e4b42-134">C#</span><span class="sxs-lookup"><span data-stu-id="e4b42-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4b42-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4b42-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4b42-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4b42-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4b42-137">Java</span><span class="sxs-lookup"><span data-stu-id="e4b42-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-entitlementmanagementsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e4b42-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4b42-138">Response</span></span>

<!-- {
  "blockType": "response"
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


