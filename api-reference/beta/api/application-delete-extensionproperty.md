---
title: Удаление Екстенсионпроперти
description: Удаление Екстенсионпроперти.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2fb1102901422b8911cba29036d73d9877415f03
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936083"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="4c4e3-103">Удаление Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="4c4e3-103">Delete extensionProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c4e3-104">Удаление [екстенсионпроперти](../resources/extensionproperty.md).</span><span class="sxs-lookup"><span data-stu-id="4c4e3-104">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c4e3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c4e3-105">Permissions</span></span>

<span data-ttu-id="4c4e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c4e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c4e3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c4e3-108">Permission type</span></span>      | <span data-ttu-id="4c4e3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c4e3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c4e3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c4e3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c4e3-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c4e3-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c4e3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c4e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c4e3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c4e3-113">Not supported.</span></span>    |
|<span data-ttu-id="4c4e3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c4e3-114">Application</span></span> | <span data-ttu-id="4c4e3-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c4e3-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c4e3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c4e3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4c4e3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c4e3-117">Request headers</span></span>

| <span data-ttu-id="4c4e3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4c4e3-118">Name</span></span>       | <span data-ttu-id="4c4e3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4c4e3-119">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="4c4e3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c4e3-120">Authorization</span></span>  | <span data-ttu-id="4c4e3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c4e3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c4e3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c4e3-123">Request body</span></span>

<span data-ttu-id="4c4e3-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c4e3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c4e3-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c4e3-125">Response</span></span>

<span data-ttu-id="4c4e3-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4c4e3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c4e3-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c4e3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c4e3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c4e3-129">Request</span></span>

<span data-ttu-id="4c4e3-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c4e3-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/extensionProperties/{id}
```

### <a name="response"></a><span data-ttu-id="4c4e3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c4e3-131">Response</span></span>

<span data-ttu-id="4c4e3-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c4e3-132">The following is an example of the response.</span></span>

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
