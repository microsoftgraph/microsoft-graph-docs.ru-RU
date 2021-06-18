---
title: Обновление educationAssignmentDefaults
description: Обновление свойств объекта educationAssignmentDefaults.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 57054d86e683fd91ffacc1f601d549405ffa5c17
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991026"
---
# <a name="update-educationassignmentdefaults"></a><span data-ttu-id="d9db8-103">Обновление educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="d9db8-103">Update educationAssignmentDefaults</span></span>
<span data-ttu-id="d9db8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9db8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9db8-105">Обновление свойств объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="d9db8-105">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>

<span data-ttu-id="d9db8-106">Только преподаватели могут обновлять эти параметры.</span><span class="sxs-lookup"><span data-stu-id="d9db8-106">Only teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9db8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9db8-107">Permissions</span></span>
<span data-ttu-id="d9db8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9db8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9db8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9db8-110">Permission type</span></span>|<span data-ttu-id="d9db8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9db8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9db8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9db8-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="d9db8-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9db8-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d9db8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9db8-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d9db8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9db8-115">Not supported.</span></span>  |
|<span data-ttu-id="d9db8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9db8-116">Application</span></span> | <span data-ttu-id="d9db8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9db8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9db8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9db8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
```

## <a name="request-headers"></a><span data-ttu-id="d9db8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9db8-119">Request headers</span></span>
|<span data-ttu-id="d9db8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d9db8-120">Name</span></span>|<span data-ttu-id="d9db8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d9db8-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d9db8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9db8-122">Authorization</span></span>|<span data-ttu-id="d9db8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9db8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d9db8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9db8-125">Content-Type</span></span>|<span data-ttu-id="d9db8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9db8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9db8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9db8-128">Request body</span></span>
<span data-ttu-id="d9db8-129">В теле запроса поставляют только значения полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d9db8-129">In the request body, supply only the values of the fields you want to update.</span></span>

<span data-ttu-id="d9db8-130">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="d9db8-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d9db8-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d9db8-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="d9db8-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9db8-132">Property</span></span>|<span data-ttu-id="d9db8-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d9db8-133">Type</span></span>|<span data-ttu-id="d9db8-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d9db8-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9db8-135">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="d9db8-135">addedStudentAction</span></span>|<span data-ttu-id="d9db8-136">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="d9db8-136">educationAddedStudentAction</span></span>| <span data-ttu-id="d9db8-137">Действия по умолчанию класса для учащихся, добавленные после даты публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="d9db8-137">Class-level default actions for students added after the assignment publication date.</span></span> <span data-ttu-id="d9db8-138">Возможные значения: `none`, `assignIfOpen`.</span><span class="sxs-lookup"><span data-stu-id="d9db8-138">Possible values are: `none`, `assignIfOpen`.</span></span> <span data-ttu-id="d9db8-139">Значение по умолчанию — `none`.</span><span class="sxs-lookup"><span data-stu-id="d9db8-139">The default value is `none`.</span></span>|
|<span data-ttu-id="d9db8-140">dueTime</span><span class="sxs-lookup"><span data-stu-id="d9db8-140">dueTime</span></span>|<span data-ttu-id="d9db8-141">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d9db8-141">TimeOfDay</span></span>| <span data-ttu-id="d9db8-142">Значение по умолчанию класса для должного поля времени.</span><span class="sxs-lookup"><span data-stu-id="d9db8-142">Class-level default value for due time field.</span></span> <span data-ttu-id="d9db8-143">Значение по умолчанию: `23:59:00`.</span><span class="sxs-lookup"><span data-stu-id="d9db8-143">Default value is `23:59:00`</span></span>|
|<span data-ttu-id="d9db8-144">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="d9db8-144">notificationChannelUrl</span></span>|<span data-ttu-id="d9db8-145">String</span><span class="sxs-lookup"><span data-stu-id="d9db8-145">String</span></span>| <span data-ttu-id="d9db8-146">По умолчанию Teams канал для отправки уведомлений, связанных с назначением.</span><span class="sxs-lookup"><span data-stu-id="d9db8-146">Default Teams channel to send notifications related to the assignment.</span></span> <span data-ttu-id="d9db8-147">Значение по умолчанию — `null`.</span><span class="sxs-lookup"><span data-stu-id="d9db8-147">Default value is `null`.</span></span>|



## <a name="response"></a><span data-ttu-id="d9db8-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9db8-148">Response</span></span>

<span data-ttu-id="d9db8-149">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d9db8-149">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9db8-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="d9db8-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9db8-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9db8-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d9db8-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9db8-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentdefaults"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
Content-Type: application/json
Content-length: 181

{
  "addedStudentAction": "assignIfOpen",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')"
}
```
# <a name="c"></a>[<span data-ttu-id="d9db8-153">C#</span><span class="sxs-lookup"><span data-stu-id="d9db8-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9db8-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9db8-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9db8-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9db8-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9db8-156">Java</span><span class="sxs-lookup"><span data-stu-id="d9db8-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentdefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9db8-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9db8-157">Response</span></span>
<span data-ttu-id="d9db8-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d9db8-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentDefaults"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "addedStudentAction": "assignIfOpen",
  "dueTime": "String",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')"
}
```

