---
title: Получение identityProvider
description: Извлечение свойств существующего identityProvider.
localization_priority: Normal
ms.openlocfilehash: f0d467bde092f84d092dbcee7c54c01e3ef849f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812973"
---
# <a name="get-identityprovider"></a><span data-ttu-id="1dafc-103">Получение identityProvider</span><span class="sxs-lookup"><span data-stu-id="1dafc-103">Get identityProvider</span></span>

> <span data-ttu-id="1dafc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1dafc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1dafc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dafc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1dafc-106">Извлечение свойств существующего [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="1dafc-106">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1dafc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1dafc-107">Permissions</span></span>

<span data-ttu-id="1dafc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dafc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dafc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dafc-110">Permission type</span></span>      | <span data-ttu-id="1dafc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dafc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dafc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dafc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1dafc-113">IdentityProvider.Read.All IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dafc-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="1dafc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dafc-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1dafc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dafc-115">Not supported.</span></span>|
|<span data-ttu-id="1dafc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dafc-116">Application</span></span>|<span data-ttu-id="1dafc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dafc-117">Not supported.</span></span>|

<span data-ttu-id="1dafc-118">Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="1dafc-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="1dafc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dafc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1dafc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dafc-120">Request headers</span></span>

|<span data-ttu-id="1dafc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1dafc-121">Name</span></span>|<span data-ttu-id="1dafc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1dafc-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1dafc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dafc-123">Authorization</span></span>|<span data-ttu-id="1dafc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dafc-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dafc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1dafc-126">Request body</span></span>

<span data-ttu-id="1dafc-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1dafc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dafc-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="1dafc-128">Response</span></span>

<span data-ttu-id="1dafc-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и представление JSON [identityProvider](../resources/identityprovider.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1dafc-129">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dafc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1dafc-130">Example</span></span>

<span data-ttu-id="1dafc-131">В следующем примере извлекается определенных **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="1dafc-131">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="1dafc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dafc-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="1dafc-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="1dafc-133">Response</span></span>

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
