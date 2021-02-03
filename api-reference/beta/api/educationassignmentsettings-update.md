---
title: Обновление educationAssignmentSettings
description: Обновление свойств объекта educationAssignmentSettings.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ec19c4e3f49c5535e6ed5f4eddafbbf21d5428ee
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092520"
---
# <a name="update-educationassignmentsettings"></a><span data-ttu-id="68df8-103">Обновление educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="68df8-103">Update educationAssignmentSettings</span></span>
<span data-ttu-id="68df8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68df8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68df8-105">Обновление свойств объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="68df8-105">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span> <span data-ttu-id="68df8-106">Только преподаватели могут обновлять эти параметры.</span><span class="sxs-lookup"><span data-stu-id="68df8-106">Only Teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="68df8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68df8-107">Permissions</span></span>
<span data-ttu-id="68df8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68df8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68df8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68df8-110">Permission type</span></span>|<span data-ttu-id="68df8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68df8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68df8-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68df8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68df8-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68df8-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="68df8-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68df8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68df8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68df8-115">Not supported.</span></span>|
|<span data-ttu-id="68df8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68df8-116">Application</span></span>|<span data-ttu-id="68df8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68df8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68df8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68df8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/{id}/assignmentSettings
```

## <a name="request-headers"></a><span data-ttu-id="68df8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68df8-119">Request headers</span></span>
|<span data-ttu-id="68df8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="68df8-120">Name</span></span>|<span data-ttu-id="68df8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="68df8-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="68df8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68df8-122">Authorization</span></span>|<span data-ttu-id="68df8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68df8-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="68df8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68df8-125">Content-Type</span></span>|<span data-ttu-id="68df8-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68df8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68df8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68df8-128">Request body</span></span>
<span data-ttu-id="68df8-129">В теле запроса укажу представление объекта [educationAssignmentSettings](../resources/educationassignmentsettings.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="68df8-129">In the request body, supply a JSON representation of the [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

<span data-ttu-id="68df8-130">В следующей таблице показаны свойства, необходимые при обновлении [объекта educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="68df8-130">The following table shows the properties that are required when you update the [educationAssignmentSettings](../resources/educationassignmentsettings.md).</span></span>

|<span data-ttu-id="68df8-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="68df8-131">Property</span></span>|<span data-ttu-id="68df8-132">Тип</span><span class="sxs-lookup"><span data-stu-id="68df8-132">Type</span></span>|<span data-ttu-id="68df8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="68df8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68df8-134">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="68df8-134">submissionAnimationDisabled</span></span>|<span data-ttu-id="68df8-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="68df8-135">Boolean</span></span>|<span data-ttu-id="68df8-136">Указывает, будет ли показана анимация поозднения.</span><span class="sxs-lookup"><span data-stu-id="68df8-136">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="68df8-137">Значение `true` указывает, что анимация не будет показана.</span><span class="sxs-lookup"><span data-stu-id="68df8-137">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="68df8-138">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="68df8-138">Default value is `false`.</span></span>|



## <a name="response"></a><span data-ttu-id="68df8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="68df8-139">Response</span></span>

<span data-ttu-id="68df8-140">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68df8-140">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68df8-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="68df8-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68df8-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="68df8-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="68df8-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="68df8-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
Content-Type: application/json
Content-length: 114

{
  "submissionAnimationDisabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="68df8-144">C#</span><span class="sxs-lookup"><span data-stu-id="68df8-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68df8-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68df8-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68df8-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68df8-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68df8-147">Java</span><span class="sxs-lookup"><span data-stu-id="68df8-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="68df8-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="68df8-148">Response</span></span>
<span data-ttu-id="68df8-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="68df8-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "submissionAnimationDisabled": true
}
```

