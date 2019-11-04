---
title: Создание Акцесспаккаже
description: Создание нового Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 06d6c92ed227b03d1adf069e1fc8dd76e9658622
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936071"
---
# <a name="create-accesspackage"></a><span data-ttu-id="97f23-103">Создание Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="97f23-103">Create accessPackage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97f23-104">Создание нового объекта [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="97f23-104">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97f23-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97f23-105">Permissions</span></span>

<span data-ttu-id="97f23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97f23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97f23-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97f23-108">Permission type</span></span>                        | <span data-ttu-id="97f23-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97f23-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="97f23-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97f23-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="97f23-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="97f23-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="97f23-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97f23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97f23-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97f23-113">Not supported.</span></span> |
| <span data-ttu-id="97f23-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97f23-114">Application</span></span>                            | <span data-ttu-id="97f23-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97f23-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97f23-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97f23-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="97f23-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97f23-117">Request headers</span></span>

| <span data-ttu-id="97f23-118">Имя</span><span class="sxs-lookup"><span data-stu-id="97f23-118">Name</span></span>          | <span data-ttu-id="97f23-119">Описание</span><span class="sxs-lookup"><span data-stu-id="97f23-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="97f23-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="97f23-120">Authorization</span></span> | <span data-ttu-id="97f23-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="97f23-121">Bearer \{token\}.</span></span> <span data-ttu-id="97f23-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="97f23-122">Required.</span></span> |
| <span data-ttu-id="97f23-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97f23-123">Content-Type</span></span>  | <span data-ttu-id="97f23-124">application/json</span><span class="sxs-lookup"><span data-stu-id="97f23-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97f23-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97f23-125">Request body</span></span>

<span data-ttu-id="97f23-126">В тексте запроса добавьте представление объекта [акцесспаккаже](../resources/accesspackage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97f23-126">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="97f23-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="97f23-127">Response</span></span>

<span data-ttu-id="97f23-128">В случае успешного выполнения этот метод возвращает код отклика 201, созданный в теле отклика, и новый объект [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="97f23-128">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="97f23-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="97f23-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97f23-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="97f23-130">Request</span></span>

<span data-ttu-id="97f23-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97f23-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_accesspackage_from_accesspackages"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives"
}
```

### <a name="response"></a><span data-ttu-id="97f23-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="97f23-132">Response</span></span>

<span data-ttu-id="97f23-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97f23-133">The following is an example of the response.</span></span>

> <span data-ttu-id="97f23-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97f23-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "isRoleScopesVisible": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
