---
title: Обновление Идентитисекуритидефаултсенфорцементполици
description: Обновление свойств объекта Идентитисекуритидефаултсенфорцементполици.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 653397a076e930ac38119c99703db97157b84ccb
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556277"
---
# <a name="update-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="72e11-103">Обновление Идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="72e11-103">Update identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="72e11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72e11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72e11-105">Обновление свойств объекта [идентитисекуритидефаултсенфорцементполици](../resources/identitysecuritydefaultsenforcementpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="72e11-105">Update the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72e11-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72e11-106">Permissions</span></span>

<span data-ttu-id="72e11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72e11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72e11-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72e11-109">Permission type</span></span>                        | <span data-ttu-id="72e11-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72e11-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72e11-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72e11-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72e11-112">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="72e11-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="72e11-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72e11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72e11-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72e11-114">Not supported.</span></span> |
| <span data-ttu-id="72e11-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="72e11-115">Application</span></span>                            | <span data-ttu-id="72e11-116">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="72e11-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="72e11-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72e11-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="request-headers"></a><span data-ttu-id="72e11-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72e11-118">Request headers</span></span>

| <span data-ttu-id="72e11-119">Имя</span><span class="sxs-lookup"><span data-stu-id="72e11-119">Name</span></span>       | <span data-ttu-id="72e11-120">Описание</span><span class="sxs-lookup"><span data-stu-id="72e11-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="72e11-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72e11-121">Authorization</span></span> | <span data-ttu-id="72e11-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72e11-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72e11-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72e11-124">Content-type</span></span> | <span data-ttu-id="72e11-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72e11-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72e11-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72e11-127">Request body</span></span>

<span data-ttu-id="72e11-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="72e11-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="72e11-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="72e11-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="72e11-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="72e11-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="72e11-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="72e11-131">Property</span></span>     | <span data-ttu-id="72e11-132">Тип</span><span class="sxs-lookup"><span data-stu-id="72e11-132">Type</span></span>        | <span data-ttu-id="72e11-133">Описание</span><span class="sxs-lookup"><span data-stu-id="72e11-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="72e11-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="72e11-134">isEnabled</span></span>|<span data-ttu-id="72e11-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="72e11-135">Boolean</span></span>|<span data-ttu-id="72e11-136">Если задано значение true, по умолчанию для клиента будет включен параметр безопасности Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="72e11-136">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="response"></a><span data-ttu-id="72e11-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="72e11-137">Response</span></span>

<span data-ttu-id="72e11-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="72e11-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72e11-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="72e11-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72e11-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="72e11-141">Request</span></span>

<span data-ttu-id="72e11-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72e11-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72e11-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="72e11-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identitysecuritydefaultsenforcementpolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/identitySecurityDefaultsEnforcementPolicy
Content-type: application/json

{
  "isEnabled": false
}
```
# <a name="c"></a>[<span data-ttu-id="72e11-144">C#</span><span class="sxs-lookup"><span data-stu-id="72e11-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identitysecuritydefaultsenforcementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72e11-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72e11-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identitysecuritydefaultsenforcementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72e11-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72e11-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identitysecuritydefaultsenforcementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="72e11-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="72e11-147">Response</span></span>

<span data-ttu-id="72e11-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="72e11-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
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
