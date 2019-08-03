---
title: Удаление Едукатионрубрик
description: Удаление объекта Едукатионрубрик.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f54816be7872734ecbd6d8a0b46a8a57694b4c68
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173155"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="72161-103">Удаление Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="72161-103">Delete educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72161-104">Удаление объекта [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="72161-104">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72161-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72161-105">Permissions</span></span>

<span data-ttu-id="72161-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72161-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72161-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72161-108">Permission type</span></span>                        | <span data-ttu-id="72161-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72161-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72161-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72161-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="72161-111">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72161-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="72161-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72161-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72161-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72161-113">Not supported.</span></span> |
| <span data-ttu-id="72161-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72161-114">Application</span></span>                            | <span data-ttu-id="72161-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72161-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72161-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72161-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="72161-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72161-117">Request headers</span></span>

| <span data-ttu-id="72161-118">Имя</span><span class="sxs-lookup"><span data-stu-id="72161-118">Name</span></span>          | <span data-ttu-id="72161-119">Описание</span><span class="sxs-lookup"><span data-stu-id="72161-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="72161-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72161-120">Authorization</span></span> | <span data-ttu-id="72161-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="72161-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="72161-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="72161-122">Request body</span></span>

<span data-ttu-id="72161-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72161-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72161-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="72161-124">Response</span></span>

<span data-ttu-id="72161-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="72161-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72161-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="72161-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72161-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="72161-128">Request</span></span>

<span data-ttu-id="72161-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72161-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```

### <a name="response"></a><span data-ttu-id="72161-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="72161-130">Response</span></span>

<span data-ttu-id="72161-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="72161-131">The following is an example of the response.</span></span>

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
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->