---
title: Создание хранителя
description: Создание объекта хранителя.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: e5472f9c3ff80a1e1fb127ebddc566880e2056aa
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659536"
---
# <a name="create-custodian"></a><span data-ttu-id="27ac6-103">Создание хранителя</span><span class="sxs-lookup"><span data-stu-id="27ac6-103">Create custodian</span></span>

<span data-ttu-id="27ac6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27ac6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27ac6-105">Создание объекта [хранителя.](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="27ac6-105">Create a new [custodian](../resources/custodian.md) object.</span></span> <span data-ttu-id="27ac6-106">После создания объекта хранителя необходимо создать [userSource](../resources/usersource.md) хранителя для ссылки на его почтовый ящик и сайт OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="27ac6-106">After the custodian object is created, you will need to create the custodian's [userSource](../resources/usersource.md) to reference their mailbox and OneDrive for Business site.</span></span>

## <a name="permissions"></a><span data-ttu-id="27ac6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27ac6-107">Permissions</span></span>

<span data-ttu-id="27ac6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27ac6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27ac6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27ac6-110">Permission type</span></span>|<span data-ttu-id="27ac6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27ac6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27ac6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27ac6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27ac6-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="27ac6-113">User.Read</span></span>|
|<span data-ttu-id="27ac6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27ac6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27ac6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27ac6-115">Not supported.</span></span>|
|<span data-ttu-id="27ac6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27ac6-116">Application</span></span>|<span data-ttu-id="27ac6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27ac6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27ac6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27ac6-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians
```

## <a name="request-headers"></a><span data-ttu-id="27ac6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27ac6-119">Request headers</span></span>

|<span data-ttu-id="27ac6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="27ac6-120">Name</span></span>|<span data-ttu-id="27ac6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="27ac6-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="27ac6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27ac6-122">Authorization</span></span>|<span data-ttu-id="27ac6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27ac6-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="27ac6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27ac6-125">Content-Type</span></span>|<span data-ttu-id="27ac6-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27ac6-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27ac6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27ac6-128">Request body</span></span>

<span data-ttu-id="27ac6-129">В теле запроса укажу представление объекта [хранителя](../resources/custodian.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="27ac6-129">In the request body, supply a JSON representation of the [custodian](../resources/custodian.md) object.</span></span>

<span data-ttu-id="27ac6-130">В следующей таблице показаны свойства, необходимые при создании [хранителя.](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="27ac6-130">The following table shows the properties that are required when you create the [custodian](../resources/custodian.md).</span></span>

|<span data-ttu-id="27ac6-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="27ac6-131">Property</span></span>|<span data-ttu-id="27ac6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="27ac6-132">Type</span></span>|<span data-ttu-id="27ac6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="27ac6-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27ac6-134">email</span><span class="sxs-lookup"><span data-stu-id="27ac6-134">email</span></span>|<span data-ttu-id="27ac6-135">String</span><span class="sxs-lookup"><span data-stu-id="27ac6-135">String</span></span>|<span data-ttu-id="27ac6-136">Основной SMTP-адрес хранителя.</span><span class="sxs-lookup"><span data-stu-id="27ac6-136">Custodian's primary SMTP address.</span></span> <span data-ttu-id="27ac6-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27ac6-137">Required.</span></span>|
|<span data-ttu-id="27ac6-138">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="27ac6-138">applyHoldToSources</span></span>|<span data-ttu-id="27ac6-139">Логический</span><span class="sxs-lookup"><span data-stu-id="27ac6-139">Boolean</span></span>|<span data-ttu-id="27ac6-140">Указывает, применяется ли удержание к источникам хранителя (например, почтовым ящикам, сайтам или Teams).</span><span class="sxs-lookup"><span data-stu-id="27ac6-140">Indicates whether a hold is applied to the custodian's sources (such as mailboxes, sites, or Teams).</span></span>|

## <a name="response"></a><span data-ttu-id="27ac6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="27ac6-141">Response</span></span>

<span data-ttu-id="27ac6-142">В случае успеха этот метод возвращает код отклика и объект `201 Created` [хранителя](../resources/custodian.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27ac6-142">If successful, this method returns a `201 Created` response code and a [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27ac6-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="27ac6-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27ac6-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="27ac6-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="27ac6-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="27ac6-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_custodian_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
Content-Type: application/json
Content-length: 279

{
    "email":"AdeleV@contoso.com",
    "applyHoldToSources":"true"
}
```
# <a name="c"></a>[<span data-ttu-id="27ac6-146">C#</span><span class="sxs-lookup"><span data-stu-id="27ac6-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-custodian-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27ac6-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27ac6-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-custodian-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27ac6-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27ac6-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-custodian-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27ac6-149">Java</span><span class="sxs-lookup"><span data-stu-id="27ac6-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-custodian-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27ac6-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="27ac6-150">Response</span></span>

<span data-ttu-id="27ac6-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="27ac6-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.custodian"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": false,
    "status": "active",
    "createdDateTime": "2020-10-30T20:47:01.7724531Z",
    "lastModifiedDateTime": "2020-10-30T20:47:02.2512381Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45353243323138344430413038363846",
    "displayName": "Adele Vance"
}
```
