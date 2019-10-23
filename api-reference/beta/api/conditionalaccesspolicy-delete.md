---
title: Удаление Кондитионалакцессполици
description: Удаление объекта Кондитионалакцессполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 97f9741040f2aa858b0c3d02116e780201830e3b
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638416"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="a48ce-103">Удаление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="a48ce-103">Delete conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a48ce-104">Удаление объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="a48ce-104">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a48ce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a48ce-105">Permissions</span></span>

<span data-ttu-id="a48ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a48ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a48ce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a48ce-108">Permission type</span></span>                        | <span data-ttu-id="a48ce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a48ce-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="a48ce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a48ce-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a48ce-111">Policy. ReadWrite. Кондитионалакцесс и Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="a48ce-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a48ce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a48ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a48ce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a48ce-113">Not supported.</span></span> |
|<span data-ttu-id="a48ce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a48ce-114">Application</span></span>                            | <span data-ttu-id="a48ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a48ce-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="a48ce-116">Этот API требует нескольких разрешений.</span><span class="sxs-lookup"><span data-stu-id="a48ce-116">This API requires multiple permissions.</span></span> <span data-ttu-id="a48ce-117">Подробнее: [Известные проблемы](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="a48ce-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="a48ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a48ce-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a48ce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a48ce-119">Request headers</span></span>

| <span data-ttu-id="a48ce-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a48ce-120">Name</span></span>          | <span data-ttu-id="a48ce-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a48ce-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a48ce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a48ce-122">Authorization</span></span> | <span data-ttu-id="a48ce-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a48ce-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a48ce-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a48ce-125">Request body</span></span>

<span data-ttu-id="a48ce-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a48ce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a48ce-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a48ce-127">Response</span></span>

<span data-ttu-id="a48ce-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a48ce-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a48ce-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a48ce-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a48ce-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a48ce-131">Request</span></span>

<span data-ttu-id="a48ce-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a48ce-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
```

### <a name="response"></a><span data-ttu-id="a48ce-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a48ce-133">Response</span></span>

<span data-ttu-id="a48ce-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a48ce-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
