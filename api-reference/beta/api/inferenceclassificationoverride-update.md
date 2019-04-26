---
title: Обновление inferenceClassificationOverride
description: 'Измените значение поля **classifyAs** для параметра отсортированное переопределение, как указано. '
localization_priority: Normal
ms.openlocfilehash: 2a51f482df6df1672182e773ea07290eef9c66dc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323718"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="28440-103">Обновление inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="28440-103">Update inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28440-104">Измените значение поля **classifyAs** для параметра [отсортированное](../resources/manage-focused-inbox.md) переопределение, как указано.</span><span class="sxs-lookup"><span data-stu-id="28440-104">Change the **classifyAs** field of a [Focused Inbox](../resources/manage-focused-inbox.md) override as specified.</span></span> 

<span data-ttu-id="28440-105">Вы не можете использовать операцию PATCH, чтобы менять поля в экземпляре [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="28440-105">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span> 

<span data-ttu-id="28440-106">Если для конкретного отправителя существует переопределение и он меняет свое отображаемое имя, вы можете использовать операцию [POST](inferenceclassification-post-overrides.md) для принудительного обновления поля ввода имени в имеющемся переопределении.</span><span class="sxs-lookup"><span data-stu-id="28440-106">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="28440-107">Если для конкретного отправителя существует переопределение и он меняет свой SMTP-адрес, "обновить" переопределение для этого отправителя можно только [удалив](inferenceclassificationoverride-delete.md) существующее переопределение и [создав](inferenceclassification-post-overrides.md) другое с новым SMTP-адресом.</span><span class="sxs-lookup"><span data-stu-id="28440-107">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="28440-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28440-108">Permissions</span></span>
<span data-ttu-id="28440-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28440-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28440-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28440-111">Permission type</span></span>      | <span data-ttu-id="28440-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28440-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28440-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28440-113">Delegated (work or school account)</span></span> | <span data-ttu-id="28440-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28440-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="28440-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28440-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28440-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28440-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="28440-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28440-117">Application</span></span> | <span data-ttu-id="28440-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28440-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="28440-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28440-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="28440-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28440-120">Request headers</span></span>
| <span data-ttu-id="28440-121">Имя</span><span class="sxs-lookup"><span data-stu-id="28440-121">Name</span></span>       | <span data-ttu-id="28440-122">Тип</span><span class="sxs-lookup"><span data-stu-id="28440-122">Type</span></span> | <span data-ttu-id="28440-123">Описание</span><span class="sxs-lookup"><span data-stu-id="28440-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="28440-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="28440-124">Authorization</span></span>  | <span data-ttu-id="28440-125">строка</span><span class="sxs-lookup"><span data-stu-id="28440-125">string</span></span>  | <span data-ttu-id="28440-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28440-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28440-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28440-128">Content-Type</span></span> | <span data-ttu-id="28440-129">string</span><span class="sxs-lookup"><span data-stu-id="28440-129">string</span></span>  | <span data-ttu-id="28440-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28440-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28440-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28440-132">Request body</span></span>
<span data-ttu-id="28440-p104">В тексте запроса предоставьте новое значение для поля **classifyAs**. Чтобы производительность была максимальной, не следует включать существующие значения, которые не меняются.</span><span class="sxs-lookup"><span data-stu-id="28440-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="28440-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="28440-135">Property</span></span>     | <span data-ttu-id="28440-136">Тип</span><span class="sxs-lookup"><span data-stu-id="28440-136">Type</span></span>   |<span data-ttu-id="28440-137">Описание</span><span class="sxs-lookup"><span data-stu-id="28440-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28440-138">classifyAs</span><span class="sxs-lookup"><span data-stu-id="28440-138">classifyAs</span></span>|<span data-ttu-id="28440-139">string</span><span class="sxs-lookup"><span data-stu-id="28440-139">string</span></span>| <span data-ttu-id="28440-p105">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="28440-p105">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="28440-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="28440-142">Response</span></span>

<span data-ttu-id="28440-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28440-143">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28440-144">Пример</span><span class="sxs-lookup"><span data-stu-id="28440-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28440-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="28440-145">Request</span></span>
<span data-ttu-id="28440-146">В следующем примере переопределение для SMTP-адреса randiw@adatum.onmicrosoft.com меняется из `other` на `focused`.</span><span class="sxs-lookup"><span data-stu-id="28440-146">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

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
##### <a name="response"></a><span data-ttu-id="28440-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="28440-147">Response</span></span>
<span data-ttu-id="28440-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28440-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
