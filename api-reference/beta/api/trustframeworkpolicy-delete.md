---
title: Удаление Трустфрамеворкполици
description: Эта операция удаляет существующий объект Трустфрамеворкполици из клиента Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9bc62bdcda19038a24441fccfe01fac9705d1344
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637439"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="82c9b-103">Удаление Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="82c9b-103">Delete trustFrameworkPolicy</span></span>

> <span data-ttu-id="82c9b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="82c9b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82c9b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82c9b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82c9b-106">Удаление существующего [трустфрамеворкполици](../resources/trustframeworkpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="82c9b-106">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="82c9b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82c9b-107">Permissions</span></span>

<span data-ttu-id="82c9b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="82c9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="82c9b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82c9b-110">Permission type</span></span>      | <span data-ttu-id="82c9b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82c9b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82c9b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82c9b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82c9b-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="82c9b-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="82c9b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82c9b-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="82c9b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82c9b-115">Not supported.</span></span>|
|<span data-ttu-id="82c9b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82c9b-116">Application</span></span>|<span data-ttu-id="82c9b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82c9b-117">Not supported.</span></span>|

<span data-ttu-id="82c9b-118">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="82c9b-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="82c9b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82c9b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="82c9b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82c9b-120">Request headers</span></span>

|<span data-ttu-id="82c9b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="82c9b-121">Name</span></span>|<span data-ttu-id="82c9b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="82c9b-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="82c9b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82c9b-123">Authorization</span></span>|<span data-ttu-id="82c9b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82c9b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82c9b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82c9b-126">Request body</span></span>

<span data-ttu-id="82c9b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82c9b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82c9b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="82c9b-128">Response</span></span>

<span data-ttu-id="82c9b-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="82c9b-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82c9b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="82c9b-130">Example</span></span>

<span data-ttu-id="82c9b-131">В следующем примере удаляется объект **трустфрамеворкполици**.</span><span class="sxs-lookup"><span data-stu-id="82c9b-131">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="82c9b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="82c9b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```

##### <a name="response"></a><span data-ttu-id="82c9b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="82c9b-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="82c9b-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="82c9b-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="82c9b-135">Языках</span><span class="sxs-lookup"><span data-stu-id="82c9b-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_trustFrameworkPolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82c9b-136">Язык</span><span class="sxs-lookup"><span data-stu-id="82c9b-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_trustFrameworkPolicy-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/trustframeworkpolicy-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/trustframeworkpolicy-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
