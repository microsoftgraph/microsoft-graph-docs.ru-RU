---
title: Создание объекта inferenceClassificationOverride
description: 'Создание переопределения фокус папки "Входящие" для отправителя, определяемую средством SMTP-адрес. Постоянно классификации последующих сообщений от этого SMTP-адреса '
ms.openlocfilehash: e15793bc8c7012628659144bd503bd8cf979ef61
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077599"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="79210-104">Создание объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="79210-104">Create inferenceClassificationOverride</span></span>

> <span data-ttu-id="79210-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="79210-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79210-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79210-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79210-107">Создание переопределения [Фокус папки "Входящие"](../resources/manage-focused-inbox.md) для отправителя, определяемую средством SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="79210-107">Create a [Focused Inbox](../resources/manage-focused-inbox.md) override for a sender identified by an SMTP address.</span></span> <span data-ttu-id="79210-108">Будущее сообщений из SMTP-адреса постоянно классифицируются как указано в переопределении.</span><span class="sxs-lookup"><span data-stu-id="79210-108">Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="79210-109">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="79210-109">**Note**</span></span>

- <span data-ttu-id="79210-110">Если переопределение с таким же SMTP-адресом уже существует, его поля **classifyAs** и **name** будут обновлены с использованием предоставленных значений.</span><span class="sxs-lookup"><span data-stu-id="79210-110">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="79210-111">Максимальное количество переопределений, поддерживаемых для почтового ящика, — 1000. Они основываются на уникальных SMTP-адресах отправителей.</span><span class="sxs-lookup"><span data-stu-id="79210-111">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="79210-112">Операция POST поддерживает создание только одного переопределения в один момент времени.</span><span class="sxs-lookup"><span data-stu-id="79210-112">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="79210-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79210-113">Permissions</span></span>
<span data-ttu-id="79210-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79210-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79210-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79210-116">Permission type</span></span>      | <span data-ttu-id="79210-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79210-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79210-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79210-118">Delegated (work or school account)</span></span> | <span data-ttu-id="79210-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79210-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="79210-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79210-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79210-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79210-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="79210-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79210-122">Application</span></span> | <span data-ttu-id="79210-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79210-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="79210-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79210-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="79210-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79210-125">Request headers</span></span>
| <span data-ttu-id="79210-126">Имя</span><span class="sxs-lookup"><span data-stu-id="79210-126">Name</span></span>       | <span data-ttu-id="79210-127">Тип</span><span class="sxs-lookup"><span data-stu-id="79210-127">Type</span></span> | <span data-ttu-id="79210-128">Описание</span><span class="sxs-lookup"><span data-stu-id="79210-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="79210-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="79210-129">Authorization</span></span>  | <span data-ttu-id="79210-130">string</span><span class="sxs-lookup"><span data-stu-id="79210-130">string</span></span>  | <span data-ttu-id="79210-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79210-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79210-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79210-133">Content-Type</span></span> | <span data-ttu-id="79210-134">string</span><span class="sxs-lookup"><span data-stu-id="79210-134">string</span></span>  | <span data-ttu-id="79210-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79210-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79210-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79210-137">Request body</span></span>
<span data-ttu-id="79210-138">В тексте запроса предоставьте описание объекта [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79210-138">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="79210-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="79210-139">Response</span></span>

<span data-ttu-id="79210-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79210-140">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79210-141">Пример</span><span class="sxs-lookup"><span data-stu-id="79210-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79210-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="79210-142">Request</span></span>
<span data-ttu-id="79210-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79210-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="79210-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="79210-144">Response</span></span>
<span data-ttu-id="79210-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="79210-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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