---
title: Update claimsmappingpolicy
description: Обновление свойств объекта claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ce110a2e3f6daaecbf7c7965ab1bf8b561147127
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434764"
---
# <a name="update-claimsmappingpolicy"></a><span data-ttu-id="8d806-103">Update claimsmappingpolicy</span><span class="sxs-lookup"><span data-stu-id="8d806-103">Update claimsmappingpolicy</span></span>

<span data-ttu-id="8d806-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d806-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d806-105">Обновление свойств объекта [claimsMappingPolicy.](../resources/claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8d806-105">Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d806-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d806-106">Permissions</span></span>

<span data-ttu-id="8d806-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d806-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d806-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d806-109">Permission type</span></span>                        | <span data-ttu-id="8d806-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d806-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8d806-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d806-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d806-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d806-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8d806-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d806-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d806-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d806-114">Not supported.</span></span> |
| <span data-ttu-id="8d806-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d806-115">Application</span></span>                            | <span data-ttu-id="8d806-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d806-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d806-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d806-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8d806-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d806-118">Request headers</span></span>

| <span data-ttu-id="8d806-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8d806-119">Name</span></span>       | <span data-ttu-id="8d806-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8d806-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8d806-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d806-121">Authorization</span></span> | <span data-ttu-id="8d806-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8d806-122">Bearer {token}</span></span> |
| <span data-ttu-id="8d806-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d806-123">Content-type</span></span> | <span data-ttu-id="8d806-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8d806-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d806-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d806-125">Request body</span></span>

<span data-ttu-id="8d806-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8d806-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8d806-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8d806-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8d806-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8d806-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8d806-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d806-129">Property</span></span>     | <span data-ttu-id="8d806-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8d806-130">Type</span></span>        | <span data-ttu-id="8d806-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8d806-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d806-132">определение</span><span class="sxs-lookup"><span data-stu-id="8d806-132">definition</span></span>|<span data-ttu-id="8d806-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d806-133">String collection</span></span>| <span data-ttu-id="8d806-134">Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики.</span><span class="sxs-lookup"><span data-stu-id="8d806-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="8d806-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d806-135">Required.</span></span>|
|<span data-ttu-id="8d806-136">description</span><span class="sxs-lookup"><span data-stu-id="8d806-136">description</span></span>|<span data-ttu-id="8d806-137">String</span><span class="sxs-lookup"><span data-stu-id="8d806-137">String</span></span>| <span data-ttu-id="8d806-138">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="8d806-138">Description for this policy.</span></span>|
|<span data-ttu-id="8d806-139">displayName</span><span class="sxs-lookup"><span data-stu-id="8d806-139">displayName</span></span>|<span data-ttu-id="8d806-140">String</span><span class="sxs-lookup"><span data-stu-id="8d806-140">String</span></span>| <span data-ttu-id="8d806-141">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8d806-141">Display name for this policy.</span></span> <span data-ttu-id="8d806-142">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8d806-142">Required.</span></span>|
|<span data-ttu-id="8d806-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="8d806-143">isOrganizationDefault</span></span>|<span data-ttu-id="8d806-144">Логический</span><span class="sxs-lookup"><span data-stu-id="8d806-144">Boolean</span></span>|<span data-ttu-id="8d806-145">Если заданной для true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="8d806-145">If set to true, activates this policy.</span></span> <span data-ttu-id="8d806-146">Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации.</span><span class="sxs-lookup"><span data-stu-id="8d806-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="8d806-147">Необязательный, значение по умолчанию является ложным.</span><span class="sxs-lookup"><span data-stu-id="8d806-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="8d806-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d806-148">Response</span></span>

<span data-ttu-id="8d806-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d806-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d806-151">Пример</span><span class="sxs-lookup"><span data-stu-id="8d806-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d806-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d806-152">Request</span></span>

<span data-ttu-id="8d806-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d806-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d806-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d806-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_claimsmappingpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="8d806-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d806-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d806-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d806-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d806-157">Java</span><span class="sxs-lookup"><span data-stu-id="8d806-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8d806-158">C#</span><span class="sxs-lookup"><span data-stu-id="8d806-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d806-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d806-159">Response</span></span>

<span data-ttu-id="8d806-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8d806-160">The following is an example of the response.</span></span>

> <span data-ttu-id="8d806-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d806-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
} -->

```http
HTTP/1.1 204 No Content
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update claimsmappingpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

