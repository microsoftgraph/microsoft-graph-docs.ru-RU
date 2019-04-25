---
title: Получение identityProvider
description: Получение свойств существующего объекта identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc06d4f8dcab8bf07d2dc0a9ff8130b305b8217c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577709"
---
# <a name="get-identityprovider"></a><span data-ttu-id="8d713-103">Получение identityProvider</span><span class="sxs-lookup"><span data-stu-id="8d713-103">Get identityProvider</span></span>

<span data-ttu-id="8d713-104">Получение свойств существующего объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="8d713-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d713-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d713-105">Permissions</span></span>

<span data-ttu-id="8d713-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d713-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d713-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d713-108">Permission type</span></span>      | <span data-ttu-id="8d713-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d713-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d713-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d713-110">Delegated (work or school account)</span></span>|<span data-ttu-id="8d713-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d713-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="8d713-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d713-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8d713-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d713-113">Not supported.</span></span>|
|<span data-ttu-id="8d713-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d713-114">Application</span></span>|<span data-ttu-id="8d713-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d713-115">Not supported.</span></span>|

<span data-ttu-id="8d713-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="8d713-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="8d713-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d713-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8d713-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d713-118">Request headers</span></span>

|<span data-ttu-id="8d713-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8d713-119">Name</span></span>|<span data-ttu-id="8d713-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8d713-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8d713-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d713-121">Authorization</span></span>|<span data-ttu-id="8d713-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d713-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d713-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d713-124">Request body</span></span>

<span data-ttu-id="8d713-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d713-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d713-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d713-126">Response</span></span>

<span data-ttu-id="8d713-127">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и представление объекта [identityProvider](../resources/identityProvider.md) в формате JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d713-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityProvider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d713-128">Пример</span><span class="sxs-lookup"><span data-stu-id="8d713-128">Example</span></span>

<span data-ttu-id="8d713-129">В приведенном ниже примере возвращается определенный объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="8d713-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="8d713-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d713-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="8d713-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d713-131">Response</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
