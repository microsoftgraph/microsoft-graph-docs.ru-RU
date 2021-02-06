---
title: Обновление inferenceClassificationOverride
description: 'Измените **поле classifyAs** переопределения focused inbox, как указано. '
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: ''
ms.openlocfilehash: 9195466b1ea09b9b0dde4c00a057d95548184edf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130328"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="fadf5-103">Обновление inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="fadf5-103">Update inferenceClassificationOverride</span></span>

<span data-ttu-id="fadf5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fadf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fadf5-105">Измените **поле classifyAs** переопределения [focused inbox,](../resources/manage-focused-inbox.md) как указано.</span><span class="sxs-lookup"><span data-stu-id="fadf5-105">Change the **classifyAs** field of a [Focused Inbox](../resources/manage-focused-inbox.md) override as specified.</span></span>

<span data-ttu-id="fadf5-106">Вы не можете использовать операцию PATCH, чтобы менять поля в экземпляре [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="fadf5-106">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span>

<span data-ttu-id="fadf5-107">Если для конкретного отправителя существует переопределение и он меняет свое отображаемое имя, вы можете использовать операцию [POST](inferenceclassification-post-overrides.md) для принудительного обновления поля ввода имени в имеющемся переопределении.</span><span class="sxs-lookup"><span data-stu-id="fadf5-107">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="fadf5-108">Если для конкретного отправителя существует переопределение и он меняет свой SMTP-адрес, "обновить" переопределение для этого отправителя можно только [удалив](inferenceclassificationoverride-delete.md) существующее переопределение и [создав](inferenceclassification-post-overrides.md) другое с новым SMTP-адресом.</span><span class="sxs-lookup"><span data-stu-id="fadf5-108">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="fadf5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fadf5-109">Permissions</span></span>
<span data-ttu-id="fadf5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fadf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fadf5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fadf5-112">Permission type</span></span>      | <span data-ttu-id="fadf5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fadf5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fadf5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fadf5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fadf5-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fadf5-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fadf5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fadf5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fadf5-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fadf5-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fadf5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fadf5-118">Application</span></span> | <span data-ttu-id="fadf5-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fadf5-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fadf5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fadf5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fadf5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fadf5-121">Request headers</span></span>
| <span data-ttu-id="fadf5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fadf5-122">Name</span></span>       | <span data-ttu-id="fadf5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="fadf5-123">Type</span></span> | <span data-ttu-id="fadf5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fadf5-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fadf5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fadf5-125">Authorization</span></span>  | <span data-ttu-id="fadf5-126">string</span><span class="sxs-lookup"><span data-stu-id="fadf5-126">string</span></span>  | <span data-ttu-id="fadf5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fadf5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fadf5-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fadf5-129">Content-Type</span></span> | <span data-ttu-id="fadf5-130">string</span><span class="sxs-lookup"><span data-stu-id="fadf5-130">string</span></span>  | <span data-ttu-id="fadf5-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fadf5-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fadf5-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fadf5-133">Request body</span></span>
<span data-ttu-id="fadf5-p104">В тексте запроса предоставьте новое значение для поля **classifyAs**. Чтобы производительность была максимальной, не следует включать существующие значения, которые не меняются.</span><span class="sxs-lookup"><span data-stu-id="fadf5-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="fadf5-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="fadf5-136">Property</span></span>     | <span data-ttu-id="fadf5-137">Тип</span><span class="sxs-lookup"><span data-stu-id="fadf5-137">Type</span></span>   |<span data-ttu-id="fadf5-138">Описание</span><span class="sxs-lookup"><span data-stu-id="fadf5-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fadf5-139">classifyAs</span><span class="sxs-lookup"><span data-stu-id="fadf5-139">classifyAs</span></span>|<span data-ttu-id="fadf5-140">string</span><span class="sxs-lookup"><span data-stu-id="fadf5-140">string</span></span>| <span data-ttu-id="fadf5-p105">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="fadf5-p105">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="fadf5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="fadf5-143">Response</span></span>

<span data-ttu-id="fadf5-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fadf5-144">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fadf5-145">Пример</span><span class="sxs-lookup"><span data-stu-id="fadf5-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fadf5-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="fadf5-146">Request</span></span>
<span data-ttu-id="fadf5-147">В следующем примере переопределение для SMTP-адреса randiw@adatum.onmicrosoft.com меняется из `other` на `focused`.</span><span class="sxs-lookup"><span data-stu-id="fadf5-147">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>


# <a name="http"></a>[<span data-ttu-id="fadf5-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="fadf5-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fadf5-149">C#</span><span class="sxs-lookup"><span data-stu-id="fadf5-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fadf5-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fadf5-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fadf5-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fadf5-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fadf5-152">Java</span><span class="sxs-lookup"><span data-stu-id="fadf5-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fadf5-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="fadf5-153">Response</span></span>
<span data-ttu-id="fadf5-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fadf5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


