---
title: Обновление activitybasedtimeoutpolicy
description: Обновление свойств объекта activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f209332b18fff377c35508f856dc00f1a7b2c036
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050663"
---
# <a name="update-activitybasedtimeoutpolicy"></a><span data-ttu-id="ce699-103">Обновление activitybasedtimeoutpolicy</span><span class="sxs-lookup"><span data-stu-id="ce699-103">Update activitybasedtimeoutpolicy</span></span>

<span data-ttu-id="ce699-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce699-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ce699-105">Обновление свойств объекта [activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ce699-105">Update the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce699-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce699-106">Permissions</span></span>

<span data-ttu-id="ce699-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce699-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce699-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce699-109">Permission type</span></span>                        | <span data-ttu-id="ce699-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce699-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce699-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce699-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce699-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce699-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="ce699-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce699-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce699-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce699-114">Not supported.</span></span> |
| <span data-ttu-id="ce699-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce699-115">Application</span></span>                            | <span data-ttu-id="ce699-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce699-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce699-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce699-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ce699-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce699-118">Request headers</span></span>

| <span data-ttu-id="ce699-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ce699-119">Name</span></span>       | <span data-ttu-id="ce699-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ce699-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ce699-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce699-121">Authorization</span></span> | <span data-ttu-id="ce699-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce699-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce699-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce699-124">Content-type</span></span> | <span data-ttu-id="ce699-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce699-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce699-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce699-127">Request body</span></span>

<span data-ttu-id="ce699-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="ce699-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ce699-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="ce699-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ce699-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ce699-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ce699-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce699-131">Property</span></span>     | <span data-ttu-id="ce699-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ce699-132">Type</span></span>        | <span data-ttu-id="ce699-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ce699-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ce699-134">определение</span><span class="sxs-lookup"><span data-stu-id="ce699-134">definition</span></span>|<span data-ttu-id="ce699-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ce699-135">String collection</span></span>| <span data-ttu-id="ce699-136">Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики.</span><span class="sxs-lookup"><span data-stu-id="ce699-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="ce699-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce699-137">Required.</span></span>|
|<span data-ttu-id="ce699-138">description</span><span class="sxs-lookup"><span data-stu-id="ce699-138">description</span></span>|<span data-ttu-id="ce699-139">String</span><span class="sxs-lookup"><span data-stu-id="ce699-139">String</span></span>| <span data-ttu-id="ce699-140">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="ce699-140">Description for this policy.</span></span>|
|<span data-ttu-id="ce699-141">displayName</span><span class="sxs-lookup"><span data-stu-id="ce699-141">displayName</span></span>|<span data-ttu-id="ce699-142">String</span><span class="sxs-lookup"><span data-stu-id="ce699-142">String</span></span>| <span data-ttu-id="ce699-143">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ce699-143">Display name for this policy.</span></span> <span data-ttu-id="ce699-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce699-144">Required.</span></span>|
|<span data-ttu-id="ce699-145">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="ce699-145">isOrganizationDefault</span></span>|<span data-ttu-id="ce699-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ce699-146">Boolean</span></span>|<span data-ttu-id="ce699-147">Если заданной для true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="ce699-147">If set to true, activates this policy.</span></span> <span data-ttu-id="ce699-148">Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации.</span><span class="sxs-lookup"><span data-stu-id="ce699-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="ce699-149">Необязательный, значение по умолчанию является ложным.</span><span class="sxs-lookup"><span data-stu-id="ce699-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="ce699-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce699-150">Response</span></span>

<span data-ttu-id="ce699-p108">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ce699-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce699-153">Пример</span><span class="sxs-lookup"><span data-stu-id="ce699-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce699-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce699-154">Request</span></span>

<span data-ttu-id="ce699-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce699-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ce699-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce699-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_activitybasedtimeoutpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="ce699-157">C#</span><span class="sxs-lookup"><span data-stu-id="ce699-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce699-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce699-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce699-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce699-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce699-160">Java</span><span class="sxs-lookup"><span data-stu-id="ce699-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce699-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce699-161">Response</span></span>

<span data-ttu-id="ce699-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ce699-162">The following is an example of the response.</span></span>

> <span data-ttu-id="ce699-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ce699-163">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
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
  "description": "Update activitybasedtimeoutpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

