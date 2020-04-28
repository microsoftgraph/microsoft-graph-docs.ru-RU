---
title: Обновление хомереалмдисковериполици
description: Обновление свойств объекта Хомереалмдисковериполици.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 82c1e77b6ef1e282fa4f11a864867520eb0ac06b
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916547"
---
# <a name="update-homerealmdiscoverypolicy"></a><span data-ttu-id="1bf11-103">Обновление хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="1bf11-103">Update homerealmdiscoverypolicy</span></span>

<span data-ttu-id="1bf11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bf11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bf11-105">Обновление свойств объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1bf11-105">Update the properties of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bf11-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bf11-106">Permissions</span></span>

<span data-ttu-id="1bf11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bf11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1bf11-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bf11-109">Permission type</span></span>                        | <span data-ttu-id="1bf11-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bf11-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1bf11-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bf11-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1bf11-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1bf11-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="1bf11-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bf11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bf11-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bf11-114">Not supported.</span></span> |
| <span data-ttu-id="1bf11-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bf11-115">Application</span></span>                            | <span data-ttu-id="1bf11-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1bf11-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bf11-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bf11-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1bf11-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bf11-118">Request headers</span></span>

| <span data-ttu-id="1bf11-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1bf11-119">Name</span></span>       | <span data-ttu-id="1bf11-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1bf11-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1bf11-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bf11-121">Authorization</span></span> | <span data-ttu-id="1bf11-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1bf11-122">Bearer {token}</span></span> |
| <span data-ttu-id="1bf11-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1bf11-123">Content-type</span></span> | <span data-ttu-id="1bf11-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1bf11-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bf11-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bf11-125">Request body</span></span>

<span data-ttu-id="1bf11-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1bf11-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1bf11-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1bf11-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1bf11-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1bf11-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1bf11-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bf11-129">Property</span></span>     | <span data-ttu-id="1bf11-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1bf11-130">Type</span></span>        | <span data-ttu-id="1bf11-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1bf11-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1bf11-132">RDLC</span><span class="sxs-lookup"><span data-stu-id="1bf11-132">definition</span></span>|<span data-ttu-id="1bf11-133">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="1bf11-133">String collection</span></span>| <span data-ttu-id="1bf11-134">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1bf11-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="1bf11-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bf11-135">Required.</span></span>|
|<span data-ttu-id="1bf11-136">description</span><span class="sxs-lookup"><span data-stu-id="1bf11-136">description</span></span>|<span data-ttu-id="1bf11-137">String</span><span class="sxs-lookup"><span data-stu-id="1bf11-137">String</span></span>| <span data-ttu-id="1bf11-138">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1bf11-138">Description for this policy.</span></span>|
|<span data-ttu-id="1bf11-139">displayName</span><span class="sxs-lookup"><span data-stu-id="1bf11-139">displayName</span></span>|<span data-ttu-id="1bf11-140">Строка</span><span class="sxs-lookup"><span data-stu-id="1bf11-140">String</span></span>| <span data-ttu-id="1bf11-141">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1bf11-141">Display name for this policy.</span></span> <span data-ttu-id="1bf11-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bf11-142">Required.</span></span>|
|<span data-ttu-id="1bf11-143">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="1bf11-143">isOrganizationDefault</span></span>|<span data-ttu-id="1bf11-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bf11-144">Boolean</span></span>|<span data-ttu-id="1bf11-145">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="1bf11-145">If set to true, activates this policy.</span></span> <span data-ttu-id="1bf11-146">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1bf11-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="1bf11-147">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="1bf11-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="1bf11-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bf11-148">Response</span></span>

<span data-ttu-id="1bf11-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1bf11-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bf11-151">Пример</span><span class="sxs-lookup"><span data-stu-id="1bf11-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bf11-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bf11-152">Request</span></span>

<span data-ttu-id="1bf11-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bf11-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1bf11-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bf11-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_homerealmdiscoverypolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
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
# <a name="javascript"></a>[<span data-ttu-id="1bf11-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bf11-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="1bf11-156">C#</span><span class="sxs-lookup"><span data-stu-id="1bf11-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bf11-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bf11-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1bf11-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="1bf11-158">Response</span></span>

<span data-ttu-id="1bf11-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1bf11-159">The following is an example of the response.</span></span>

> <span data-ttu-id="1bf11-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bf11-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
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
  "description": "Update homerealmdiscoverypolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
