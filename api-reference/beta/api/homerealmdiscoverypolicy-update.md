---
title: Обновление хомереалмдисковериполици
description: Обновление свойств объекта Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d8da4afac67140886bc2758072aa16706d01ab0b
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475751"
---
# <a name="update-homerealmdiscoverypolicy"></a><span data-ttu-id="516e0-103">Обновление хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="516e0-103">Update homerealmdiscoverypolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="516e0-104">Обновление свойств объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="516e0-104">Update the properties of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="516e0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="516e0-105">Permissions</span></span>

<span data-ttu-id="516e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="516e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="516e0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="516e0-108">Permission type</span></span>                        | <span data-ttu-id="516e0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="516e0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="516e0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="516e0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="516e0-111">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="516e0-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="516e0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="516e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="516e0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="516e0-113">Not supported.</span></span> |
| <span data-ttu-id="516e0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="516e0-114">Application</span></span>                            | <span data-ttu-id="516e0-115">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="516e0-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="516e0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="516e0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="516e0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="516e0-117">Request headers</span></span>

| <span data-ttu-id="516e0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="516e0-118">Name</span></span>       | <span data-ttu-id="516e0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="516e0-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="516e0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="516e0-120">Authorization</span></span> | <span data-ttu-id="516e0-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="516e0-121">Bearer {token}</span></span> |
| <span data-ttu-id="516e0-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="516e0-122">Content-type</span></span> | <span data-ttu-id="516e0-123">application/json</span><span class="sxs-lookup"><span data-stu-id="516e0-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="516e0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="516e0-124">Request body</span></span>

<span data-ttu-id="516e0-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="516e0-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="516e0-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="516e0-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="516e0-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="516e0-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="516e0-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="516e0-128">Property</span></span>     | <span data-ttu-id="516e0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="516e0-129">Type</span></span>        | <span data-ttu-id="516e0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="516e0-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="516e0-131">RDLC</span><span class="sxs-lookup"><span data-stu-id="516e0-131">definition</span></span>|<span data-ttu-id="516e0-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="516e0-132">String collection</span></span>| <span data-ttu-id="516e0-133">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="516e0-133">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="516e0-134">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="516e0-134">Required.</span></span>|
|<span data-ttu-id="516e0-135">description</span><span class="sxs-lookup"><span data-stu-id="516e0-135">description</span></span>|<span data-ttu-id="516e0-136">String</span><span class="sxs-lookup"><span data-stu-id="516e0-136">String</span></span>| <span data-ttu-id="516e0-137">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="516e0-137">Description for this policy.</span></span>|
|<span data-ttu-id="516e0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="516e0-138">displayName</span></span>|<span data-ttu-id="516e0-139">Строка</span><span class="sxs-lookup"><span data-stu-id="516e0-139">String</span></span>| <span data-ttu-id="516e0-140">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="516e0-140">Display name for this policy.</span></span> <span data-ttu-id="516e0-141">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="516e0-141">Required.</span></span>|
|<span data-ttu-id="516e0-142">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="516e0-142">isOrganizationDefault</span></span>|<span data-ttu-id="516e0-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="516e0-143">Boolean</span></span>|<span data-ttu-id="516e0-144">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="516e0-144">If set to true, activates this policy.</span></span> <span data-ttu-id="516e0-145">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="516e0-145">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="516e0-146">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="516e0-146">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="516e0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="516e0-147">Response</span></span>

<span data-ttu-id="516e0-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="516e0-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="516e0-150">Пример</span><span class="sxs-lookup"><span data-stu-id="516e0-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="516e0-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="516e0-151">Request</span></span>

<span data-ttu-id="516e0-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="516e0-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="516e0-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="516e0-153">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="516e0-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="516e0-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="516e0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="516e0-155">Response</span></span>

<span data-ttu-id="516e0-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="516e0-156">The following is an example of the response.</span></span>

> <span data-ttu-id="516e0-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="516e0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
