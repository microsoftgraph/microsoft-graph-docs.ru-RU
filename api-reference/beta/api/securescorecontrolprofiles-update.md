---
title: Обновление объектов secureScoreControlProfiles
description: Обновление редактируемого свойства Секурескореконтролпрофилес в любом интегрированном решении для изменения различных свойств, таких как assignedTo или Тенантноте.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 6d3df08c36a7a59e4502164ac1f89c85268d0a01
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330195"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="f4a17-103">Обновление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="f4a17-103">Update secureScoreControlProfiles</span></span>

<span data-ttu-id="f4a17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4a17-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4a17-105">Обновление редактируемого свойства **секурескореконтролпрофилес** в любом интегрированном решении для изменения различных свойств, таких как **assignedTo** или **тенантноте**.</span><span class="sxs-lookup"><span data-stu-id="f4a17-105">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4a17-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4a17-106">Permissions</span></span>

<span data-ttu-id="f4a17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4a17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4a17-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4a17-109">Permission type</span></span>      | <span data-ttu-id="f4a17-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4a17-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4a17-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4a17-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="f4a17-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a17-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="f4a17-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4a17-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f4a17-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4a17-114">Not supported.</span></span>  |
|<span data-ttu-id="f4a17-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f4a17-115">Application</span></span> | <span data-ttu-id="f4a17-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a17-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4a17-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4a17-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f4a17-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4a17-118">Request headers</span></span>

| <span data-ttu-id="f4a17-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f4a17-119">Name</span></span>       | <span data-ttu-id="f4a17-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f4a17-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f4a17-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4a17-121">Authorization</span></span>  | <span data-ttu-id="f4a17-122">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="f4a17-122">Bearer {code}.</span></span> <span data-ttu-id="f4a17-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f4a17-123">Required.</span></span>|
|<span data-ttu-id="f4a17-124">Prefer</span><span class="sxs-lookup"><span data-stu-id="f4a17-124">Prefer</span></span> | <span data-ttu-id="f4a17-125">Возврат = представление.</span><span class="sxs-lookup"><span data-stu-id="f4a17-125">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4a17-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4a17-126">Request body</span></span>

<span data-ttu-id="f4a17-127">В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f4a17-127">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f4a17-128">В следующей таблице перечислены поля, которые можно обновить для Секурескореконтролпрофиле.</span><span class="sxs-lookup"><span data-stu-id="f4a17-128">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="f4a17-129">Значения для существующих свойств, не включенных в текст запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="f4a17-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="f4a17-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f4a17-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f4a17-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4a17-131">Property</span></span>   | <span data-ttu-id="f4a17-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f4a17-132">Type</span></span> |<span data-ttu-id="f4a17-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f4a17-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4a17-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="f4a17-134">assignedTo</span></span>|<span data-ttu-id="f4a17-135">String</span><span class="sxs-lookup"><span data-stu-id="f4a17-135">String</span></span>|<span data-ttu-id="f4a17-136">Имя аналитики, которой назначен элемент управления для рассмотрения, внедрения или исправления.</span><span class="sxs-lookup"><span data-stu-id="f4a17-136">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="f4a17-137">тенантноте</span><span class="sxs-lookup"><span data-stu-id="f4a17-137">tenantNote</span></span>|<span data-ttu-id="f4a17-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f4a17-138">String</span></span>|<span data-ttu-id="f4a17-139">Комментарии аналитика в элементе управления (для управления клиентом).</span><span class="sxs-lookup"><span data-stu-id="f4a17-139">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="f4a17-140">контролстатеупдатес</span><span class="sxs-lookup"><span data-stu-id="f4a17-140">controlStateUpdates</span></span>| <span data-ttu-id="f4a17-141">Строка</span><span class="sxs-lookup"><span data-stu-id="f4a17-141">String</span></span>|<span data-ttu-id="f4a17-142">Управляемый аналитикой параметр для элемента управления.</span><span class="sxs-lookup"><span data-stu-id="f4a17-142">Analyst driven setting on the control.</span></span> <span data-ttu-id="f4a17-143">Возможные значения: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="f4a17-143">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="f4a17-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4a17-144">Response</span></span>

<span data-ttu-id="f4a17-145">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f4a17-145">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="f4a17-146">Если используется заголовок необязательного запроса, метод возвращает `200 OK` код отклика и обновленный объект [секурескореконтролпрофилес](../resources/securescorecontrolprofiles.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4a17-146">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4a17-147">Пример</span><span class="sxs-lookup"><span data-stu-id="f4a17-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4a17-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4a17-148">Request</span></span>

<span data-ttu-id="f4a17-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4a17-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4a17-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4a17-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f4a17-151">C#</span><span class="sxs-lookup"><span data-stu-id="f4a17-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4a17-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4a17-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4a17-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4a17-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f4a17-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4a17-154">Response</span></span>

<span data-ttu-id="f4a17-155">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="f4a17-155">The following is an example of a successful response.</span></span>
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


