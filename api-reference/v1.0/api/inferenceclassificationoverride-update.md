---
title: Обновление объекта inferenceclassificationoverride
description: 'Изменение поля **classifyAs** переопределения указанным образом. '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 985bdfa4646eb9e5145b14337084ec9ce65450fc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806487"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="e046a-103">Обновление объекта inferenceclassificationoverride</span><span class="sxs-lookup"><span data-stu-id="e046a-103">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="e046a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e046a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e046a-105">Изменение поля **classifyAs** переопределения указанным образом.</span><span class="sxs-lookup"><span data-stu-id="e046a-105">Change the **classifyAs** field of an override as specified.</span></span>

<span data-ttu-id="e046a-106">Вы не можете использовать операцию PATCH, чтобы менять поля в экземпляре [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="e046a-106">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span>

<span data-ttu-id="e046a-107">Если для конкретного отправителя существует переопределение и он меняет свое отображаемое имя, вы можете использовать операцию [POST](inferenceclassification-post-overrides.md) для принудительного обновления поля ввода имени в имеющемся переопределении.</span><span class="sxs-lookup"><span data-stu-id="e046a-107">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="e046a-108">Если для конкретного отправителя существует переопределение и он меняет свой SMTP-адрес, "обновить" переопределение для этого отправителя можно только [удалив](inferenceclassificationoverride-delete.md) существующее переопределение и [создав](inferenceclassification-post-overrides.md) другое с новым SMTP-адресом.</span><span class="sxs-lookup"><span data-stu-id="e046a-108">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="e046a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e046a-109">Permissions</span></span>
<span data-ttu-id="e046a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e046a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e046a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e046a-112">Permission type</span></span>      | <span data-ttu-id="e046a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e046a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e046a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e046a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e046a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e046a-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e046a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e046a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e046a-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e046a-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e046a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e046a-118">Application</span></span> | <span data-ttu-id="e046a-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e046a-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e046a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e046a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e046a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e046a-121">Request headers</span></span>
| <span data-ttu-id="e046a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e046a-122">Name</span></span>       | <span data-ttu-id="e046a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e046a-123">Type</span></span> | <span data-ttu-id="e046a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e046a-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e046a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e046a-125">Authorization</span></span>  | <span data-ttu-id="e046a-126">string</span><span class="sxs-lookup"><span data-stu-id="e046a-126">string</span></span>  | <span data-ttu-id="e046a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e046a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e046a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e046a-129">Content-Type</span></span> | <span data-ttu-id="e046a-130">string</span><span class="sxs-lookup"><span data-stu-id="e046a-130">string</span></span>  | <span data-ttu-id="e046a-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e046a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e046a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e046a-133">Request body</span></span>
<span data-ttu-id="e046a-p104">В тексте запроса предоставьте новое значение для поля **classifyAs**. Чтобы производительность была максимальной, не следует включать существующие значения, которые не меняются.</span><span class="sxs-lookup"><span data-stu-id="e046a-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="e046a-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="e046a-136">Property</span></span>     | <span data-ttu-id="e046a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="e046a-137">Type</span></span>   |<span data-ttu-id="e046a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="e046a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e046a-139">classifyAs</span><span class="sxs-lookup"><span data-stu-id="e046a-139">classifyAs</span></span>|<span data-ttu-id="e046a-140">string</span><span class="sxs-lookup"><span data-stu-id="e046a-140">string</span></span>| <span data-ttu-id="e046a-141">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя.</span><span class="sxs-lookup"><span data-stu-id="e046a-141">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="e046a-142">Возможные значения: `focused` , `other` .</span><span class="sxs-lookup"><span data-stu-id="e046a-142">The possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="e046a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e046a-143">Response</span></span>

<span data-ttu-id="e046a-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e046a-144">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e046a-145">Пример</span><span class="sxs-lookup"><span data-stu-id="e046a-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e046a-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e046a-146">Request</span></span>
<span data-ttu-id="e046a-147">В следующем примере переопределение для SMTP-адреса randiw@adatum.onmicrosoft.com меняется из `other` на `focused`.</span><span class="sxs-lookup"><span data-stu-id="e046a-147">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>


# <a name="http"></a>[<span data-ttu-id="e046a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e046a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
# <a name="c"></a>[<span data-ttu-id="e046a-149">C#</span><span class="sxs-lookup"><span data-stu-id="e046a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e046a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e046a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e046a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e046a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e046a-152">Java</span><span class="sxs-lookup"><span data-stu-id="e046a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e046a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e046a-153">Response</span></span>
<span data-ttu-id="e046a-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e046a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
