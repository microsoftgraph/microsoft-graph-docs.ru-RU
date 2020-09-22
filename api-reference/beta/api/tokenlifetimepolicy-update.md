---
title: Обновление токенлифетимеполици
description: Обновление свойств объекта Токенлифетимеполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 21c4f1c80e2cfa1a74d79bb5f80b35d788613680
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062206"
---
# <a name="update-tokenlifetimepolicy"></a><span data-ttu-id="0f045-103">Обновление токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="0f045-103">Update tokenlifetimepolicy</span></span>

<span data-ttu-id="0f045-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f045-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f045-105">Обновление свойств объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0f045-105">Update the properties of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f045-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f045-106">Permissions</span></span>

<span data-ttu-id="0f045-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f045-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f045-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f045-109">Permission type</span></span>                        | <span data-ttu-id="0f045-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f045-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0f045-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f045-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f045-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f045-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
| <span data-ttu-id="0f045-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f045-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f045-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f045-114">Not supported.</span></span> |
| <span data-ttu-id="0f045-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f045-115">Application</span></span>                            | <span data-ttu-id="0f045-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f045-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f045-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f045-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0f045-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f045-118">Request headers</span></span>

| <span data-ttu-id="0f045-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0f045-119">Name</span></span>       | <span data-ttu-id="0f045-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0f045-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0f045-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f045-121">Authorization</span></span> | <span data-ttu-id="0f045-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="0f045-122">Bearer {token}</span></span> |
| <span data-ttu-id="0f045-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f045-123">Content-type</span></span> | <span data-ttu-id="0f045-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0f045-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f045-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f045-125">Request body</span></span>

<span data-ttu-id="0f045-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0f045-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0f045-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0f045-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0f045-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0f045-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0f045-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f045-129">Property</span></span>     | <span data-ttu-id="0f045-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0f045-130">Type</span></span>        | <span data-ttu-id="0f045-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0f045-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0f045-132">RDLC</span><span class="sxs-lookup"><span data-stu-id="0f045-132">definition</span></span>|<span data-ttu-id="0f045-133">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="0f045-133">String collection</span></span>| <span data-ttu-id="0f045-134">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0f045-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="0f045-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f045-135">Required.</span></span>|
|<span data-ttu-id="0f045-136">description</span><span class="sxs-lookup"><span data-stu-id="0f045-136">description</span></span>|<span data-ttu-id="0f045-137">String</span><span class="sxs-lookup"><span data-stu-id="0f045-137">String</span></span>| <span data-ttu-id="0f045-138">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0f045-138">Description for this policy.</span></span>|
|<span data-ttu-id="0f045-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0f045-139">displayName</span></span>|<span data-ttu-id="0f045-140">String</span><span class="sxs-lookup"><span data-stu-id="0f045-140">String</span></span>| <span data-ttu-id="0f045-141">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0f045-141">Display name for this policy.</span></span> <span data-ttu-id="0f045-142">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="0f045-142">Required.</span></span>|
|<span data-ttu-id="0f045-143">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="0f045-143">isOrganizationDefault</span></span>|<span data-ttu-id="0f045-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f045-144">Boolean</span></span>|<span data-ttu-id="0f045-145">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="0f045-145">If set to true, activates this policy.</span></span> <span data-ttu-id="0f045-146">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0f045-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="0f045-147">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="0f045-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="0f045-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f045-148">Response</span></span>

<span data-ttu-id="0f045-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0f045-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f045-151">Пример</span><span class="sxs-lookup"><span data-stu-id="0f045-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f045-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f045-152">Request</span></span>

<span data-ttu-id="0f045-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f045-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0f045-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f045-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tokenlifetimepolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "type": "type-value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="0f045-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f045-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="0f045-156">C#</span><span class="sxs-lookup"><span data-stu-id="0f045-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f045-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f045-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0f045-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f045-158">Response</span></span>

<span data-ttu-id="0f045-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0f045-159">The following is an example of the response.</span></span>

> <span data-ttu-id="0f045-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f045-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Update tokenlifetimepolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


