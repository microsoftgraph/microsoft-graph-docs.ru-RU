---
title: Обновление activitybasedtimeoutpolicy
description: Обновление свойств объекта activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 00f18ae417a33420001c0375576c08ce4fe1fd26
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910594"
---
# <a name="update-activitybasedtimeoutpolicy"></a><span data-ttu-id="001e4-103">Обновление activitybasedtimeoutpolicy</span><span class="sxs-lookup"><span data-stu-id="001e4-103">Update activitybasedtimeoutpolicy</span></span>

<span data-ttu-id="001e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="001e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="001e4-105">Обновление свойств объекта [activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="001e4-105">Update the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="001e4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="001e4-106">Permissions</span></span>

<span data-ttu-id="001e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="001e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="001e4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="001e4-109">Permission type</span></span>                        | <span data-ttu-id="001e4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="001e4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="001e4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="001e4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="001e4-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="001e4-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="001e4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="001e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="001e4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="001e4-114">Not supported.</span></span> |
| <span data-ttu-id="001e4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="001e4-115">Application</span></span>                            | <span data-ttu-id="001e4-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="001e4-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="001e4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="001e4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="001e4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="001e4-118">Request headers</span></span>

| <span data-ttu-id="001e4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="001e4-119">Name</span></span>       | <span data-ttu-id="001e4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="001e4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="001e4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="001e4-121">Authorization</span></span> | <span data-ttu-id="001e4-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="001e4-122">Bearer {token}</span></span> |
| <span data-ttu-id="001e4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="001e4-123">Content-type</span></span> | <span data-ttu-id="001e4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="001e4-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="001e4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="001e4-125">Request body</span></span>

<span data-ttu-id="001e4-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="001e4-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="001e4-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="001e4-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="001e4-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="001e4-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="001e4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="001e4-129">Property</span></span>     | <span data-ttu-id="001e4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="001e4-130">Type</span></span>        | <span data-ttu-id="001e4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="001e4-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="001e4-132">definition</span><span class="sxs-lookup"><span data-stu-id="001e4-132">definition</span></span>|<span data-ttu-id="001e4-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="001e4-133">String collection</span></span>| <span data-ttu-id="001e4-134">Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="001e4-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="001e4-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="001e4-135">Required.</span></span>|
|<span data-ttu-id="001e4-136">description</span><span class="sxs-lookup"><span data-stu-id="001e4-136">description</span></span>|<span data-ttu-id="001e4-137">String</span><span class="sxs-lookup"><span data-stu-id="001e4-137">String</span></span>| <span data-ttu-id="001e4-138">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="001e4-138">Description for this policy.</span></span>|
|<span data-ttu-id="001e4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="001e4-139">displayName</span></span>|<span data-ttu-id="001e4-140">String</span><span class="sxs-lookup"><span data-stu-id="001e4-140">String</span></span>| <span data-ttu-id="001e4-141">Отображаемого имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="001e4-141">Display name for this policy.</span></span> <span data-ttu-id="001e4-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="001e4-142">Required.</span></span>|
|<span data-ttu-id="001e4-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="001e4-143">isOrganizationDefault</span></span>|<span data-ttu-id="001e4-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="001e4-144">Boolean</span></span>|<span data-ttu-id="001e4-145">Если установлено true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="001e4-145">If set to true, activates this policy.</span></span> <span data-ttu-id="001e4-146">Для одного типа политики может быть несколько политик, но только одна может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="001e4-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="001e4-147">Необязательный, значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="001e4-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="001e4-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="001e4-148">Response</span></span>

<span data-ttu-id="001e4-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="001e4-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="001e4-151">Пример</span><span class="sxs-lookup"><span data-stu-id="001e4-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="001e4-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="001e4-152">Request</span></span>

<span data-ttu-id="001e4-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="001e4-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="001e4-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="001e4-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_activitybasedtimeoutpolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="001e4-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="001e4-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="001e4-156">C#</span><span class="sxs-lookup"><span data-stu-id="001e4-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="001e4-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="001e4-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="001e4-158">Java</span><span class="sxs-lookup"><span data-stu-id="001e4-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="001e4-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="001e4-159">Response</span></span>

<span data-ttu-id="001e4-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="001e4-160">The following is an example of the response.</span></span>

> <span data-ttu-id="001e4-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="001e4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


