---
title: Удаление Токенлифетимеполици
description: Удаление Токенлифетимеполици из приложения или servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 055da6eb449c8600e39755f4725ce72af35af045
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234451"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="955ab-103">Удаление Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="955ab-103">Remove tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="955ab-104">Удаление [токенлифетимеполици](../resources/tokenlifetimepolicy.md) из [приложения](../resources/application.md) или [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="955ab-104">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="955ab-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="955ab-105">Permissions</span></span>

<span data-ttu-id="955ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="955ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="955ab-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="955ab-108">Permission type</span></span>                        | <span data-ttu-id="955ab-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="955ab-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="955ab-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="955ab-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="955ab-111">Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="955ab-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="955ab-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="955ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="955ab-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955ab-113">Not supported.</span></span> |
| <span data-ttu-id="955ab-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="955ab-114">Application</span></span>                            | <span data-ttu-id="955ab-115">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="955ab-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="955ab-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="955ab-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
DELETE /servicePrincipals/{id}/tokenLifetimePolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="955ab-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="955ab-117">Request headers</span></span>

| <span data-ttu-id="955ab-118">Имя</span><span class="sxs-lookup"><span data-stu-id="955ab-118">Name</span></span>          | <span data-ttu-id="955ab-119">Описание</span><span class="sxs-lookup"><span data-stu-id="955ab-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="955ab-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="955ab-120">Authorization</span></span> | <span data-ttu-id="955ab-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="955ab-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="955ab-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="955ab-122">Request body</span></span>

<span data-ttu-id="955ab-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="955ab-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="955ab-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="955ab-124">Response</span></span>

<span data-ttu-id="955ab-125">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="955ab-125">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="955ab-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="955ab-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="955ab-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="955ab-127">Request</span></span>

<span data-ttu-id="955ab-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="955ab-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="955ab-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="955ab-129">Response</span></span>

<span data-ttu-id="955ab-130">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="955ab-130">The following is an example of the response.</span></span>

> <span data-ttu-id="955ab-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="955ab-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->