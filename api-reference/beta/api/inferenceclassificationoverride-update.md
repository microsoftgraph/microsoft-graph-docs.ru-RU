---
title: Обновление inferenceClassificationOverride
description: 'Изменение поля **classifyAs** фокус папки "Входящие" переопределять значение, как указано. '
localization_priority: Normal
ms.openlocfilehash: b9d462bc09f69b07d5b6b4bce031932e1b702b44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887908"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="83186-103">Обновление inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="83186-103">Update inferenceClassificationOverride</span></span>

> <span data-ttu-id="83186-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="83186-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83186-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83186-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="83186-106">Изменение поля **classifyAs** [Фокус папки "Входящие"](../resources/manage-focused-inbox.md) переопределять значение, как указано.</span><span class="sxs-lookup"><span data-stu-id="83186-106">Change the **classifyAs** field of a [Focused Inbox](../resources/manage-focused-inbox.md) override as specified.</span></span> 

<span data-ttu-id="83186-107">Вы не можете использовать операцию PATCH, чтобы менять поля в экземпляре [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="83186-107">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span> 

<span data-ttu-id="83186-108">Если для конкретного отправителя существует переопределение и он меняет свое отображаемое имя, вы можете использовать операцию [POST](inferenceclassification-post-overrides.md) для принудительного обновления поля ввода имени в имеющемся переопределении.</span><span class="sxs-lookup"><span data-stu-id="83186-108">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="83186-109">Если для конкретного отправителя существует переопределение и он меняет свой SMTP-адрес, "обновить" переопределение для этого отправителя можно только [удалив](inferenceclassificationoverride-delete.md) существующее переопределение и [создав](inferenceclassification-post-overrides.md) другое с новым SMTP-адресом.</span><span class="sxs-lookup"><span data-stu-id="83186-109">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="83186-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83186-110">Permissions</span></span>
<span data-ttu-id="83186-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83186-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83186-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83186-113">Permission type</span></span>      | <span data-ttu-id="83186-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83186-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83186-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83186-115">Delegated (work or school account)</span></span> | <span data-ttu-id="83186-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83186-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="83186-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83186-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83186-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83186-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="83186-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83186-119">Application</span></span> | <span data-ttu-id="83186-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83186-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="83186-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83186-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="83186-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83186-122">Request headers</span></span>
| <span data-ttu-id="83186-123">Имя</span><span class="sxs-lookup"><span data-stu-id="83186-123">Name</span></span>       | <span data-ttu-id="83186-124">Тип</span><span class="sxs-lookup"><span data-stu-id="83186-124">Type</span></span> | <span data-ttu-id="83186-125">Описание</span><span class="sxs-lookup"><span data-stu-id="83186-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="83186-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="83186-126">Authorization</span></span>  | <span data-ttu-id="83186-127">string</span><span class="sxs-lookup"><span data-stu-id="83186-127">string</span></span>  | <span data-ttu-id="83186-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83186-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83186-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83186-130">Content-Type</span></span> | <span data-ttu-id="83186-131">string</span><span class="sxs-lookup"><span data-stu-id="83186-131">string</span></span>  | <span data-ttu-id="83186-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83186-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83186-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83186-134">Request body</span></span>
<span data-ttu-id="83186-p105">В тексте запроса предоставьте новое значение для поля **classifyAs**. Чтобы производительность была максимальной, не следует включать существующие значения, которые не меняются.</span><span class="sxs-lookup"><span data-stu-id="83186-p105">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="83186-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="83186-137">Property</span></span>     | <span data-ttu-id="83186-138">Тип</span><span class="sxs-lookup"><span data-stu-id="83186-138">Type</span></span>   |<span data-ttu-id="83186-139">Описание</span><span class="sxs-lookup"><span data-stu-id="83186-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83186-140">classifyAs</span><span class="sxs-lookup"><span data-stu-id="83186-140">classifyAs</span></span>|<span data-ttu-id="83186-141">string</span><span class="sxs-lookup"><span data-stu-id="83186-141">string</span></span>| <span data-ttu-id="83186-p106">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="83186-p106">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="83186-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="83186-144">Response</span></span>

<span data-ttu-id="83186-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83186-145">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83186-146">Пример</span><span class="sxs-lookup"><span data-stu-id="83186-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83186-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="83186-147">Request</span></span>
<span data-ttu-id="83186-148">В следующем примере переопределение для SMTP-адреса randiw@adatum.onmicrosoft.com меняется из `other` на `focused`.</span><span class="sxs-lookup"><span data-stu-id="83186-148">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

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
##### <a name="response"></a><span data-ttu-id="83186-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="83186-149">Response</span></span>
<span data-ttu-id="83186-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="83186-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
