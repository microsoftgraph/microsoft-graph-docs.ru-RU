---
title: Обновление Ентитлементманажементсеттингс
description: Обновление объекта Ентитлементманажементсеттингс для изменения одного или нескольких его свойств.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 23d37c089e9c81939ba9342a7f5747dd979b8bec
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225090"
---
# <a name="update-entitlementmanagementsettings"></a><span data-ttu-id="e305e-103">Обновление Ентитлементманажементсеттингс</span><span class="sxs-lookup"><span data-stu-id="e305e-103">Update entitlementManagementSettings</span></span>

<span data-ttu-id="e305e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e305e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e305e-105">Обновление существующего объекта [ентитлементманажементсеттингс](../resources/entitlementmanagementsettings.md) для изменения одного или нескольких его свойств.</span><span class="sxs-lookup"><span data-stu-id="e305e-105">Update an existing [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object to change one or more of its properties.</span></span>


## <a name="permissions"></a><span data-ttu-id="e305e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e305e-106">Permissions</span></span>
<span data-ttu-id="e305e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e305e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e305e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e305e-109">Permission type</span></span>                        | <span data-ttu-id="e305e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e305e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e305e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e305e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e305e-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e305e-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="e305e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e305e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e305e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e305e-114">Not supported.</span></span> |
|<span data-ttu-id="e305e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e305e-115">Application</span></span>                            | <span data-ttu-id="e305e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e305e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e305e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e305e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/entitlementManagement/settings
```
## <a name="request-headers"></a><span data-ttu-id="e305e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e305e-118">Request headers</span></span>
| <span data-ttu-id="e305e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e305e-119">Name</span></span>         | <span data-ttu-id="e305e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e305e-120">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="e305e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e305e-121">Authorization</span></span> | <span data-ttu-id="e305e-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="e305e-122">Bearer \{token\}.</span></span> <span data-ttu-id="e305e-123">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="e305e-123">Required.</span></span> |
| <span data-ttu-id="e305e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e305e-124">Content-Type</span></span>  | <span data-ttu-id="e305e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e305e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e305e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e305e-127">Request body</span></span>
<span data-ttu-id="e305e-128">В тексте запроса добавьте представление параметров объекта [ентитлементманажементсеттингс](../resources/entitlementmanagementsettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e305e-128">In the request body, supply a JSON representation of the parameters of an [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e305e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e305e-129">Response</span></span>
<span data-ttu-id="e305e-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e305e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e305e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e305e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e305e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e305e-132">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="e305e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e305e-133">Response</span></span>

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
