---
title: Обновление educationAssignmentDefaults
description: Обновление свойств объекта educationAssignmentDefaults.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4dd6d6d8d2c5433ca2ad133c57cae8b17af79ad5
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780822"
---
# <a name="update-educationassignmentdefaults"></a><span data-ttu-id="23a1d-103">Обновление educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="23a1d-103">Update educationAssignmentDefaults</span></span>
<span data-ttu-id="23a1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23a1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23a1d-105">Обновление свойств объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="23a1d-105">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span> <span data-ttu-id="23a1d-106">Только преподаватели могут обновлять эти параметры.</span><span class="sxs-lookup"><span data-stu-id="23a1d-106">Only teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="23a1d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23a1d-107">Permissions</span></span>
<span data-ttu-id="23a1d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23a1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23a1d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23a1d-110">Permission type</span></span>|<span data-ttu-id="23a1d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23a1d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23a1d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23a1d-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="23a1d-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23a1d-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="23a1d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23a1d-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="23a1d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23a1d-115">Not supported.</span></span>  |
|<span data-ttu-id="23a1d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23a1d-116">Application</span></span> | <span data-ttu-id="23a1d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23a1d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23a1d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23a1d-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/{id}/assignmentDefaults
```

## <a name="request-headers"></a><span data-ttu-id="23a1d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23a1d-119">Request headers</span></span>
|<span data-ttu-id="23a1d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="23a1d-120">Name</span></span>|<span data-ttu-id="23a1d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="23a1d-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="23a1d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23a1d-122">Authorization</span></span>|<span data-ttu-id="23a1d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23a1d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="23a1d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23a1d-125">Content-Type</span></span>|<span data-ttu-id="23a1d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23a1d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23a1d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23a1d-128">Request body</span></span>
<span data-ttu-id="23a1d-129">В теле запроса укажи значения для соответствующих полей объекта [educationAssignmentDefaults,](../resources/educationassignmentdefaults.md) который должен быть обновлен.</span><span class="sxs-lookup"><span data-stu-id="23a1d-129">In the request body, supply the values for relevant fields of the [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object that should be updated.</span></span> <span data-ttu-id="23a1d-130">Существующие свойства, не включенные в тело запроса, будут поддерживать прежние значения.</span><span class="sxs-lookup"><span data-stu-id="23a1d-130">Existing properties that are not included in the request body will maintain their previous values.</span></span> <span data-ttu-id="23a1d-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="23a1d-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="23a1d-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="23a1d-132">Property</span></span>|<span data-ttu-id="23a1d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="23a1d-133">Type</span></span>|<span data-ttu-id="23a1d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="23a1d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23a1d-135">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="23a1d-135">addedStudentAction</span></span>|<span data-ttu-id="23a1d-136">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="23a1d-136">educationAddedStudentAction</span></span>|<span data-ttu-id="23a1d-137">Поведение по умолчанию на уровне класса для обработки учащихся, добавленных после публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="23a1d-137">Class-level default behavior for handling students who are added after the assignment is published.</span></span> <span data-ttu-id="23a1d-138">Возможные значения: `none`, `assignIfOpen`.</span><span class="sxs-lookup"><span data-stu-id="23a1d-138">Possible values are: `none`, `assignIfOpen`.</span></span> <span data-ttu-id="23a1d-139">Значение по умолчанию — `none`.</span><span class="sxs-lookup"><span data-stu-id="23a1d-139">The default value is `none`.</span></span>|
|<span data-ttu-id="23a1d-140">dueTime</span><span class="sxs-lookup"><span data-stu-id="23a1d-140">dueTime</span></span>|<span data-ttu-id="23a1d-141">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="23a1d-141">TimeOfDay</span></span>|<span data-ttu-id="23a1d-142">Значение по умолчанию класса для должного поля времени.</span><span class="sxs-lookup"><span data-stu-id="23a1d-142">Class-level default value for due time field.</span></span> <span data-ttu-id="23a1d-143">Значение по умолчанию: `23:59:00`.</span><span class="sxs-lookup"><span data-stu-id="23a1d-143">Default value is `23:59:00`</span></span>|
|<span data-ttu-id="23a1d-144">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="23a1d-144">notificationChannelUrl</span></span>|<span data-ttu-id="23a1d-145">String</span><span class="sxs-lookup"><span data-stu-id="23a1d-145">String</span></span>|<span data-ttu-id="23a1d-146">По умолчанию Teams канал, в который будут отправлены уведомления.</span><span class="sxs-lookup"><span data-stu-id="23a1d-146">Default Teams channel to which notifications will be sent.</span></span> <span data-ttu-id="23a1d-147">Значение по умолчанию — `null`.</span><span class="sxs-lookup"><span data-stu-id="23a1d-147">Default value is `null`.</span></span>|



## <a name="response"></a><span data-ttu-id="23a1d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="23a1d-148">Response</span></span>

<span data-ttu-id="23a1d-149">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="23a1d-149">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23a1d-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="23a1d-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23a1d-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="23a1d-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="23a1d-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="23a1d-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentdefaults"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{id}/assignmentDefaults
Content-Type: application/json
Content-length: 181

{
  "addedStudentAction": "assignIfOpen",
  "addToCalendarAction": "studentsAndTeamOwners",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```
# <a name="c"></a>[<span data-ttu-id="23a1d-153">C#</span><span class="sxs-lookup"><span data-stu-id="23a1d-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23a1d-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23a1d-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23a1d-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23a1d-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23a1d-156">Java</span><span class="sxs-lookup"><span data-stu-id="23a1d-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentdefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="23a1d-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="23a1d-157">Response</span></span>
<span data-ttu-id="23a1d-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="23a1d-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "addToCalendarAction": "studentsAndTeamOwners",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```

