---
title: Удаление identityProvider
description: Удаление существующих identityProvider.
localization_priority: Normal
ms.openlocfilehash: 35689037d4f6a564ee3e1e40d18401ef793ef474
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808297"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="65f51-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="65f51-103">Delete identityProvider</span></span>

> <span data-ttu-id="65f51-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="65f51-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65f51-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65f51-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65f51-106">Удаление существующих [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="65f51-106">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65f51-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65f51-107">Permissions</span></span>

<span data-ttu-id="65f51-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65f51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65f51-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65f51-110">Permission type</span></span>      | <span data-ttu-id="65f51-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65f51-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65f51-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65f51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65f51-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65f51-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="65f51-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65f51-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="65f51-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65f51-115">Not supported.</span></span>|
|<span data-ttu-id="65f51-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65f51-116">Application</span></span>|<span data-ttu-id="65f51-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65f51-117">Not supported.</span></span>|

<span data-ttu-id="65f51-118">Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="65f51-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="65f51-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65f51-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="65f51-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65f51-120">Request headers</span></span>

|<span data-ttu-id="65f51-121">Имя</span><span class="sxs-lookup"><span data-stu-id="65f51-121">Name</span></span>|<span data-ttu-id="65f51-122">Описание</span><span class="sxs-lookup"><span data-stu-id="65f51-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="65f51-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65f51-123">Authorization</span></span>|<span data-ttu-id="65f51-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65f51-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65f51-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65f51-126">Request body</span></span>

<span data-ttu-id="65f51-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65f51-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65f51-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="65f51-128">Response</span></span>

<span data-ttu-id="65f51-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="65f51-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="65f51-130">Пример</span><span class="sxs-lookup"><span data-stu-id="65f51-130">Example</span></span>

<span data-ttu-id="65f51-131">В следующем примере удаляется **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="65f51-131">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="65f51-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="65f51-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="65f51-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="65f51-133">Response</span></span>

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
