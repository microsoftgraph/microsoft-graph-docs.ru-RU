---
title: Обновление объектов secureScoreControlProfiles
description: Обновление редактируемого свойства secureScoreControlProfiles в рамках любого интегрированного решения для изменения различных свойств, например, присвоенныхTo или tenantNote.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 6fee598a91d7153b98ca6e36bb9a21ff949e8b22
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787242"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="304e9-103">Обновление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="304e9-103">Update secureScoreControlProfiles</span></span>

<span data-ttu-id="304e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="304e9-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="304e9-105">Обновление редактируемого **свойства secureScoreControlProfiles** в рамках любого интегрированного решения для изменения различных свойств, например, присвоенныхTo или **tenantNote.** </span><span class="sxs-lookup"><span data-stu-id="304e9-105">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="304e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="304e9-106">Permissions</span></span>

<span data-ttu-id="304e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="304e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="304e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="304e9-109">Permission type</span></span>      | <span data-ttu-id="304e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="304e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="304e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="304e9-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="304e9-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304e9-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="304e9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="304e9-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="304e9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="304e9-114">Not supported.</span></span>  |
|<span data-ttu-id="304e9-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="304e9-115">Application</span></span> | <span data-ttu-id="304e9-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304e9-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="304e9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="304e9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="304e9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="304e9-118">Request headers</span></span>

| <span data-ttu-id="304e9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="304e9-119">Name</span></span>       | <span data-ttu-id="304e9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="304e9-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="304e9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="304e9-121">Authorization</span></span>  | <span data-ttu-id="304e9-122">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="304e9-122">Bearer {code}.</span></span> <span data-ttu-id="304e9-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="304e9-123">Required.</span></span>|
|<span data-ttu-id="304e9-124">Prefer</span><span class="sxs-lookup"><span data-stu-id="304e9-124">Prefer</span></span> | <span data-ttu-id="304e9-125">return=representation.</span><span class="sxs-lookup"><span data-stu-id="304e9-125">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="304e9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="304e9-126">Request body</span></span>

<span data-ttu-id="304e9-127">В теле запроса поставляем представление JSON значений для соответствующих полей, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="304e9-127">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="304e9-128">В следующей таблице перечислены поля, которые можно обновить для secureScoreControlProfile.</span><span class="sxs-lookup"><span data-stu-id="304e9-128">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="304e9-129">Значения для существующих свойств, не включенных в тело запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="304e9-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="304e9-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="304e9-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="304e9-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="304e9-131">Property</span></span>   | <span data-ttu-id="304e9-132">Тип</span><span class="sxs-lookup"><span data-stu-id="304e9-132">Type</span></span> |<span data-ttu-id="304e9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="304e9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="304e9-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="304e9-134">assignedTo</span></span>|<span data-ttu-id="304e9-135">String</span><span class="sxs-lookup"><span data-stu-id="304e9-135">String</span></span>|<span data-ttu-id="304e9-136">Имя аналитика, на который назначен контроль для выполнения, выполнения или устранения.</span><span class="sxs-lookup"><span data-stu-id="304e9-136">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="304e9-137">tenantNote</span><span class="sxs-lookup"><span data-stu-id="304e9-137">tenantNote</span></span>|<span data-ttu-id="304e9-138">String</span><span class="sxs-lookup"><span data-stu-id="304e9-138">String</span></span>|<span data-ttu-id="304e9-139">Аналитик комментирует управление (для управления клиентом).</span><span class="sxs-lookup"><span data-stu-id="304e9-139">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="304e9-140">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="304e9-140">controlStateUpdates</span></span>| <span data-ttu-id="304e9-141">String</span><span class="sxs-lookup"><span data-stu-id="304e9-141">String</span></span>|<span data-ttu-id="304e9-142">Параметр управления, управляемый аналитиком.</span><span class="sxs-lookup"><span data-stu-id="304e9-142">Analyst driven setting on the control.</span></span> <span data-ttu-id="304e9-143">Возможные значения: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="304e9-143">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="304e9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="304e9-144">Response</span></span>

<span data-ttu-id="304e9-145">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="304e9-145">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="304e9-146">Если используется необязательный заголовок запроса, метод возвращает код ответа и обновленный объект `200 OK` [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="304e9-146">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="304e9-147">Пример</span><span class="sxs-lookup"><span data-stu-id="304e9-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="304e9-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="304e9-148">Request</span></span>

<span data-ttu-id="304e9-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="304e9-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="304e9-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="304e9-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "controlStateUpdates": "controlStateUpdates-value"
}
```
# <a name="c"></a>[<span data-ttu-id="304e9-151">C#</span><span class="sxs-lookup"><span data-stu-id="304e9-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="304e9-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="304e9-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="304e9-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="304e9-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="304e9-154">Java</span><span class="sxs-lookup"><span data-stu-id="304e9-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescorecontrolprofiles-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="304e9-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="304e9-155">Response</span></span>

<span data-ttu-id="304e9-156">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="304e9-156">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```




<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


