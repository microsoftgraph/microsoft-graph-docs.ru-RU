---
title: Обновление educationAssignmentSettings
description: Обновление свойств объекта educationAssignmentSettings.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7c251885de43022f8e3065c7004dab33d4fa78a8
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992979"
---
# <a name="update-educationassignmentsettings"></a><span data-ttu-id="41b2b-103">Обновление educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="41b2b-103">Update educationAssignmentSettings</span></span>
<span data-ttu-id="41b2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41b2b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41b2b-105">Обновление свойств объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="41b2b-105">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span> <span data-ttu-id="41b2b-106">Только Учителя могут обновлять эти параметры.</span><span class="sxs-lookup"><span data-stu-id="41b2b-106">Only Teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="41b2b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41b2b-107">Permissions</span></span>
<span data-ttu-id="41b2b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41b2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41b2b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41b2b-110">Permission type</span></span>|<span data-ttu-id="41b2b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41b2b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41b2b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41b2b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41b2b-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41b2b-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="41b2b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41b2b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41b2b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41b2b-115">Not supported.</span></span>|
|<span data-ttu-id="41b2b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41b2b-116">Application</span></span>|<span data-ttu-id="41b2b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41b2b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41b2b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41b2b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

## <a name="request-headers"></a><span data-ttu-id="41b2b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41b2b-119">Request headers</span></span>
|<span data-ttu-id="41b2b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="41b2b-120">Name</span></span>|<span data-ttu-id="41b2b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="41b2b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="41b2b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41b2b-122">Authorization</span></span>|<span data-ttu-id="41b2b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41b2b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="41b2b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41b2b-125">Content-Type</span></span>|<span data-ttu-id="41b2b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41b2b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41b2b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41b2b-128">Request body</span></span>
<span data-ttu-id="41b2b-129">В теле запроса поставляют представление JSON объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="41b2b-129">In the request body, supply a JSON representation of the [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

<span data-ttu-id="41b2b-130">В следующей таблице показаны свойства, необходимые при обновлении [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="41b2b-130">The following table shows the properties that are required when you update the [educationAssignmentSettings](../resources/educationassignmentsettings.md).</span></span>

|<span data-ttu-id="41b2b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="41b2b-131">Property</span></span>|<span data-ttu-id="41b2b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="41b2b-132">Type</span></span>|<span data-ttu-id="41b2b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="41b2b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41b2b-134">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="41b2b-134">submissionAnimationDisabled</span></span>|<span data-ttu-id="41b2b-135">Логический</span><span class="sxs-lookup"><span data-stu-id="41b2b-135">Boolean</span></span>|<span data-ttu-id="41b2b-136">Указывает, будет ли показана анимация празднования по очереди.</span><span class="sxs-lookup"><span data-stu-id="41b2b-136">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="41b2b-137">Значение `true` указывает, что анимация не будет показана.</span><span class="sxs-lookup"><span data-stu-id="41b2b-137">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="41b2b-138">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="41b2b-138">Default value is `false`.</span></span>|



## <a name="response"></a><span data-ttu-id="41b2b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="41b2b-139">Response</span></span>

<span data-ttu-id="41b2b-140">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="41b2b-140">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41b2b-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="41b2b-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41b2b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="41b2b-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="41b2b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="41b2b-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
Content-Type: application/json
Content-length: 114

{
  "submissionAnimationDisabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="41b2b-144">C#</span><span class="sxs-lookup"><span data-stu-id="41b2b-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41b2b-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41b2b-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41b2b-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41b2b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41b2b-147">Java</span><span class="sxs-lookup"><span data-stu-id="41b2b-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41b2b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="41b2b-148">Response</span></span>
<span data-ttu-id="41b2b-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="41b2b-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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

