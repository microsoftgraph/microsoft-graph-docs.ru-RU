---
title: Обновление tokenIssuancePolicy
description: Обновление свойств объекта tokenIssuancePolicy.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: de3f0962e3b988f758ee6e8a2f64a4032251a92f
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910842"
---
# <a name="update-tokenissuancepolicy"></a><span data-ttu-id="a2eb8-103">Обновление tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="a2eb8-103">Update tokenIssuancePolicy</span></span>

<span data-ttu-id="a2eb8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2eb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2eb8-105">Обновление свойств объекта [tokenIssuancePolicy.](../resources/tokenIssuancePolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2eb8-105">Update the properties of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2eb8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2eb8-106">Permissions</span></span>

<span data-ttu-id="a2eb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2eb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2eb8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2eb8-109">Permission type</span></span>                        | <span data-ttu-id="a2eb8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2eb8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a2eb8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2eb8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2eb8-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2eb8-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="a2eb8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2eb8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2eb8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-114">Not supported.</span></span> |
| <span data-ttu-id="a2eb8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a2eb8-115">Application</span></span>                            | <span data-ttu-id="a2eb8-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2eb8-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2eb8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2eb8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a2eb8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2eb8-118">Request headers</span></span>

| <span data-ttu-id="a2eb8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a2eb8-119">Name</span></span>       | <span data-ttu-id="a2eb8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a2eb8-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a2eb8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2eb8-121">Authorization</span></span> | <span data-ttu-id="a2eb8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2eb8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2eb8-124">Content-type</span></span> | <span data-ttu-id="a2eb8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2eb8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2eb8-127">Request body</span></span>

<span data-ttu-id="a2eb8-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a2eb8-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a2eb8-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a2eb8-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2eb8-131">Property</span></span>     | <span data-ttu-id="a2eb8-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a2eb8-132">Type</span></span>        | <span data-ttu-id="a2eb8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a2eb8-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2eb8-134">definition</span><span class="sxs-lookup"><span data-stu-id="a2eb8-134">definition</span></span>|<span data-ttu-id="a2eb8-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a2eb8-135">String collection</span></span>| <span data-ttu-id="a2eb8-136">Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="a2eb8-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-137">Required.</span></span>|
|<span data-ttu-id="a2eb8-138">description</span><span class="sxs-lookup"><span data-stu-id="a2eb8-138">description</span></span>|<span data-ttu-id="a2eb8-139">String</span><span class="sxs-lookup"><span data-stu-id="a2eb8-139">String</span></span>| <span data-ttu-id="a2eb8-140">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-140">Description for this policy.</span></span>|
|<span data-ttu-id="a2eb8-141">displayName</span><span class="sxs-lookup"><span data-stu-id="a2eb8-141">displayName</span></span>|<span data-ttu-id="a2eb8-142">String</span><span class="sxs-lookup"><span data-stu-id="a2eb8-142">String</span></span>| <span data-ttu-id="a2eb8-143">Отображаемого имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-143">Display name for this policy.</span></span> <span data-ttu-id="a2eb8-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-144">Required.</span></span>|
|<span data-ttu-id="a2eb8-145">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="a2eb8-145">isOrganizationDefault</span></span>|<span data-ttu-id="a2eb8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2eb8-146">Boolean</span></span>|<span data-ttu-id="a2eb8-147">Если установлено true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-147">If set to true, activates this policy.</span></span> <span data-ttu-id="a2eb8-148">Для одного типа политики может быть несколько политик, но только одна может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="a2eb8-149">Необязательный, значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="a2eb8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2eb8-150">Response</span></span>

<span data-ttu-id="a2eb8-p108">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2eb8-153">Пример</span><span class="sxs-lookup"><span data-stu-id="a2eb8-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2eb8-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2eb8-154">Request</span></span>

<span data-ttu-id="a2eb8-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2eb8-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2eb8-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tokenissuancepolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="a2eb8-157">C#</span><span class="sxs-lookup"><span data-stu-id="a2eb8-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2eb8-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2eb8-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2eb8-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2eb8-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2eb8-160">Java</span><span class="sxs-lookup"><span data-stu-id="a2eb8-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tokenissuancepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="a2eb8-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2eb8-161">Response</span></span>

<span data-ttu-id="a2eb8-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-162">The following is an example of the response.</span></span>

> <span data-ttu-id="a2eb8-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2eb8-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
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
  "description": "Update tokenissuancepolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


