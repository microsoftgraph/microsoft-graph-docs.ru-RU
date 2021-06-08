---
title: Хранители обновлений
description: Обновление свойств объекта-хранителя.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 051c7db53f9d949018583fcb2f6a1e44ce2eddb9
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786014"
---
# <a name="update-custodian"></a><span data-ttu-id="69f54-103">Хранители обновлений</span><span class="sxs-lookup"><span data-stu-id="69f54-103">Update custodian</span></span>

<span data-ttu-id="69f54-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="69f54-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69f54-105">Обновление свойств [объекта-хранителя.](../resources/ediscovery-custodian.md)</span><span class="sxs-lookup"><span data-stu-id="69f54-105">Update the properties of a [custodian](../resources/ediscovery-custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="69f54-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69f54-106">Permissions</span></span>

<span data-ttu-id="69f54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f54-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69f54-109">Permission type</span></span>|<span data-ttu-id="69f54-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69f54-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f54-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69f54-111">Delegated (work or school account)</span></span>|<span data-ttu-id="69f54-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f54-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="69f54-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69f54-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f54-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f54-114">Not supported.</span></span>|
|<span data-ttu-id="69f54-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69f54-115">Application</span></span>|<span data-ttu-id="69f54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f54-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f54-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69f54-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}
```

## <a name="request-headers"></a><span data-ttu-id="69f54-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69f54-118">Request headers</span></span>

|<span data-ttu-id="69f54-119">Имя</span><span class="sxs-lookup"><span data-stu-id="69f54-119">Name</span></span>|<span data-ttu-id="69f54-120">Описание</span><span class="sxs-lookup"><span data-stu-id="69f54-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69f54-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69f54-121">Authorization</span></span>|<span data-ttu-id="69f54-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69f54-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="69f54-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69f54-124">Content-Type</span></span>|<span data-ttu-id="69f54-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69f54-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f54-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69f54-127">Request body</span></span>

<span data-ttu-id="69f54-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="69f54-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="69f54-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="69f54-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="69f54-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="69f54-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="69f54-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="69f54-131">Property</span></span>|<span data-ttu-id="69f54-132">Тип</span><span class="sxs-lookup"><span data-stu-id="69f54-132">Type</span></span>|<span data-ttu-id="69f54-133">Описание</span><span class="sxs-lookup"><span data-stu-id="69f54-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69f54-134">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="69f54-134">applyHoldToSources</span></span>|<span data-ttu-id="69f54-135">Логический</span><span class="sxs-lookup"><span data-stu-id="69f54-135">Boolean</span></span>|<span data-ttu-id="69f54-136">Определяет, были ли приодержится источники хранителя во время создания.</span><span class="sxs-lookup"><span data-stu-id="69f54-136">Identifies whether a custodian's sources were placed on hold during creation.</span></span>|

## <a name="response"></a><span data-ttu-id="69f54-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="69f54-137">Response</span></span>

<span data-ttu-id="69f54-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="69f54-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="69f54-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="69f54-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69f54-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="69f54-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="69f54-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="69f54-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_custodian"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
Content-Type: application/json
Content-length: 254

{
  "applyHoldToSources": "false",
}
```
# <a name="c"></a>[<span data-ttu-id="69f54-142">C#</span><span class="sxs-lookup"><span data-stu-id="69f54-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-custodian-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69f54-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69f54-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-custodian-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69f54-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69f54-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-custodian-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69f54-145">Java</span><span class="sxs-lookup"><span data-stu-id="69f54-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-custodian-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="69f54-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f54-146">Response</span></span>

<!-- {
  "blockType": "response"
}
-->

``` http
HTTP/1.1 204 No Content
```
