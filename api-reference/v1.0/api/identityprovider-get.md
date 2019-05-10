---
title: Получение identityProvider
description: Получение свойств существующего объекта identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a666f9f578ab945c268646f898ec107194fb8016
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613434"
---
# <a name="get-identityprovider"></a><span data-ttu-id="9509d-103">Получение identityProvider</span><span class="sxs-lookup"><span data-stu-id="9509d-103">Get identityProvider</span></span>

<span data-ttu-id="9509d-104">Получение свойств существующего объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="9509d-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9509d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9509d-105">Permissions</span></span>

<span data-ttu-id="9509d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9509d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9509d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9509d-108">Permission type</span></span>      | <span data-ttu-id="9509d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9509d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9509d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9509d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9509d-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9509d-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="9509d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9509d-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9509d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9509d-113">Not supported.</span></span>|
|<span data-ttu-id="9509d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9509d-114">Application</span></span>|<span data-ttu-id="9509d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9509d-115">Not supported.</span></span>|

<span data-ttu-id="9509d-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="9509d-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="9509d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9509d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9509d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9509d-118">Request headers</span></span>

|<span data-ttu-id="9509d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9509d-119">Name</span></span>|<span data-ttu-id="9509d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9509d-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9509d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9509d-121">Authorization</span></span>|<span data-ttu-id="9509d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9509d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9509d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9509d-124">Request body</span></span>

<span data-ttu-id="9509d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9509d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9509d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9509d-126">Response</span></span>

<span data-ttu-id="9509d-127">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и представление объекта [identityProvider](../resources/identityProvider.md) в формате JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9509d-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityProvider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9509d-128">Пример</span><span class="sxs-lookup"><span data-stu-id="9509d-128">Example</span></span>

<span data-ttu-id="9509d-129">В приведенном ниже примере возвращается определенный объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="9509d-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="9509d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9509d-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="9509d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9509d-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9509d-132">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="9509d-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9509d-133">C#</span><span class="sxs-lookup"><span data-stu-id="9509d-133">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-identityprovider-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9509d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9509d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-identityprovider-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
