---
title: Обновление secureScoreControlProfiles
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: b89a5e147d4882dbe25456cd2acc42b56924d12b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817656"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="3e651-104">Обновление secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="3e651-104">Update secureScoreControlProfiles</span></span>

 > <span data-ttu-id="3e651-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e651-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e651-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e651-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e651-107">Обновите свойство редактируемого **secureScoreControlProfiles** в любой интегрированное решение для изменения различных свойств, например **assignedTo** или **tenantNote**.</span><span class="sxs-lookup"><span data-stu-id="3e651-107">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e651-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e651-108">Permissions</span></span>

<span data-ttu-id="3e651-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e651-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e651-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e651-111">Permission type</span></span>      | <span data-ttu-id="3e651-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e651-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e651-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e651-113">Delegated (work or school account)</span></span> |   <span data-ttu-id="3e651-114">SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="3e651-114">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="3e651-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e651-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3e651-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e651-116">Not supported.</span></span>  |
|<span data-ttu-id="3e651-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e651-117">Application</span></span> | <span data-ttu-id="3e651-118">SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="3e651-118">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e651-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e651-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3e651-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e651-120">Request headers</span></span>

| <span data-ttu-id="3e651-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3e651-121">Name</span></span>       | <span data-ttu-id="3e651-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3e651-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3e651-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e651-123">Authorization</span></span>  | <span data-ttu-id="3e651-p104">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e651-p104">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="3e651-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="3e651-126">Prefer</span></span> | <span data-ttu-id="3e651-127">Возвращает = представление.</span><span class="sxs-lookup"><span data-stu-id="3e651-127">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e651-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e651-128">Request body</span></span>

<span data-ttu-id="3e651-129">В тексте запроса укажите представление JSON значений для соответствующие поля, которые должны обновляться.</span><span class="sxs-lookup"><span data-stu-id="3e651-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3e651-130">В следующей таблице приведены поля, которые могут быть обновлены для secureScoreControlProfile.</span><span class="sxs-lookup"><span data-stu-id="3e651-130">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="3e651-131">Значения для существующих свойств, которые не включены в тексте запроса остаются без изменений.</span><span class="sxs-lookup"><span data-stu-id="3e651-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="3e651-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3e651-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e651-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e651-133">Property</span></span>   | <span data-ttu-id="3e651-134">Тип</span><span class="sxs-lookup"><span data-stu-id="3e651-134">Type</span></span> |<span data-ttu-id="3e651-135">Описание</span><span class="sxs-lookup"><span data-stu-id="3e651-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e651-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="3e651-136">assignedTo</span></span>|<span data-ttu-id="3e651-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3e651-137">String</span></span>|<span data-ttu-id="3e651-138">Имя элемента управления аналитик назначается для рассмотрения, реализации или исправления.</span><span class="sxs-lookup"><span data-stu-id="3e651-138">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="3e651-139">tenantNote</span><span class="sxs-lookup"><span data-stu-id="3e651-139">tenantNote</span></span>|<span data-ttu-id="3e651-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3e651-140">String</span></span>|<span data-ttu-id="3e651-141">Комментарии аналитик на элементе управления (для управления клиента).</span><span class="sxs-lookup"><span data-stu-id="3e651-141">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="3e651-142">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="3e651-142">controlStateUpdates</span></span>| <span data-ttu-id="3e651-143">Строка</span><span class="sxs-lookup"><span data-stu-id="3e651-143">String</span></span>|<span data-ttu-id="3e651-144">Аналитик, управляемых с помощью параметра на элементе управления.</span><span class="sxs-lookup"><span data-stu-id="3e651-144">Analyst driven setting on the control.</span></span> <span data-ttu-id="3e651-145">Возможные значения: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="3e651-145">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="3e651-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e651-146">Response</span></span>

<span data-ttu-id="3e651-147">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3e651-147">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="3e651-148">Если используется запрос на необязательный заголовок, метод возвращает `200 OK` код ответа и обновленные [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3e651-148">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e651-149">Пример</span><span class="sxs-lookup"><span data-stu-id="3e651-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e651-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e651-150">Request</span></span>

<span data-ttu-id="3e651-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e651-151">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "assignedTo": "assignedTo-value",
  "controlStateUpdates": "controlStateUpdates-value",
  "tenantNote": "tenantNote-value"
}
```

### <a name="response"></a><span data-ttu-id="3e651-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e651-152">Response</span></span>

<span data-ttu-id="3e651-153">Ниже приведен пример успешного ответа.</span><span class="sxs-lookup"><span data-stu-id="3e651-153">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```




<!-- {
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
