---
title: Удаление identityProvider
description: Удаление существующего объекта identityProvider.
localization_priority: Normal
ms.openlocfilehash: 7a6da4d841fec8b025fee2b3a9455a01894a0fac
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592271"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="f6f04-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="f6f04-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6f04-104">Удаление существующего объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="f6f04-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6f04-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6f04-105">Permissions</span></span>

<span data-ttu-id="f6f04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6f04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6f04-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6f04-108">Permission type</span></span>      | <span data-ttu-id="f6f04-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6f04-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6f04-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6f04-110">Delegated (work or school account)</span></span>|<span data-ttu-id="f6f04-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6f04-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="f6f04-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6f04-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f6f04-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6f04-113">Not supported.</span></span>|
|<span data-ttu-id="f6f04-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6f04-114">Application</span></span>|<span data-ttu-id="f6f04-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6f04-115">Not supported.</span></span>|

<span data-ttu-id="f6f04-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="f6f04-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f6f04-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6f04-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f6f04-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6f04-118">Request headers</span></span>

|<span data-ttu-id="f6f04-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f6f04-119">Name</span></span>|<span data-ttu-id="f6f04-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f6f04-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f6f04-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6f04-121">Authorization</span></span>|<span data-ttu-id="f6f04-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6f04-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6f04-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6f04-124">Request body</span></span>

<span data-ttu-id="f6f04-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6f04-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6f04-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6f04-126">Response</span></span>

<span data-ttu-id="f6f04-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f6f04-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f6f04-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f6f04-128">Example</span></span>

<span data-ttu-id="f6f04-129">В приведенном ниже примере удаляется объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="f6f04-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="f6f04-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6f04-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="f6f04-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6f04-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f6f04-132">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="f6f04-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f6f04-133">Языках</span><span class="sxs-lookup"><span data-stu-id="f6f04-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_identityprovider-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6f04-134">Язык</span><span class="sxs-lookup"><span data-stu-id="f6f04-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_identityprovider-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/identityprovider-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
