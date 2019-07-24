---
title: Удаление Онпремисесажентграуп
description: Удаление объекта **онпремисесажентграуп** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f893502156560e455dbed46a1db4e9dc6faf327
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841166"
---
# <a name="delete-onpremisesagentgroup"></a><span data-ttu-id="6e73b-103">Удаление Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="6e73b-103">Delete onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e73b-104">Удаление объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6e73b-104">Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e73b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e73b-105">Permissions</span></span>

<span data-ttu-id="6e73b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e73b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e73b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e73b-108">Permission type</span></span>                        | <span data-ttu-id="6e73b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e73b-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e73b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e73b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e73b-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6e73b-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="6e73b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e73b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e73b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e73b-113">Not supported.</span></span> |
| <span data-ttu-id="6e73b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e73b-114">Application</span></span>                            | <span data-ttu-id="6e73b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e73b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e73b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e73b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="6e73b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e73b-117">Request headers</span></span>

| <span data-ttu-id="6e73b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6e73b-118">Name</span></span>          | <span data-ttu-id="6e73b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6e73b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6e73b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e73b-120">Authorization</span></span> | <span data-ttu-id="6e73b-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6e73b-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e73b-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6e73b-122">Request body</span></span>

<span data-ttu-id="6e73b-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e73b-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e73b-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e73b-124">Response</span></span>

<span data-ttu-id="6e73b-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6e73b-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e73b-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="6e73b-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e73b-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e73b-128">Request</span></span>

<span data-ttu-id="6e73b-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e73b-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesagentgroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
```

### <a name="response"></a><span data-ttu-id="6e73b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e73b-130">Response</span></span>

<span data-ttu-id="6e73b-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6e73b-131">The following is an example of the response.</span></span>

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
  "description": "Delete onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
