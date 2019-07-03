---
title: Обновление объектов secureScoreControlProfiles
description: Обновление редактируемого свойства Секурескореконтролпрофилес в любом интегрированном решении для изменения различных свойств, таких как assignedTo или Тенантноте.
localization_priority: Normal
ms.openlocfilehash: 293d57d3e3d1d1e8a549b71f9ee2514191b76485
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457382"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="060d2-103">Обновление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="060d2-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="060d2-104">Обновление редактируемого свойства **секурескореконтролпрофилес** в любом интегрированном решении для изменения различных свойств, таких как **assignedTo** или **тенантноте**.</span><span class="sxs-lookup"><span data-stu-id="060d2-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="060d2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="060d2-105">Permissions</span></span>

<span data-ttu-id="060d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="060d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="060d2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="060d2-108">Permission type</span></span>      | <span data-ttu-id="060d2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="060d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="060d2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="060d2-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="060d2-111">Область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="060d2-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="060d2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="060d2-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="060d2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="060d2-113">Not supported.</span></span>  |
|<span data-ttu-id="060d2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="060d2-114">Application</span></span> | <span data-ttu-id="060d2-115">Область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="060d2-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="060d2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="060d2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="060d2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="060d2-117">Request headers</span></span>

| <span data-ttu-id="060d2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="060d2-118">Name</span></span>       | <span data-ttu-id="060d2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="060d2-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="060d2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="060d2-120">Authorization</span></span>  | <span data-ttu-id="060d2-121">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="060d2-121">Bearer {code}.</span></span> <span data-ttu-id="060d2-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="060d2-122">Required.</span></span>|
|<span data-ttu-id="060d2-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="060d2-123">Prefer</span></span> | <span data-ttu-id="060d2-124">Возврат = представление.</span><span class="sxs-lookup"><span data-stu-id="060d2-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="060d2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="060d2-125">Request body</span></span>

<span data-ttu-id="060d2-126">В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="060d2-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="060d2-127">В следующей таблице перечислены поля, которые можно обновить для Секурескореконтролпрофиле.</span><span class="sxs-lookup"><span data-stu-id="060d2-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="060d2-128">Значения для существующих свойств, не включенных в текст запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="060d2-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="060d2-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="060d2-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="060d2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="060d2-130">Property</span></span>   | <span data-ttu-id="060d2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="060d2-131">Type</span></span> |<span data-ttu-id="060d2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="060d2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="060d2-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="060d2-133">assignedTo</span></span>|<span data-ttu-id="060d2-134">String</span><span class="sxs-lookup"><span data-stu-id="060d2-134">String</span></span>|<span data-ttu-id="060d2-135">Имя аналитики, которой назначен элемент управления для рассмотрения, внедрения или исправления.</span><span class="sxs-lookup"><span data-stu-id="060d2-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="060d2-136">Тенантноте</span><span class="sxs-lookup"><span data-stu-id="060d2-136">tenantNote</span></span>|<span data-ttu-id="060d2-137">String</span><span class="sxs-lookup"><span data-stu-id="060d2-137">String</span></span>|<span data-ttu-id="060d2-138">Комментарии аналитика в элементе управления (для управления клиентом).</span><span class="sxs-lookup"><span data-stu-id="060d2-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="060d2-139">Контролстатеупдатес</span><span class="sxs-lookup"><span data-stu-id="060d2-139">controlStateUpdates</span></span>| <span data-ttu-id="060d2-140">String</span><span class="sxs-lookup"><span data-stu-id="060d2-140">String</span></span>|<span data-ttu-id="060d2-141">Управляемый аналитикой параметр для элемента управления.</span><span class="sxs-lookup"><span data-stu-id="060d2-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="060d2-142">Возможные значения: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="060d2-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="060d2-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="060d2-143">Response</span></span>

<span data-ttu-id="060d2-144">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="060d2-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="060d2-145">Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [секурескореконтролпрофилес](../resources/securescorecontrolprofiles.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="060d2-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="060d2-146">Пример</span><span class="sxs-lookup"><span data-stu-id="060d2-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="060d2-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="060d2-147">Request</span></span>

<span data-ttu-id="060d2-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="060d2-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="060d2-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="060d2-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="060d2-150">C#</span><span class="sxs-lookup"><span data-stu-id="060d2-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="060d2-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="060d2-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="060d2-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="060d2-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="060d2-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="060d2-153">Response</span></span>

<span data-ttu-id="060d2-154">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="060d2-154">The following is an example of a successful response.</span></span>
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
