---
title: Создание custodian userSource
description: Создание нового объекта userSource хранителя.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1fb67377785a8120bb6e4b1453901b9f8b0137ed
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946140"
---
# <a name="create-custodian-usersource"></a><span data-ttu-id="dee43-103">Создание custodian userSource</span><span class="sxs-lookup"><span data-stu-id="dee43-103">Create custodian userSource</span></span>

<span data-ttu-id="dee43-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="dee43-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dee43-105">Создание нового объекта [userSource хранителя.](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="dee43-105">Create a new custodian [userSource](../resources/ediscovery-usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dee43-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dee43-106">Permissions</span></span>

<span data-ttu-id="dee43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dee43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dee43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dee43-109">Permission type</span></span>|<span data-ttu-id="dee43-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dee43-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dee43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dee43-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dee43-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dee43-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="dee43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dee43-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dee43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dee43-114">Not supported.</span></span>|
|<span data-ttu-id="dee43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dee43-115">Application</span></span>|<span data-ttu-id="dee43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dee43-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dee43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dee43-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="dee43-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dee43-118">Request headers</span></span>

|<span data-ttu-id="dee43-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dee43-119">Name</span></span>|<span data-ttu-id="dee43-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dee43-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dee43-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dee43-121">Authorization</span></span>|<span data-ttu-id="dee43-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dee43-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="dee43-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dee43-124">Content-Type</span></span>|<span data-ttu-id="dee43-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dee43-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dee43-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dee43-127">Request body</span></span>

<span data-ttu-id="dee43-128">В теле запроса поставляем JSON-представление [объекта userSource.](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="dee43-128">In the request body, supply a JSON representation of the [userSource](../resources/ediscovery-usersource.md) object.</span></span>

<span data-ttu-id="dee43-129">В следующей таблице показаны свойства, необходимые при создании [userSource.](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="dee43-129">The following table shows the properties that are required when you create the [userSource](../resources/ediscovery-usersource.md).</span></span>

|<span data-ttu-id="dee43-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dee43-130">Property</span></span>|<span data-ttu-id="dee43-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dee43-131">Type</span></span>|<span data-ttu-id="dee43-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dee43-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dee43-133">email</span><span class="sxs-lookup"><span data-stu-id="dee43-133">email</span></span>|<span data-ttu-id="dee43-134">String</span><span class="sxs-lookup"><span data-stu-id="dee43-134">String</span></span>|<span data-ttu-id="dee43-135">SMTP-адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="dee43-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="dee43-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="dee43-136">includedSources</span></span>|<span data-ttu-id="dee43-137">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="dee43-137">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="dee43-138">Указывает, какие источники включены в эту группу.</span><span class="sxs-lookup"><span data-stu-id="dee43-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="dee43-139">Возможные значения: `mailbox`, `site`.</span><span class="sxs-lookup"><span data-stu-id="dee43-139">Possible values are: `mailbox`, `site`.</span></span>|

## <a name="response"></a><span data-ttu-id="dee43-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dee43-140">Response</span></span>

<span data-ttu-id="dee43-141">В случае успеха этот метод возвращает код отклика и `201 Created` [объект microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dee43-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dee43-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="dee43-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dee43-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="dee43-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dee43-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="dee43-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_usersource_from__1"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources
Content-Type: application/json
Content-length: 233

{
    "email":"megan@contoso.com",
    "includedSources":"mailbox, site"
}
```
# <a name="c"></a>[<span data-ttu-id="dee43-145">C#</span><span class="sxs-lookup"><span data-stu-id="dee43-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-usersource-from--1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dee43-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dee43-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-usersource-from--1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dee43-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dee43-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-usersource-from--1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dee43-148">Java</span><span class="sxs-lookup"><span data-stu-id="dee43-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-usersource-from--1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="dee43-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="dee43-149">Response</span></span>

<span data-ttu-id="dee43-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dee43-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.userSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('45454331323337443946343043464239')/userSources/$entity",
    "displayName": "Megan Bowen",
    "createdDateTime": "2020-11-06T16:09:08.4905571Z",
    "id": "34383036-3741-4545-3242-373530353435",
    "email": "megan@contoso.com",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null
        }
    }
}
```
