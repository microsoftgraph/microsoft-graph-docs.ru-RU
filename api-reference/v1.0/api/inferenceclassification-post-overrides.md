---
title: Создание объекта inferenceClassificationOverride
description: 'Создание переопределения для отправителя, указанному по SMTP-адресу. Будущие сообщения с этого SMTP-адреса будут согласованы. '
localization_priority: Normal
ms.openlocfilehash: 5a3972a9c8a86f6bf49c892511a05e398427f33a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880838"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="9e67d-104">Создание объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="9e67d-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="9e67d-p102">Создание переопределения для отправителя, определенного адресом SMTP. Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.</span><span class="sxs-lookup"><span data-stu-id="9e67d-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="9e67d-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="9e67d-107">**Note**</span></span>

- <span data-ttu-id="9e67d-108">Если переопределение с таким же SMTP-адресом уже существует, его поля **classifyAs** и **name** будут обновлены с использованием предоставленных значений.</span><span class="sxs-lookup"><span data-stu-id="9e67d-108">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="9e67d-109">Максимальное количество переопределений, поддерживаемых для почтового ящика, — 1000. Они основываются на уникальных SMTP-адресах отправителей.</span><span class="sxs-lookup"><span data-stu-id="9e67d-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="9e67d-110">Операция POST поддерживает создание только одного переопределения в один момент времени.</span><span class="sxs-lookup"><span data-stu-id="9e67d-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e67d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e67d-111">Permissions</span></span>
<span data-ttu-id="9e67d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e67d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e67d-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e67d-114">Permission type</span></span>      | <span data-ttu-id="9e67d-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e67d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e67d-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e67d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="9e67d-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e67d-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9e67d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e67d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e67d-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e67d-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9e67d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e67d-120">Application</span></span> | <span data-ttu-id="9e67d-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e67d-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e67d-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e67d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="9e67d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e67d-123">Request headers</span></span>
| <span data-ttu-id="9e67d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="9e67d-124">Name</span></span>       | <span data-ttu-id="9e67d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9e67d-125">Type</span></span> | <span data-ttu-id="9e67d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9e67d-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9e67d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e67d-127">Authorization</span></span>  | <span data-ttu-id="9e67d-128">string</span><span class="sxs-lookup"><span data-stu-id="9e67d-128">string</span></span>  | <span data-ttu-id="9e67d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e67d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9e67d-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e67d-131">Content-Type</span></span> | <span data-ttu-id="9e67d-132">string</span><span class="sxs-lookup"><span data-stu-id="9e67d-132">string</span></span>  | <span data-ttu-id="9e67d-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e67d-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e67d-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e67d-135">Request body</span></span>
<span data-ttu-id="9e67d-136">В тексте запроса предоставьте описание объекта [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e67d-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9e67d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e67d-137">Response</span></span>

<span data-ttu-id="9e67d-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e67d-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e67d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="9e67d-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e67d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e67d-140">Request</span></span>
<span data-ttu-id="9e67d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e67d-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9e67d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e67d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9e67d-143">C#</span><span class="sxs-lookup"><span data-stu-id="9e67d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-inferenceclassificationoverride-from-inferenceclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e67d-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="9e67d-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-inferenceclassificationoverride-from-inferenceclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9e67d-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9e67d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-inferenceclassificationoverride-from-inferenceclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9e67d-146">Java</span><span class="sxs-lookup"><span data-stu-id="9e67d-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-inferenceclassificationoverride-from-inferenceclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9e67d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e67d-147">Response</span></span>
<span data-ttu-id="9e67d-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e67d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
