---
title: Обновление хранителя
description: Обновление свойств объекта custodian.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 605438ac3ba9883ca159fe97015701282f39e347
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658922"
---
# <a name="update-custodian"></a><span data-ttu-id="5aa7a-103">Обновление хранителя</span><span class="sxs-lookup"><span data-stu-id="5aa7a-103">Update custodian</span></span>

<span data-ttu-id="5aa7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aa7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aa7a-105">Обновление свойств объекта [custodian.](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="5aa7a-105">Update the properties of a [custodian](../resources/custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5aa7a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5aa7a-106">Permissions</span></span>

<span data-ttu-id="5aa7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5aa7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5aa7a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5aa7a-109">Permission type</span></span>|<span data-ttu-id="5aa7a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5aa7a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5aa7a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5aa7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5aa7a-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="5aa7a-112">User.Read</span></span>|
|<span data-ttu-id="5aa7a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5aa7a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5aa7a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-114">Not supported.</span></span>|
|<span data-ttu-id="5aa7a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5aa7a-115">Application</span></span>|<span data-ttu-id="5aa7a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5aa7a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5aa7a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}
```

## <a name="request-headers"></a><span data-ttu-id="5aa7a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5aa7a-118">Request headers</span></span>

|<span data-ttu-id="5aa7a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5aa7a-119">Name</span></span>|<span data-ttu-id="5aa7a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5aa7a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5aa7a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5aa7a-121">Authorization</span></span>|<span data-ttu-id="5aa7a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5aa7a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5aa7a-124">Content-Type</span></span>|<span data-ttu-id="5aa7a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5aa7a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5aa7a-127">Request body</span></span>

<span data-ttu-id="5aa7a-128">В теле запроса укажу представление объекта [хранителя](../resources/custodian.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-128">In the request body, supply a JSON representation of the [custodian](../resources/custodian.md) object.</span></span>

<span data-ttu-id="5aa7a-129">В следующей таблице перечислены свойства объекта [хранителя,](../resources/custodian.md) которые можно изменить.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-129">The following table lists the properties of a [custodian](../resources/custodian.md) object that can be modified.</span></span>

|<span data-ttu-id="5aa7a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5aa7a-130">Property</span></span>|<span data-ttu-id="5aa7a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5aa7a-131">Type</span></span>|<span data-ttu-id="5aa7a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5aa7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5aa7a-133">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="5aa7a-133">applyHoldToSources</span></span>|<span data-ttu-id="5aa7a-134">Логический</span><span class="sxs-lookup"><span data-stu-id="5aa7a-134">Boolean</span></span>|<span data-ttu-id="5aa7a-135">Определяет, были ли источники хранителя помещены на удержание во время создания.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-135">Identifies whether a custodian's sources were placed on hold during creation.</span></span> <span data-ttu-id="5aa7a-136">Подробные сведения см. в [под удержании для хранителей.](/microsoft-365/compliance/add-custodians-to-case#step-4-place-custodians-on-hold)</span><span class="sxs-lookup"><span data-stu-id="5aa7a-136">For details, see [Place custodians on hold](/microsoft-365/compliance/add-custodians-to-case#step-4-place-custodians-on-hold).</span></span>|

## <a name="response"></a><span data-ttu-id="5aa7a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5aa7a-137">Response</span></span>

<span data-ttu-id="5aa7a-138">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект хранителя](../resources/custodian.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-138">If successful, this method returns a `200 OK` response code and an updated [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5aa7a-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="5aa7a-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5aa7a-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5aa7a-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5aa7a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aa7a-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5aa7a-142">C#</span><span class="sxs-lookup"><span data-stu-id="5aa7a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-custodian-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5aa7a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5aa7a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-custodian-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5aa7a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aa7a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-custodian-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5aa7a-145">Java</span><span class="sxs-lookup"><span data-stu-id="5aa7a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-custodian-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5aa7a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5aa7a-146">Response</span></span>

<span data-ttu-id="5aa7a-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.custodian"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": false,
    "status": "active",
    "createdDateTime": "2020-10-30T20:59:54.9900703Z",
    "lastModifiedDateTime": "2020-10-30T21:01:34.1400013Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45454331323337443946343043464239",
    "displayName": "Adele Vance"
}
```
