---
title: Обновление secureScoreControlProfiles
description: Обновите свойство редактируемого secureScoreControlProfiles в любой интегрированное решение для изменения различных свойств, например assignedTo или tenantNote.
localization_priority: Normal
ms.openlocfilehash: 711fd29e906822def0a5f4b5fbca13a1d73732d6
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642032"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="ee451-103">Обновление secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="ee451-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee451-104">Обновите свойство редактируемого **secureScoreControlProfiles** в любой интегрированное решение для изменения различных свойств, например **assignedTo** или **tenantNote**.</span><span class="sxs-lookup"><span data-stu-id="ee451-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee451-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee451-105">Permissions</span></span>

<span data-ttu-id="ee451-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee451-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee451-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee451-108">Permission type</span></span>      | <span data-ttu-id="ee451-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee451-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee451-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee451-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="ee451-111">SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="ee451-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="ee451-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee451-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ee451-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee451-113">Not supported.</span></span>  |
|<span data-ttu-id="ee451-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee451-114">Application</span></span> | <span data-ttu-id="ee451-115">SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="ee451-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee451-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee451-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ee451-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee451-117">Request headers</span></span>

| <span data-ttu-id="ee451-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ee451-118">Name</span></span>       | <span data-ttu-id="ee451-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ee451-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ee451-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee451-120">Authorization</span></span>  | <span data-ttu-id="ee451-p102">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee451-p102">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="ee451-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="ee451-123">Prefer</span></span> | <span data-ttu-id="ee451-124">Возвращает = представление.</span><span class="sxs-lookup"><span data-stu-id="ee451-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee451-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee451-125">Request body</span></span>

<span data-ttu-id="ee451-126">В тексте запроса укажите представление JSON значений для соответствующие поля, которые должны обновляться.</span><span class="sxs-lookup"><span data-stu-id="ee451-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ee451-127">В следующей таблице приведены поля, которые могут быть обновлены для secureScoreControlProfile.</span><span class="sxs-lookup"><span data-stu-id="ee451-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="ee451-128">Значения для существующих свойств, которые не включены в тексте запроса остаются без изменений.</span><span class="sxs-lookup"><span data-stu-id="ee451-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="ee451-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ee451-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ee451-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee451-130">Property</span></span>   | <span data-ttu-id="ee451-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ee451-131">Type</span></span> |<span data-ttu-id="ee451-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ee451-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee451-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="ee451-133">assignedTo</span></span>|<span data-ttu-id="ee451-134">String</span><span class="sxs-lookup"><span data-stu-id="ee451-134">String</span></span>|<span data-ttu-id="ee451-135">Имя элемента управления аналитик назначается для рассмотрения, реализации или исправления.</span><span class="sxs-lookup"><span data-stu-id="ee451-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="ee451-136">tenantNote</span><span class="sxs-lookup"><span data-stu-id="ee451-136">tenantNote</span></span>|<span data-ttu-id="ee451-137">String</span><span class="sxs-lookup"><span data-stu-id="ee451-137">String</span></span>|<span data-ttu-id="ee451-138">Комментарии аналитик на элементе управления (для управления клиента).</span><span class="sxs-lookup"><span data-stu-id="ee451-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="ee451-139">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="ee451-139">controlStateUpdates</span></span>| <span data-ttu-id="ee451-140">String</span><span class="sxs-lookup"><span data-stu-id="ee451-140">String</span></span>|<span data-ttu-id="ee451-141">Аналитик, управляемых с помощью параметра на элементе управления.</span><span class="sxs-lookup"><span data-stu-id="ee451-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="ee451-142">Возможные значения: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="ee451-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="ee451-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee451-143">Response</span></span>

<span data-ttu-id="ee451-144">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ee451-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="ee451-145">Если используется запрос на необязательный заголовок, метод возвращает `200 OK` код ответа и обновленные [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ee451-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee451-146">Пример</span><span class="sxs-lookup"><span data-stu-id="ee451-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee451-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee451-147">Request</span></span>

<span data-ttu-id="ee451-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee451-148">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee451-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee451-149">Response</span></span>

<span data-ttu-id="ee451-150">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="ee451-150">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
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
    "Error: /api-reference/beta/api/securescorecontrolprofiles-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
