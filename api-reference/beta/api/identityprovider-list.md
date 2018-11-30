---
title: Список identityProviders
description: Извлечение всех identityProviders в каталоге.
ms.openlocfilehash: fd5662690b644bc7a34587a5bdfc519188a3d4ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080955"
---
# <a name="list-identityproviders"></a><span data-ttu-id="755e0-103">Список identityProviders</span><span class="sxs-lookup"><span data-stu-id="755e0-103">List identityProviders</span></span>

> <span data-ttu-id="755e0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="755e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="755e0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="755e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="755e0-106">Извлечение всех [identityProviders](../resources/identityprovider.md) в каталоге.</span><span class="sxs-lookup"><span data-stu-id="755e0-106">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="755e0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="755e0-107">Permissions</span></span>

<span data-ttu-id="755e0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="755e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="755e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="755e0-110">Permission type</span></span>      | <span data-ttu-id="755e0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="755e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="755e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="755e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="755e0-113">IdentityProvider.Read.All IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="755e0-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="755e0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="755e0-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="755e0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="755e0-115">Not supported.</span></span>|
|<span data-ttu-id="755e0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="755e0-116">Application</span></span>|<span data-ttu-id="755e0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="755e0-117">Not supported.</span></span>|

<span data-ttu-id="755e0-118">Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="755e0-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="755e0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="755e0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="755e0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="755e0-120">Request headers</span></span>

|<span data-ttu-id="755e0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="755e0-121">Name</span></span>|<span data-ttu-id="755e0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="755e0-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="755e0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="755e0-123">Authorization</span></span>|<span data-ttu-id="755e0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="755e0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="755e0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="755e0-126">Request body</span></span>

<span data-ttu-id="755e0-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="755e0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="755e0-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="755e0-128">Response</span></span>

<span data-ttu-id="755e0-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию [identityProviders](../resources/identityprovider.md) в представление JSON в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="755e0-129">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="755e0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="755e0-130">Example</span></span>

<span data-ttu-id="755e0-131">В следующем примере извлекаются все **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="755e0-131">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="755e0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="755e0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="755e0-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="755e0-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "Amazon-OAUTH",
        "name": "Login with Amazon",
        "type": "Amazon",
        "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
        "clientSecret": "*****"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->