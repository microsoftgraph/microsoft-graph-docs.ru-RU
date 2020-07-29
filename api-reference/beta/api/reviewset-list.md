---
title: Список Ревиевсетс
description: Получение списка объектов reviewing для объекта Едисковерикасе.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0543a29273973e1b63735558d27998b68b1bcd25
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510198"
---
# <a name="list-reviewsets"></a><span data-ttu-id="d341f-103">Список Ревиевсетс</span><span class="sxs-lookup"><span data-stu-id="d341f-103">List reviewSets</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d341f-104">Получение списка объектов [reviewing](../resources/reviewset.md) для объекта [едисковерикасе](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="d341f-104">Retrieve the list of [reviewSet](../resources/reviewset.md) objects in an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d341f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d341f-105">Permissions</span></span>

<span data-ttu-id="d341f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d341f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d341f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d341f-108">Permission type</span></span>                        | <span data-ttu-id="d341f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d341f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d341f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d341f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d341f-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="d341f-111">User.Read</span></span> |
| <span data-ttu-id="d341f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d341f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d341f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d341f-113">Not supported.</span></span> |
| <span data-ttu-id="d341f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d341f-114">Application</span></span>                            | <span data-ttu-id="d341f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d341f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d341f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d341f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets
```

## <a name="request-headers"></a><span data-ttu-id="d341f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d341f-117">Request headers</span></span>

| <span data-ttu-id="d341f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d341f-118">Name</span></span>          | <span data-ttu-id="d341f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d341f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d341f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d341f-120">Authorization</span></span> | <span data-ttu-id="d341f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d341f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d341f-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d341f-123">Request body</span></span>

<span data-ttu-id="d341f-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d341f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d341f-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d341f-125">Response</span></span>

<span data-ttu-id="d341f-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенную коллекцию [перепредставления](../resources/reviewset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d341f-126">If successful, this method returns a `200 OK` response code and the requested [reviewSet](../resources/reviewset.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d341f-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="d341f-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d341f-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="d341f-128">Request</span></span>

<span data-ttu-id="d341f-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d341f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_reviewset",
  "@odata.type": "microsoft.graph.reviewSet"
}-->

```http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets
```

### <a name="response"></a><span data-ttu-id="d341f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d341f-130">Response</span></span>

<span data-ttu-id="d341f-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d341f-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSet"
} -->

```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cases",
    "@odata.nextLink": "https://graph.microsoft.com/beta/compliance/ediscovery/cases?$skiptoken=<encodedPageToken>",
    "value": [
        {
            "id": "f6a91542-4ce7-4712-b275-c29545dd8507",
            "displayName": "My Reviewset 1",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T11:58:27.1408174Z"
        },
        {
            "id": "0d78ec4a-aa91-41ea-8da8-d68b030c168f",
            "displayName": "My Reviewset 2",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T12:03:32.2038960Z"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete reviewSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
