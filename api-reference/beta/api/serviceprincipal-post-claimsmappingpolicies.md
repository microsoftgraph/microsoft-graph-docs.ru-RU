---
title: Назначение Клаимсмаппингполици
description: Назначьте Клаимсмаппингполици участнику службы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce7a1af7b058aa25fbeaad3df21fb8f4ed735046
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234487"
---
# <a name="assign-claimsmappingpolicy"></a><span data-ttu-id="c37e9-103">Назначение Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="c37e9-103">Assign claimsMappingPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c37e9-104">Назначьте [клаимсмаппингполици](../resources/claimsmappingpolicy.md) для [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="c37e9-104">Assign a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c37e9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c37e9-105">Permissions</span></span>

<span data-ttu-id="c37e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c37e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c37e9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c37e9-108">Permission type</span></span>                        | <span data-ttu-id="c37e9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c37e9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c37e9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c37e9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c37e9-111">Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c37e9-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="c37e9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c37e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c37e9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c37e9-113">Not supported.</span></span> |
| <span data-ttu-id="c37e9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c37e9-114">Application</span></span>                            | <span data-ttu-id="c37e9-115">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c37e9-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c37e9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c37e9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/claimsMappingPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c37e9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c37e9-117">Request headers</span></span>

| <span data-ttu-id="c37e9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c37e9-118">Name</span></span>          | <span data-ttu-id="c37e9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c37e9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c37e9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c37e9-120">Authorization</span></span> | <span data-ttu-id="c37e9-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c37e9-121">Bearer {token}</span></span> |
| <span data-ttu-id="c37e9-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c37e9-122">Content-Type</span></span> | <span data-ttu-id="c37e9-123">application/json</span><span class="sxs-lookup"><span data-stu-id="c37e9-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c37e9-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c37e9-124">Request body</span></span>

<span data-ttu-id="c37e9-125">В тексте запроса укажите идентификатор объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) (с помощью `@odata.id` свойства), который должен быть назначен субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="c37e9-125">In the request body, supply the identifier of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="c37e9-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c37e9-126">Response</span></span>

<span data-ttu-id="c37e9-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c37e9-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c37e9-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c37e9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c37e9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c37e9-130">Request</span></span>

<span data-ttu-id="c37e9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c37e9-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```

### <a name="response"></a><span data-ttu-id="c37e9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c37e9-132">Response</span></span>

<span data-ttu-id="c37e9-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c37e9-133">The following is an example of the response.</span></span>

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
  "description": "Assign claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->