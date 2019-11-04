---
title: Удаление Екстенсионпроперти
description: Удаление Екстенсионпроперти.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 30d45906695e2e9bfb256f5dedf4a2108308b63d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939749"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="5ee6b-103">Удаление Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="5ee6b-103">Delete extensionProperty</span></span>

<span data-ttu-id="5ee6b-104">Удаление [екстенсионпроперти](../resources/extensionproperty.md).</span><span class="sxs-lookup"><span data-stu-id="5ee6b-104">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5ee6b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ee6b-105">Permissions</span></span>

<span data-ttu-id="5ee6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ee6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ee6b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ee6b-108">Permission type</span></span>      | <span data-ttu-id="5ee6b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ee6b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ee6b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ee6b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5ee6b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5ee6b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5ee6b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ee6b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ee6b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ee6b-113">Not supported.</span></span>    |
|<span data-ttu-id="5ee6b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ee6b-114">Application</span></span> | <span data-ttu-id="5ee6b-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee6b-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ee6b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ee6b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5ee6b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ee6b-117">Request headers</span></span>

| <span data-ttu-id="5ee6b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5ee6b-118">Name</span></span>       | <span data-ttu-id="5ee6b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5ee6b-119">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5ee6b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ee6b-120">Authorization</span></span>  | <span data-ttu-id="5ee6b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ee6b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ee6b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ee6b-123">Request body</span></span>

<span data-ttu-id="5ee6b-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ee6b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ee6b-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ee6b-125">Response</span></span>

<span data-ttu-id="5ee6b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5ee6b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ee6b-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5ee6b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ee6b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ee6b-129">Request</span></span>

<span data-ttu-id="5ee6b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ee6b-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties/{id}
```

### <a name="response"></a><span data-ttu-id="5ee6b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ee6b-131">Response</span></span>

<span data-ttu-id="5ee6b-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5ee6b-132">The following is an example of the response.</span></span>

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
  "description": "Delete extensionProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
