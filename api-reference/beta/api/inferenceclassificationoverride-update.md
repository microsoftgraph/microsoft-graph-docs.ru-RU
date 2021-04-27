---
title: Обновление inferenceClassificationOverride
description: 'Измените **поле classifyAs** переопределения сфокусированного почтового ящика, как указано. '
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: ''
ms.openlocfilehash: 655be2a14ca6948bcb76bda02c1aaca43c5ad09b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040520"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="b12ca-103">Обновление inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="b12ca-103">Update inferenceClassificationOverride</span></span>

<span data-ttu-id="b12ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b12ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b12ca-105">Измените **поле classifyAs** переопределения сфокусированного почтового ящика, как указано. [](../resources/manage-focused-inbox.md)</span><span class="sxs-lookup"><span data-stu-id="b12ca-105">Change the **classifyAs** field of a [Focused Inbox](../resources/manage-focused-inbox.md) override as specified.</span></span>

<span data-ttu-id="b12ca-106">Вы не можете использовать операцию PATCH, чтобы менять поля в экземпляре [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="b12ca-106">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span>

<span data-ttu-id="b12ca-107">Если для конкретного отправителя существует переопределение и он меняет свое отображаемое имя, вы можете использовать операцию [POST](inferenceclassification-post-overrides.md) для принудительного обновления поля ввода имени в имеющемся переопределении.</span><span class="sxs-lookup"><span data-stu-id="b12ca-107">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="b12ca-108">Если для конкретного отправителя существует переопределение и он меняет свой SMTP-адрес, "обновить" переопределение для этого отправителя можно только [удалив](inferenceclassificationoverride-delete.md) существующее переопределение и [создав](inferenceclassification-post-overrides.md) другое с новым SMTP-адресом.</span><span class="sxs-lookup"><span data-stu-id="b12ca-108">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="b12ca-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b12ca-109">Permissions</span></span>
<span data-ttu-id="b12ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b12ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b12ca-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b12ca-112">Permission type</span></span>      | <span data-ttu-id="b12ca-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b12ca-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b12ca-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b12ca-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b12ca-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b12ca-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b12ca-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b12ca-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b12ca-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b12ca-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b12ca-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b12ca-118">Application</span></span> | <span data-ttu-id="b12ca-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b12ca-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b12ca-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b12ca-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b12ca-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b12ca-121">Request headers</span></span>
| <span data-ttu-id="b12ca-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b12ca-122">Name</span></span>       | <span data-ttu-id="b12ca-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b12ca-123">Type</span></span> | <span data-ttu-id="b12ca-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b12ca-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b12ca-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b12ca-125">Authorization</span></span>  | <span data-ttu-id="b12ca-126">string</span><span class="sxs-lookup"><span data-stu-id="b12ca-126">string</span></span>  | <span data-ttu-id="b12ca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b12ca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b12ca-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b12ca-129">Content-Type</span></span> | <span data-ttu-id="b12ca-130">string</span><span class="sxs-lookup"><span data-stu-id="b12ca-130">string</span></span>  | <span data-ttu-id="b12ca-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b12ca-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b12ca-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b12ca-133">Request body</span></span>
<span data-ttu-id="b12ca-p104">В тексте запроса предоставьте новое значение для поля **classifyAs**. Чтобы производительность была максимальной, не следует включать существующие значения, которые не меняются.</span><span class="sxs-lookup"><span data-stu-id="b12ca-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="b12ca-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="b12ca-136">Property</span></span>     | <span data-ttu-id="b12ca-137">Тип</span><span class="sxs-lookup"><span data-stu-id="b12ca-137">Type</span></span>   |<span data-ttu-id="b12ca-138">Описание</span><span class="sxs-lookup"><span data-stu-id="b12ca-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b12ca-139">classifyAs</span><span class="sxs-lookup"><span data-stu-id="b12ca-139">classifyAs</span></span>|<span data-ttu-id="b12ca-140">string</span><span class="sxs-lookup"><span data-stu-id="b12ca-140">string</span></span>| <span data-ttu-id="b12ca-p105">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="b12ca-p105">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="b12ca-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b12ca-143">Response</span></span>

<span data-ttu-id="b12ca-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b12ca-144">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b12ca-145">Пример</span><span class="sxs-lookup"><span data-stu-id="b12ca-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b12ca-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b12ca-146">Request</span></span>
<span data-ttu-id="b12ca-147">В следующем примере переопределение для SMTP-адреса randiw@adatum.onmicrosoft.com меняется из `other` на `focused`.</span><span class="sxs-lookup"><span data-stu-id="b12ca-147">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>


# <a name="http"></a>[<span data-ttu-id="b12ca-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="b12ca-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
# <a name="c"></a>[<span data-ttu-id="b12ca-149">C#</span><span class="sxs-lookup"><span data-stu-id="b12ca-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b12ca-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b12ca-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b12ca-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b12ca-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b12ca-152">Java</span><span class="sxs-lookup"><span data-stu-id="b12ca-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b12ca-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b12ca-153">Response</span></span>
<span data-ttu-id="b12ca-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b12ca-154">Here is an example of the response.</span></span> <span data-ttu-id="b12ca-155">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b12ca-155">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


