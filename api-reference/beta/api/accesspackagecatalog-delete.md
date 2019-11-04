---
title: Удаление Акцесспаккажекаталог
description: Удаление Акцесспаккажекаталог.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f6ab9df54690c93453e3fd030c37978d42db7da9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936092"
---
# <a name="delete-accesspackagecatalog"></a><span data-ttu-id="b75bd-103">Удаление Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="b75bd-103">Delete accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b75bd-104">Удаление [акцесспаккажекаталог](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="b75bd-104">Delete an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b75bd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b75bd-105">Permissions</span></span>

<span data-ttu-id="b75bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b75bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b75bd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b75bd-108">Permission type</span></span>                        | <span data-ttu-id="b75bd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b75bd-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b75bd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b75bd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b75bd-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b75bd-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="b75bd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b75bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b75bd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b75bd-113">Not supported.</span></span> |
| <span data-ttu-id="b75bd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b75bd-114">Application</span></span>                            | <span data-ttu-id="b75bd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b75bd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b75bd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b75bd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b75bd-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b75bd-117">Request headers</span></span>

| <span data-ttu-id="b75bd-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b75bd-118">Name</span></span>          | <span data-ttu-id="b75bd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b75bd-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b75bd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b75bd-120">Authorization</span></span> | <span data-ttu-id="b75bd-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="b75bd-121">Bearer \{token\}.</span></span> <span data-ttu-id="b75bd-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="b75bd-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b75bd-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b75bd-123">Request body</span></span>

<span data-ttu-id="b75bd-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b75bd-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b75bd-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="b75bd-125">Response</span></span>

<span data-ttu-id="b75bd-126">В случае успешного выполнения этот метод возвращает код ответа серии 200.</span><span class="sxs-lookup"><span data-stu-id="b75bd-126">If successful, this method returns a 200-series response code.</span></span> <span data-ttu-id="b75bd-127">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b75bd-127">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b75bd-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b75bd-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b75bd-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b75bd-129">Request</span></span>

<span data-ttu-id="b75bd-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b75bd-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accesspackagecatalog"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

### <a name="response"></a><span data-ttu-id="b75bd-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b75bd-131">Response</span></span>

<span data-ttu-id="b75bd-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b75bd-132">The following is an example of the response.</span></span>

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
  "description": "Delete accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
