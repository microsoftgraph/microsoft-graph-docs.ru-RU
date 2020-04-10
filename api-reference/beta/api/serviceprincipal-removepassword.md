---
title: 'servicePrincipal: Ремовепассворд'
description: Удаление пароля из servicePrincipal
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a4c68e934fb6ea3085c5dd268371e9f5763519c9
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218614"
---
# <a name="serviceprincipal-removepassword"></a><span data-ttu-id="bffa1-103">servicePrincipal: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="bffa1-103">servicePrincipal: removePassword</span></span>

<span data-ttu-id="bffa1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bffa1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bffa1-105">Удаление пароля из объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="bffa1-105">Remove a password from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bffa1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bffa1-106">Permissions</span></span>

<span data-ttu-id="bffa1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bffa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bffa1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bffa1-109">Permission type</span></span>                        | <span data-ttu-id="bffa1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bffa1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bffa1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bffa1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bffa1-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bffa1-112">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="bffa1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bffa1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bffa1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bffa1-114">Not supported.</span></span> |
| <span data-ttu-id="bffa1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bffa1-115">Application</span></span>                            | <span data-ttu-id="bffa1-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bffa1-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bffa1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bffa1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="bffa1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bffa1-118">Request headers</span></span>

| <span data-ttu-id="bffa1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bffa1-119">Name</span></span>           | <span data-ttu-id="bffa1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bffa1-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="bffa1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bffa1-121">Authorization</span></span>  | <span data-ttu-id="bffa1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bffa1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bffa1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bffa1-124">Content-type</span></span>   | <span data-ttu-id="bffa1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bffa1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bffa1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bffa1-127">Request body</span></span>

| <span data-ttu-id="bffa1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bffa1-128">Property</span></span>     | <span data-ttu-id="bffa1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bffa1-129">Type</span></span>   |<span data-ttu-id="bffa1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bffa1-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bffa1-131">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="bffa1-131">keyId</span></span> | <span data-ttu-id="bffa1-132">GUID</span><span class="sxs-lookup"><span data-stu-id="bffa1-132">GUID</span></span> | <span data-ttu-id="bffa1-133">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="bffa1-133">The unique identifier for the password.</span></span> <span data-ttu-id="bffa1-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bffa1-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bffa1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bffa1-135">Response</span></span>

<span data-ttu-id="bffa1-136">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="bffa1-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bffa1-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="bffa1-137">Examples</span></span>

<span data-ttu-id="bffa1-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="bffa1-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="bffa1-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bffa1-139">Request</span></span>

<span data-ttu-id="bffa1-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bffa1-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bffa1-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bffa1-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_removepassword"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="javascript"></a>[<span data-ttu-id="bffa1-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bffa1-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bffa1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bffa1-143">Response</span></span>

<span data-ttu-id="bffa1-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bffa1-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
