---
title: Обновление identitySecurityDefaultsEnforcementPolicy
description: Обновление свойств объекта identitySecurityDefaultsEnforcementPolicy.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 110c74817316f9fb88b4f343b85d61b81ef9a726
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783619"
---
# <a name="update-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="54731-103">Обновление identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="54731-103">Update identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="54731-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54731-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54731-105">Обновление свойств объекта [identitySecurityDefaultsEnforcementPolicy.](../resources/identitysecuritydefaultsenforcementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="54731-105">Update the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="54731-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54731-106">Permissions</span></span>

<span data-ttu-id="54731-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54731-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54731-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54731-109">Permission type</span></span>                        | <span data-ttu-id="54731-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54731-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54731-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54731-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54731-112">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="54731-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="54731-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54731-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54731-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54731-114">Not supported.</span></span> |
| <span data-ttu-id="54731-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54731-115">Application</span></span>                            | <span data-ttu-id="54731-116">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="54731-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="54731-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54731-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="request-headers"></a><span data-ttu-id="54731-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54731-118">Request headers</span></span>

| <span data-ttu-id="54731-119">Имя</span><span class="sxs-lookup"><span data-stu-id="54731-119">Name</span></span>       | <span data-ttu-id="54731-120">Описание</span><span class="sxs-lookup"><span data-stu-id="54731-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="54731-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54731-121">Authorization</span></span> | <span data-ttu-id="54731-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54731-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54731-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54731-124">Content-type</span></span> | <span data-ttu-id="54731-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54731-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54731-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54731-127">Request body</span></span>

<span data-ttu-id="54731-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="54731-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="54731-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="54731-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="54731-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="54731-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="54731-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="54731-131">Property</span></span>     | <span data-ttu-id="54731-132">Тип</span><span class="sxs-lookup"><span data-stu-id="54731-132">Type</span></span>        | <span data-ttu-id="54731-133">Описание</span><span class="sxs-lookup"><span data-stu-id="54731-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="54731-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="54731-134">isEnabled</span></span>|<span data-ttu-id="54731-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="54731-135">Boolean</span></span>|<span data-ttu-id="54731-136">Если установлено значение true, Azure Active Directory по умолчанию для клиента включена безопасность.</span><span class="sxs-lookup"><span data-stu-id="54731-136">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="response"></a><span data-ttu-id="54731-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="54731-137">Response</span></span>

<span data-ttu-id="54731-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="54731-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54731-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="54731-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54731-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="54731-141">Request</span></span>

<span data-ttu-id="54731-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54731-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="54731-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="54731-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identitysecuritydefaultsenforcementpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/identitySecurityDefaultsEnforcementPolicy
Content-type: application/json

{
  "isEnabled": false
}
```
# <a name="c"></a>[<span data-ttu-id="54731-144">C#</span><span class="sxs-lookup"><span data-stu-id="54731-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identitysecuritydefaultsenforcementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54731-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54731-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identitysecuritydefaultsenforcementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54731-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54731-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identitysecuritydefaultsenforcementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54731-147">Java</span><span class="sxs-lookup"><span data-stu-id="54731-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identitysecuritydefaultsenforcementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="54731-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="54731-148">Response</span></span>

<span data-ttu-id="54731-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54731-149">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update identitysecuritydefaultsenforcementpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

