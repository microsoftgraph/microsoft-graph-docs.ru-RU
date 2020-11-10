---
title: Создание объекта inferenceClassificationOverride
description: 'Создание переопределения сортировки почты для отправителя, определенного SMTP-адресом. Будущие сообщения с этого SMTP-адреса будут согласованы. '
localization_priority: Normal
doc_type: apiPageType
author: svpsiva
ms.prod: ''
ms.openlocfilehash: 13e12c908701d624c9bb9332977e0fba20cf4146
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953110"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="a179d-104">Создание объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="a179d-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="a179d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a179d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a179d-106">Создание [отсортированного переопределения папки "Входящие"](../resources/manage-focused-inbox.md) для отправителя, определенного SMTP-адресом.</span><span class="sxs-lookup"><span data-stu-id="a179d-106">Create a [Focused Inbox](../resources/manage-focused-inbox.md) override for a sender identified by an SMTP address.</span></span> <span data-ttu-id="a179d-107">Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.</span><span class="sxs-lookup"><span data-stu-id="a179d-107">Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="a179d-108">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="a179d-108">**Note**</span></span>

- <span data-ttu-id="a179d-109">Если переопределение с таким же SMTP-адресом уже существует, то поля **classifyAs** и **Name** этого переопределения обновляются с использованием предоставленных значений.</span><span class="sxs-lookup"><span data-stu-id="a179d-109">If an override already exists with the same SMTP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="a179d-110">Максимальное количество переопределений, поддерживаемых для почтового ящика, — 1000. Они основываются на уникальных SMTP-адресах отправителей.</span><span class="sxs-lookup"><span data-stu-id="a179d-110">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="a179d-111">Операция POST поддерживает создание только одного переопределения в один момент времени.</span><span class="sxs-lookup"><span data-stu-id="a179d-111">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="a179d-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a179d-112">Permissions</span></span>
<span data-ttu-id="a179d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a179d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a179d-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a179d-115">Permission type</span></span>      | <span data-ttu-id="a179d-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a179d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a179d-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a179d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="a179d-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a179d-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a179d-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a179d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a179d-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a179d-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a179d-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a179d-121">Application</span></span> | <span data-ttu-id="a179d-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a179d-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a179d-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a179d-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="a179d-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a179d-124">Request headers</span></span>
| <span data-ttu-id="a179d-125">Имя</span><span class="sxs-lookup"><span data-stu-id="a179d-125">Name</span></span>       | <span data-ttu-id="a179d-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a179d-126">Type</span></span> | <span data-ttu-id="a179d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a179d-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a179d-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a179d-128">Authorization</span></span>  | <span data-ttu-id="a179d-129">string</span><span class="sxs-lookup"><span data-stu-id="a179d-129">string</span></span>  | <span data-ttu-id="a179d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a179d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a179d-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a179d-132">Content-Type</span></span> | <span data-ttu-id="a179d-133">string</span><span class="sxs-lookup"><span data-stu-id="a179d-133">string</span></span>  | <span data-ttu-id="a179d-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a179d-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a179d-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a179d-136">Request body</span></span>
<span data-ttu-id="a179d-137">В тексте запроса предоставьте описание объекта [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a179d-137">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a179d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a179d-138">Response</span></span>

<span data-ttu-id="a179d-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a179d-139">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a179d-140">Пример</span><span class="sxs-lookup"><span data-stu-id="a179d-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a179d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a179d-141">Request</span></span>
<span data-ttu-id="a179d-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a179d-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a179d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a179d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/beta/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="a179d-144">C#</span><span class="sxs-lookup"><span data-stu-id="a179d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-inferenceclassificationoverride-from-inferenceclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a179d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a179d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-inferenceclassificationoverride-from-inferenceclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a179d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a179d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-inferenceclassificationoverride-from-inferenceclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a179d-147">Java</span><span class="sxs-lookup"><span data-stu-id="a179d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-inferenceclassificationoverride-from-inferenceclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a179d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a179d-148">Response</span></span>
<span data-ttu-id="a179d-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a179d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


