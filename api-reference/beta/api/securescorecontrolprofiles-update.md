---
title: Обновление объектов secureScoreControlProfiles
description: Обновление редактируемого свойства Секурескореконтролпрофилес в любом интегрированном решении для изменения различных свойств, таких как assignedTo или Тенантноте.
localization_priority: Normal
ms.openlocfilehash: 711fd29e906822def0a5f4b5fbca13a1d73732d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545649"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="0148f-103">Обновление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="0148f-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0148f-104">Обновление редактируемого свойства **секурескореконтролпрофилес** в любом интегрированном решении для изменения различных свойств, таких как **assignedTo** или **тенантноте**.</span><span class="sxs-lookup"><span data-stu-id="0148f-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="0148f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0148f-105">Permissions</span></span>

<span data-ttu-id="0148f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0148f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0148f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0148f-108">Permission type</span></span>      | <span data-ttu-id="0148f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0148f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0148f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0148f-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="0148f-111">Область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="0148f-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="0148f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0148f-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0148f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0148f-113">Not supported.</span></span>  |
|<span data-ttu-id="0148f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0148f-114">Application</span></span> | <span data-ttu-id="0148f-115">Область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="0148f-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0148f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0148f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0148f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0148f-117">Request headers</span></span>

| <span data-ttu-id="0148f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0148f-118">Name</span></span>       | <span data-ttu-id="0148f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0148f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0148f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0148f-120">Authorization</span></span>  | <span data-ttu-id="0148f-121">Bearer {Code}.</span><span class="sxs-lookup"><span data-stu-id="0148f-121">Bearer {code}.</span></span> <span data-ttu-id="0148f-122">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="0148f-122">Required.</span></span>|
|<span data-ttu-id="0148f-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="0148f-123">Prefer</span></span> | <span data-ttu-id="0148f-124">Возврат = представление.</span><span class="sxs-lookup"><span data-stu-id="0148f-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0148f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0148f-125">Request body</span></span>

<span data-ttu-id="0148f-126">В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0148f-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0148f-127">В следующей таблице перечислены поля, которые можно обновить для Секурескореконтролпрофиле.</span><span class="sxs-lookup"><span data-stu-id="0148f-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="0148f-128">Значения для существующих свойств, не включенных в текст запроса, не изменятся.</span><span class="sxs-lookup"><span data-stu-id="0148f-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="0148f-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0148f-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0148f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0148f-130">Property</span></span>   | <span data-ttu-id="0148f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0148f-131">Type</span></span> |<span data-ttu-id="0148f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0148f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0148f-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="0148f-133">assignedTo</span></span>|<span data-ttu-id="0148f-134">String</span><span class="sxs-lookup"><span data-stu-id="0148f-134">String</span></span>|<span data-ttu-id="0148f-135">Имя аналитики, которой назначен элемент управления для рассмотрения, внедрения или исправления.</span><span class="sxs-lookup"><span data-stu-id="0148f-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="0148f-136">Тенантноте</span><span class="sxs-lookup"><span data-stu-id="0148f-136">tenantNote</span></span>|<span data-ttu-id="0148f-137">String</span><span class="sxs-lookup"><span data-stu-id="0148f-137">String</span></span>|<span data-ttu-id="0148f-138">Комментарии аналитика в элементе управления (для управления клиентом).</span><span class="sxs-lookup"><span data-stu-id="0148f-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="0148f-139">Контролстатеупдатес</span><span class="sxs-lookup"><span data-stu-id="0148f-139">controlStateUpdates</span></span>| <span data-ttu-id="0148f-140">String</span><span class="sxs-lookup"><span data-stu-id="0148f-140">String</span></span>|<span data-ttu-id="0148f-141">Управляемый аналитикой параметр для элемента управления.</span><span class="sxs-lookup"><span data-stu-id="0148f-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="0148f-142">Возможные значения: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="0148f-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="0148f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0148f-143">Response</span></span>

<span data-ttu-id="0148f-144">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0148f-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="0148f-145">Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [секурескореконтролпрофилес](../resources/securescorecontrolprofiles.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0148f-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0148f-146">Пример</span><span class="sxs-lookup"><span data-stu-id="0148f-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="0148f-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="0148f-147">Request</span></span>

<span data-ttu-id="0148f-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0148f-148">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0148f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0148f-149">Response</span></span>

<span data-ttu-id="0148f-150">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="0148f-150">The following is an example of a successful response.</span></span>
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
