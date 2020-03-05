---
title: Обновление хомереалмдисковериполици
description: Обновление свойств объекта Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2604911f823413ff7e29cb4e90fae5e0273b520e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446529"
---
# <a name="update-homerealmdiscoverypolicy"></a><span data-ttu-id="29e4d-103">Обновление хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="29e4d-103">Update homerealmdiscoverypolicy</span></span>

<span data-ttu-id="29e4d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="29e4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29e4d-105">Обновление свойств объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="29e4d-105">Update the properties of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="29e4d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29e4d-106">Permissions</span></span>

<span data-ttu-id="29e4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29e4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29e4d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29e4d-109">Permission type</span></span>                        | <span data-ttu-id="29e4d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29e4d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="29e4d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29e4d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="29e4d-112">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="29e4d-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="29e4d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29e4d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29e4d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29e4d-114">Not supported.</span></span> |
| <span data-ttu-id="29e4d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29e4d-115">Application</span></span>                            | <span data-ttu-id="29e4d-116">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="29e4d-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="29e4d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29e4d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="29e4d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29e4d-118">Request headers</span></span>

| <span data-ttu-id="29e4d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="29e4d-119">Name</span></span>       | <span data-ttu-id="29e4d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="29e4d-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="29e4d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="29e4d-121">Authorization</span></span> | <span data-ttu-id="29e4d-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="29e4d-122">Bearer {token}</span></span> |
| <span data-ttu-id="29e4d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29e4d-123">Content-type</span></span> | <span data-ttu-id="29e4d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="29e4d-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="29e4d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29e4d-125">Request body</span></span>

<span data-ttu-id="29e4d-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="29e4d-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="29e4d-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="29e4d-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="29e4d-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="29e4d-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="29e4d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="29e4d-129">Property</span></span>     | <span data-ttu-id="29e4d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="29e4d-130">Type</span></span>        | <span data-ttu-id="29e4d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="29e4d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="29e4d-132">RDLC</span><span class="sxs-lookup"><span data-stu-id="29e4d-132">definition</span></span>|<span data-ttu-id="29e4d-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="29e4d-133">String collection</span></span>| <span data-ttu-id="29e4d-134">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="29e4d-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="29e4d-135">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="29e4d-135">Required.</span></span>|
|<span data-ttu-id="29e4d-136">description</span><span class="sxs-lookup"><span data-stu-id="29e4d-136">description</span></span>|<span data-ttu-id="29e4d-137">String</span><span class="sxs-lookup"><span data-stu-id="29e4d-137">String</span></span>| <span data-ttu-id="29e4d-138">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="29e4d-138">Description for this policy.</span></span>|
|<span data-ttu-id="29e4d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="29e4d-139">displayName</span></span>|<span data-ttu-id="29e4d-140">Строка</span><span class="sxs-lookup"><span data-stu-id="29e4d-140">String</span></span>| <span data-ttu-id="29e4d-141">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="29e4d-141">Display name for this policy.</span></span> <span data-ttu-id="29e4d-142">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="29e4d-142">Required.</span></span>|
|<span data-ttu-id="29e4d-143">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="29e4d-143">isOrganizationDefault</span></span>|<span data-ttu-id="29e4d-144">Логический</span><span class="sxs-lookup"><span data-stu-id="29e4d-144">Boolean</span></span>|<span data-ttu-id="29e4d-145">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="29e4d-145">If set to true, activates this policy.</span></span> <span data-ttu-id="29e4d-146">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29e4d-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="29e4d-147">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="29e4d-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="29e4d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="29e4d-148">Response</span></span>

<span data-ttu-id="29e4d-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="29e4d-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29e4d-151">Пример</span><span class="sxs-lookup"><span data-stu-id="29e4d-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="29e4d-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="29e4d-152">Request</span></span>

<span data-ttu-id="29e4d-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29e4d-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="29e4d-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="29e4d-154">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="29e4d-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29e4d-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="29e4d-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="29e4d-156">Response</span></span>

<span data-ttu-id="29e4d-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="29e4d-157">The following is an example of the response.</span></span>

> <span data-ttu-id="29e4d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29e4d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
