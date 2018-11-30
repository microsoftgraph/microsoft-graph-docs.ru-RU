---
title: Удаление identityProvider
description: Удаление существующих identityProvider.
ms.openlocfilehash: ac6f8cafa72b94891a540c05c2d4e5e2f32e23c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074644"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="c89ca-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="c89ca-103">Delete identityProvider</span></span>

> <span data-ttu-id="c89ca-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c89ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c89ca-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c89ca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c89ca-106">Удаление существующих [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="c89ca-106">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c89ca-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c89ca-107">Permissions</span></span>

<span data-ttu-id="c89ca-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c89ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c89ca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c89ca-110">Permission type</span></span>      | <span data-ttu-id="c89ca-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c89ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c89ca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c89ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c89ca-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89ca-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="c89ca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c89ca-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c89ca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c89ca-115">Not supported.</span></span>|
|<span data-ttu-id="c89ca-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c89ca-116">Application</span></span>|<span data-ttu-id="c89ca-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c89ca-117">Not supported.</span></span>|

<span data-ttu-id="c89ca-118">Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="c89ca-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="c89ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c89ca-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c89ca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c89ca-120">Request headers</span></span>

|<span data-ttu-id="c89ca-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c89ca-121">Name</span></span>|<span data-ttu-id="c89ca-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c89ca-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c89ca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c89ca-123">Authorization</span></span>|<span data-ttu-id="c89ca-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c89ca-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c89ca-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c89ca-126">Request body</span></span>

<span data-ttu-id="c89ca-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c89ca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c89ca-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c89ca-128">Response</span></span>

<span data-ttu-id="c89ca-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c89ca-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c89ca-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c89ca-130">Example</span></span>

<span data-ttu-id="c89ca-131">В следующем примере удаляется **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="c89ca-131">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="c89ca-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c89ca-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="c89ca-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="c89ca-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->