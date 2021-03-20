---
title: Создание legalHold userSource
description: Создание нового объекта legalHold userSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5c49ba39da5967713d0b80ed51cf0aa95229f4be
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952428"
---
# <a name="create-legalhold-usersource"></a><span data-ttu-id="88ba3-103">Создание legalHold userSource</span><span class="sxs-lookup"><span data-stu-id="88ba3-103">Create legalHold userSource</span></span>

<span data-ttu-id="88ba3-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="88ba3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88ba3-105">Добавляет userSource в объект legalHold.</span><span class="sxs-lookup"><span data-stu-id="88ba3-105">Adds a userSource to a legalHold object.</span></span>

## <a name="permissions"></a><span data-ttu-id="88ba3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88ba3-106">Permissions</span></span>

<span data-ttu-id="88ba3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88ba3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88ba3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88ba3-109">Permission type</span></span>|<span data-ttu-id="88ba3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88ba3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88ba3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88ba3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88ba3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88ba3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="88ba3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88ba3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88ba3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88ba3-114">Not supported.</span></span>|
|<span data-ttu-id="88ba3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88ba3-115">Application</span></span>|<span data-ttu-id="88ba3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88ba3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88ba3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88ba3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="88ba3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88ba3-118">Request headers</span></span>

|<span data-ttu-id="88ba3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="88ba3-119">Name</span></span>|<span data-ttu-id="88ba3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="88ba3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="88ba3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88ba3-121">Authorization</span></span>|<span data-ttu-id="88ba3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88ba3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="88ba3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88ba3-124">Content-Type</span></span>|<span data-ttu-id="88ba3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88ba3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88ba3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88ba3-127">Request body</span></span>

<span data-ttu-id="88ba3-128">В теле запроса поставляем JSON-представление [объекта userSource.](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="88ba3-128">In the request body, supply a JSON representation of the [userSource](../resources/ediscovery-usersource.md) object.</span></span>

<span data-ttu-id="88ba3-129">В следующей таблице показаны свойства, необходимые при создании [userSource.](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="88ba3-129">The following table shows the properties that are required when you create the [userSource](../resources/ediscovery-usersource.md).</span></span>

|<span data-ttu-id="88ba3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="88ba3-130">Property</span></span>|<span data-ttu-id="88ba3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="88ba3-131">Type</span></span>|<span data-ttu-id="88ba3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="88ba3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88ba3-133">email</span><span class="sxs-lookup"><span data-stu-id="88ba3-133">email</span></span>|<span data-ttu-id="88ba3-134">String</span><span class="sxs-lookup"><span data-stu-id="88ba3-134">String</span></span>|<span data-ttu-id="88ba3-135">SMTP-адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="88ba3-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="88ba3-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="88ba3-136">includedSources</span></span>|<span data-ttu-id="88ba3-137">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="88ba3-137">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="88ba3-138">Указывает, какие источники включены в эту группу.</span><span class="sxs-lookup"><span data-stu-id="88ba3-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="88ba3-139">Это значение должно быть `mailbox` , `site` не поддерживается для legalHolds в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="88ba3-139">This value must be `mailbox`, `site` is not supported for legalHolds at this time.</span></span>|

## <a name="response"></a><span data-ttu-id="88ba3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="88ba3-140">Response</span></span>

<span data-ttu-id="88ba3-141">В случае успеха этот метод возвращает код отклика и `201 Created` [объект microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="88ba3-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88ba3-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="88ba3-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88ba3-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="88ba3-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="88ba3-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="88ba3-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_usersource_from__2"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/userSources
Content-Type: application/json
Content-length: 208

{
  "email": "adelev@contoso.com",
  "includedSources": "mailbox"
}
```
# <a name="c"></a>[<span data-ttu-id="88ba3-145">C#</span><span class="sxs-lookup"><span data-stu-id="88ba3-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-usersource-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88ba3-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88ba3-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-usersource-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88ba3-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88ba3-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-usersource-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88ba3-148">Java</span><span class="sxs-lookup"><span data-stu-id="88ba3-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-usersource-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="88ba3-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="88ba3-149">Response</span></span>

<span data-ttu-id="88ba3-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="88ba3-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalholds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/userSources",
    "value": [
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-12-28T20:08:57.857Z",
            "id": "2192ca40-8ea2-410e-ba3b-ec8ae873be6b",
            "email": "AdeleV@contoso.com",
            "includedSources": "mailbox",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "EDiscovery admin"
                }
            }
        }
    ]
}
```
