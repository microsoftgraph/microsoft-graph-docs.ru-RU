---
title: Обновление объектов secureScoreControlProfiles
description: Обновление редактируемого свойства Секурескореконтролпрофилес в любом интегрированном решении для изменения различных свойств, таких как assignedTo или Тенантноте.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7778a6a8760c368a261154b53b138ec3801701dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453627"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="7bf0f-103">Обновление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="7bf0f-103">Update secureScoreControlProfiles</span></span>

<span data-ttu-id="7bf0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bf0f-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bf0f-105">Обновление редактируемого свойства **секурескореконтролпрофилес** в любом интегрированном решении для изменения различных свойств, таких как **assignedTo** или **тенантноте**.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-105">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bf0f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bf0f-106">Permissions</span></span>

<span data-ttu-id="7bf0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bf0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bf0f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bf0f-109">Permission type</span></span>      | <span data-ttu-id="7bf0f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bf0f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bf0f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bf0f-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="7bf0f-112">Область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-112">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="7bf0f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bf0f-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7bf0f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-114">Not supported.</span></span>  |
|<span data-ttu-id="7bf0f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bf0f-115">Application</span></span> | <span data-ttu-id="7bf0f-116">Область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-116">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bf0f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bf0f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7bf0f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bf0f-118">Request headers</span></span>

| <span data-ttu-id="7bf0f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7bf0f-119">Name</span></span>       | <span data-ttu-id="7bf0f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7bf0f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7bf0f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bf0f-121">Authorization</span></span>  | <span data-ttu-id="7bf0f-122">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-122">Bearer {code}.</span></span> <span data-ttu-id="7bf0f-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-123">Required.</span></span>|
|<span data-ttu-id="7bf0f-124">Prefer</span><span class="sxs-lookup"><span data-stu-id="7bf0f-124">Prefer</span></span> | <span data-ttu-id="7bf0f-125">Возврат = представление.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-125">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bf0f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7bf0f-126">Request body</span></span>

<span data-ttu-id="7bf0f-127">В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-127">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7bf0f-128">В следующей таблице перечислены поля, которые можно обновить для Секурескореконтролпрофиле.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-128">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="7bf0f-129">Значения для существующих свойств, не включенных в текст запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="7bf0f-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7bf0f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bf0f-131">Property</span></span>   | <span data-ttu-id="7bf0f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7bf0f-132">Type</span></span> |<span data-ttu-id="7bf0f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7bf0f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bf0f-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="7bf0f-134">assignedTo</span></span>|<span data-ttu-id="7bf0f-135">String</span><span class="sxs-lookup"><span data-stu-id="7bf0f-135">String</span></span>|<span data-ttu-id="7bf0f-136">Имя аналитики, которой назначен элемент управления для рассмотрения, внедрения или исправления.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-136">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="7bf0f-137">тенантноте</span><span class="sxs-lookup"><span data-stu-id="7bf0f-137">tenantNote</span></span>|<span data-ttu-id="7bf0f-138">String</span><span class="sxs-lookup"><span data-stu-id="7bf0f-138">String</span></span>|<span data-ttu-id="7bf0f-139">Комментарии аналитика в элементе управления (для управления клиентом).</span><span class="sxs-lookup"><span data-stu-id="7bf0f-139">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="7bf0f-140">контролстатеупдатес</span><span class="sxs-lookup"><span data-stu-id="7bf0f-140">controlStateUpdates</span></span>| <span data-ttu-id="7bf0f-141">String</span><span class="sxs-lookup"><span data-stu-id="7bf0f-141">String</span></span>|<span data-ttu-id="7bf0f-142">Управляемый аналитикой параметр для элемента управления.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-142">Analyst driven setting on the control.</span></span> <span data-ttu-id="7bf0f-143">Возможные значения: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-143">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="7bf0f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bf0f-144">Response</span></span>

<span data-ttu-id="7bf0f-145">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-145">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="7bf0f-146">Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [секурескореконтролпрофилес](../resources/securescorecontrolprofiles.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-146">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bf0f-147">Пример</span><span class="sxs-lookup"><span data-stu-id="7bf0f-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bf0f-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bf0f-148">Request</span></span>

<span data-ttu-id="7bf0f-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7bf0f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bf0f-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7bf0f-151">C#</span><span class="sxs-lookup"><span data-stu-id="7bf0f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7bf0f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bf0f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bf0f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bf0f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7bf0f-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bf0f-154">Response</span></span>

<span data-ttu-id="7bf0f-155">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="7bf0f-155">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
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
