---
title: Обновление клаимсмаппингполици
description: Обновление свойств объекта Клаимсмаппингполици.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbc70494077e9d2dea878c2da8657b3cf630aef1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083871"
---
# <a name="update-claimsmappingpolicy"></a><span data-ttu-id="440ed-103">Обновление клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="440ed-103">Update claimsmappingpolicy</span></span>

<span data-ttu-id="440ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="440ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="440ed-105">Обновление свойств объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="440ed-105">Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="440ed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="440ed-106">Permissions</span></span>

<span data-ttu-id="440ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="440ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="440ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="440ed-109">Permission type</span></span>                        | <span data-ttu-id="440ed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="440ed-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="440ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="440ed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="440ed-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="440ed-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="440ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="440ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="440ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="440ed-114">Not supported.</span></span> |
| <span data-ttu-id="440ed-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="440ed-115">Application</span></span>                            | <span data-ttu-id="440ed-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="440ed-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="440ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="440ed-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="440ed-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="440ed-118">Request headers</span></span>

| <span data-ttu-id="440ed-119">Имя</span><span class="sxs-lookup"><span data-stu-id="440ed-119">Name</span></span>       | <span data-ttu-id="440ed-120">Описание</span><span class="sxs-lookup"><span data-stu-id="440ed-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="440ed-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="440ed-121">Authorization</span></span> | <span data-ttu-id="440ed-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="440ed-122">Bearer {token}</span></span> |
| <span data-ttu-id="440ed-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="440ed-123">Content-type</span></span> | <span data-ttu-id="440ed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="440ed-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="440ed-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="440ed-125">Request body</span></span>

<span data-ttu-id="440ed-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="440ed-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="440ed-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="440ed-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="440ed-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="440ed-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="440ed-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="440ed-129">Property</span></span>     | <span data-ttu-id="440ed-130">Тип</span><span class="sxs-lookup"><span data-stu-id="440ed-130">Type</span></span>        | <span data-ttu-id="440ed-131">Описание</span><span class="sxs-lookup"><span data-stu-id="440ed-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="440ed-132">RDLC</span><span class="sxs-lookup"><span data-stu-id="440ed-132">definition</span></span>|<span data-ttu-id="440ed-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="440ed-133">String collection</span></span>| <span data-ttu-id="440ed-134">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="440ed-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="440ed-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="440ed-135">Required.</span></span>|
|<span data-ttu-id="440ed-136">description</span><span class="sxs-lookup"><span data-stu-id="440ed-136">description</span></span>|<span data-ttu-id="440ed-137">Строка</span><span class="sxs-lookup"><span data-stu-id="440ed-137">String</span></span>| <span data-ttu-id="440ed-138">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="440ed-138">Description for this policy.</span></span>|
|<span data-ttu-id="440ed-139">displayName</span><span class="sxs-lookup"><span data-stu-id="440ed-139">displayName</span></span>|<span data-ttu-id="440ed-140">Строка</span><span class="sxs-lookup"><span data-stu-id="440ed-140">String</span></span>| <span data-ttu-id="440ed-141">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="440ed-141">Display name for this policy.</span></span> <span data-ttu-id="440ed-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="440ed-142">Required.</span></span>|
|<span data-ttu-id="440ed-143">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="440ed-143">isOrganizationDefault</span></span>|<span data-ttu-id="440ed-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="440ed-144">Boolean</span></span>|<span data-ttu-id="440ed-145">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="440ed-145">If set to true, activates this policy.</span></span> <span data-ttu-id="440ed-146">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="440ed-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="440ed-147">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="440ed-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="440ed-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="440ed-148">Response</span></span>

<span data-ttu-id="440ed-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="440ed-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="440ed-151">Пример</span><span class="sxs-lookup"><span data-stu-id="440ed-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="440ed-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="440ed-152">Request</span></span>

<span data-ttu-id="440ed-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="440ed-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="440ed-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="440ed-154">HTTP</span></span>](#tab/http)
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
  "isOrganizationDefault": true,
  "type": "type-value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="440ed-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="440ed-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="440ed-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="440ed-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="440ed-157">Java</span><span class="sxs-lookup"><span data-stu-id="440ed-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="440ed-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="440ed-158">Response</span></span>

<span data-ttu-id="440ed-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="440ed-159">The following is an example of the response.</span></span>

> <span data-ttu-id="440ed-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="440ed-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

