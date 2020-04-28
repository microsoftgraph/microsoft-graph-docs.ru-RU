---
title: Обновление Токениссуанцеполици
description: Обновление свойств объекта Токениссуанцеполици.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a521a6b8999abb9ff48959be8f42e7f7094d83f7
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916313"
---
# <a name="update-tokenissuancepolicy"></a><span data-ttu-id="d73da-103">Обновление Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="d73da-103">Update tokenIssuancePolicy</span></span>

<span data-ttu-id="d73da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d73da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d73da-105">Обновление свойств объекта [токениссуанцеполици](../resources/tokenIssuancePolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d73da-105">Update the properties of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d73da-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d73da-106">Permissions</span></span>

<span data-ttu-id="d73da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d73da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d73da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d73da-109">Permission type</span></span>                        | <span data-ttu-id="d73da-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d73da-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d73da-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d73da-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d73da-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="d73da-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="d73da-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d73da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d73da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d73da-114">Not supported.</span></span> |
| <span data-ttu-id="d73da-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d73da-115">Application</span></span>                            | <span data-ttu-id="d73da-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="d73da-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="d73da-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d73da-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d73da-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d73da-118">Request headers</span></span>

| <span data-ttu-id="d73da-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d73da-119">Name</span></span>       | <span data-ttu-id="d73da-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d73da-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d73da-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d73da-121">Authorization</span></span> | <span data-ttu-id="d73da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d73da-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d73da-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d73da-124">Content-type</span></span> | <span data-ttu-id="d73da-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d73da-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d73da-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d73da-127">Request body</span></span>

<span data-ttu-id="d73da-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d73da-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d73da-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="d73da-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d73da-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d73da-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d73da-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d73da-131">Property</span></span>     | <span data-ttu-id="d73da-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d73da-132">Type</span></span>        | <span data-ttu-id="d73da-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d73da-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d73da-134">RDLC</span><span class="sxs-lookup"><span data-stu-id="d73da-134">definition</span></span>|<span data-ttu-id="d73da-135">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="d73da-135">String collection</span></span>| <span data-ttu-id="d73da-136">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d73da-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="d73da-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d73da-137">Required.</span></span>|
|<span data-ttu-id="d73da-138">description</span><span class="sxs-lookup"><span data-stu-id="d73da-138">description</span></span>|<span data-ttu-id="d73da-139">String</span><span class="sxs-lookup"><span data-stu-id="d73da-139">String</span></span>| <span data-ttu-id="d73da-140">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d73da-140">Description for this policy.</span></span>|
|<span data-ttu-id="d73da-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d73da-141">displayName</span></span>|<span data-ttu-id="d73da-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d73da-142">String</span></span>| <span data-ttu-id="d73da-143">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d73da-143">Display name for this policy.</span></span> <span data-ttu-id="d73da-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d73da-144">Required.</span></span>|
|<span data-ttu-id="d73da-145">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="d73da-145">isOrganizationDefault</span></span>|<span data-ttu-id="d73da-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d73da-146">Boolean</span></span>|<span data-ttu-id="d73da-147">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="d73da-147">If set to true, activates this policy.</span></span> <span data-ttu-id="d73da-148">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d73da-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="d73da-149">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="d73da-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="d73da-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d73da-150">Response</span></span>

<span data-ttu-id="d73da-p108">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d73da-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d73da-153">Пример</span><span class="sxs-lookup"><span data-stu-id="d73da-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="d73da-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="d73da-154">Request</span></span>

<span data-ttu-id="d73da-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d73da-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d73da-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="d73da-156">HTTP</span></span>](#tab/http)
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
  "isOrganizationDefault": true,
  "type": "type-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d73da-157">C#</span><span class="sxs-lookup"><span data-stu-id="d73da-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d73da-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d73da-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d73da-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d73da-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="d73da-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="d73da-160">Response</span></span>

<span data-ttu-id="d73da-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d73da-161">The following is an example of the response.</span></span>

> <span data-ttu-id="d73da-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d73da-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
