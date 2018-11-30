---
title: Создание объекта inferenceClassificationOverride
description: 'Создание переопределения для отправителя, определяемую средством SMTP-адрес. Постоянно классификации последующих сообщений от этого SMTP-адреса '
ms.openlocfilehash: f068984598ce841b2e7af52c1ed1d25c0e101d10
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027755"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="c6058-104">Создание объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="c6058-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="c6058-p102">Создание переопределения для отправителя, определенного адресом SMTP. Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.</span><span class="sxs-lookup"><span data-stu-id="c6058-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="c6058-107">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="c6058-107">**Note**</span></span>

- <span data-ttu-id="c6058-108">Если переопределение с таким же SMTP-адресом уже существует, его поля **classifyAs** и **name** будут обновлены с использованием предоставленных значений.</span><span class="sxs-lookup"><span data-stu-id="c6058-108">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="c6058-109">Максимальное количество переопределений, поддерживаемых для почтового ящика, — 1000. Они основываются на уникальных SMTP-адресах отправителей.</span><span class="sxs-lookup"><span data-stu-id="c6058-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="c6058-110">Операция POST поддерживает создание только одного переопределения в один момент времени.</span><span class="sxs-lookup"><span data-stu-id="c6058-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6058-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6058-111">Permissions</span></span>
<span data-ttu-id="c6058-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6058-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6058-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6058-114">Permission type</span></span>      | <span data-ttu-id="c6058-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6058-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6058-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6058-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c6058-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6058-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6058-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6058-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6058-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6058-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6058-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6058-120">Application</span></span> | <span data-ttu-id="c6058-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6058-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6058-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6058-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="c6058-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6058-123">Request headers</span></span>
| <span data-ttu-id="c6058-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c6058-124">Name</span></span>       | <span data-ttu-id="c6058-125">Тип</span><span class="sxs-lookup"><span data-stu-id="c6058-125">Type</span></span> | <span data-ttu-id="c6058-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c6058-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6058-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6058-127">Authorization</span></span>  | <span data-ttu-id="c6058-128">string</span><span class="sxs-lookup"><span data-stu-id="c6058-128">string</span></span>  | <span data-ttu-id="c6058-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6058-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6058-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6058-131">Content-Type</span></span> | <span data-ttu-id="c6058-132">string</span><span class="sxs-lookup"><span data-stu-id="c6058-132">string</span></span>  | <span data-ttu-id="c6058-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6058-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6058-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6058-135">Request body</span></span>
<span data-ttu-id="c6058-136">В тексте запроса предоставьте описание объекта [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6058-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c6058-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6058-137">Response</span></span>

<span data-ttu-id="c6058-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6058-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6058-139">Пример</span><span class="sxs-lookup"><span data-stu-id="c6058-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6058-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6058-140">Request</span></span>
<span data-ttu-id="c6058-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6058-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c6058-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6058-142">Response</span></span>
<span data-ttu-id="c6058-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c6058-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->