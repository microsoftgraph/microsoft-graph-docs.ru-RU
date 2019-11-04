---
title: Создание Акцесспаккажеассигнментполици
description: Используйте этот API для создания нового Акцесспаккажеассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 280a532c2d0047fecb0085f88b73c92c30a4867f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936057"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="b47ae-103">Создание Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="b47ae-103">Create accessPackageAssignmentPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b47ae-104">В [управлении обслуживанием Azure AD](../resources/entitlementmanagement-root.md)используйте этот API, чтобы создать новый объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b47ae-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), use this API to create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b47ae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b47ae-105">Permissions</span></span>

<span data-ttu-id="b47ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b47ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b47ae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b47ae-108">Permission type</span></span>                        | <span data-ttu-id="b47ae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b47ae-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b47ae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b47ae-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b47ae-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b47ae-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="b47ae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b47ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b47ae-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b47ae-113">Not supported.</span></span> |
| <span data-ttu-id="b47ae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b47ae-114">Application</span></span>                            | <span data-ttu-id="b47ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b47ae-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b47ae-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b47ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="b47ae-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b47ae-117">Request headers</span></span>

| <span data-ttu-id="b47ae-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b47ae-118">Name</span></span>          | <span data-ttu-id="b47ae-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b47ae-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b47ae-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b47ae-120">Authorization</span></span> | <span data-ttu-id="b47ae-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="b47ae-121">Bearer \{token\}.</span></span> <span data-ttu-id="b47ae-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="b47ae-122">Required.</span></span> |
| <span data-ttu-id="b47ae-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b47ae-123">Content-Type</span></span>  | <span data-ttu-id="b47ae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b47ae-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b47ae-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b47ae-125">Request body</span></span>

<span data-ttu-id="b47ae-126">В тексте запроса добавьте представление объекта [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b47ae-126">In the request body, supply a JSON representation of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b47ae-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b47ae-127">Response</span></span>

<span data-ttu-id="b47ae-128">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b47ae-128">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b47ae-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="b47ae-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b47ae-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b47ae-130">Request</span></span>

<span data-ttu-id="b47ae-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b47ae-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator",
  "isEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="b47ae-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b47ae-132">Response</span></span>

<span data-ttu-id="b47ae-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b47ae-133">The following is an example of the response.</span></span>

> <span data-ttu-id="b47ae-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b47ae-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "4c02f928-7752-49aa-8fc8-e286d973a965",
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
