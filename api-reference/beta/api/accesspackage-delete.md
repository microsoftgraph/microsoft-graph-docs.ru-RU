---
title: Удаление Акцесспаккаже
description: Удаление Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 05d4261f6a2fb6d786dfcb56214f11adec3ab7c0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936079"
---
# <a name="delete-accesspackage"></a><span data-ttu-id="27287-103">Удаление Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="27287-103">Delete accessPackage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27287-104">Удаление объекта [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="27287-104">Delete an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27287-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27287-105">Permissions</span></span>

<span data-ttu-id="27287-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27287-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27287-108">Permission type</span></span>                        | <span data-ttu-id="27287-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27287-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27287-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27287-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="27287-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="27287-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="27287-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27287-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27287-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27287-113">Not supported.</span></span> |
| <span data-ttu-id="27287-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27287-114">Application</span></span>                            | <span data-ttu-id="27287-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27287-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27287-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27287-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}

```

## <a name="request-headers"></a><span data-ttu-id="27287-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27287-117">Request headers</span></span>

| <span data-ttu-id="27287-118">Имя</span><span class="sxs-lookup"><span data-stu-id="27287-118">Name</span></span>          | <span data-ttu-id="27287-119">Описание</span><span class="sxs-lookup"><span data-stu-id="27287-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="27287-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="27287-120">Authorization</span></span> | <span data-ttu-id="27287-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="27287-121">Bearer \{token\}.</span></span> <span data-ttu-id="27287-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="27287-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27287-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27287-123">Request body</span></span>

<span data-ttu-id="27287-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27287-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27287-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="27287-125">Response</span></span>

<span data-ttu-id="27287-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="27287-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27287-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="27287-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27287-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="27287-129">Request</span></span>

<span data-ttu-id="27287-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27287-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accesspackage"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```

### <a name="response"></a><span data-ttu-id="27287-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="27287-131">Response</span></span>

<span data-ttu-id="27287-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="27287-132">The following is an example of the response.</span></span>

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
  "description": "Delete accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
