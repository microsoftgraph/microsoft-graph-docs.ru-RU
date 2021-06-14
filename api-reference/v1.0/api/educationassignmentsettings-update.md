---
title: Обновление educationAssignmentSettings
description: Обновление свойств объекта educationAssignmentSettings.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 11802b1b2fadfc717a123db31ad91436183442ed
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912949"
---
# <a name="update-educationassignmentsettings"></a><span data-ttu-id="de000-103">Обновление educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="de000-103">Update educationAssignmentSettings</span></span>
<span data-ttu-id="de000-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de000-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de000-105">Обновление свойств объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="de000-105">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span> <span data-ttu-id="de000-106">Только Учителя могут обновлять эти параметры.</span><span class="sxs-lookup"><span data-stu-id="de000-106">Only Teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="de000-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de000-107">Permissions</span></span>
<span data-ttu-id="de000-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de000-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de000-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de000-110">Permission type</span></span>|<span data-ttu-id="de000-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de000-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de000-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de000-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de000-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de000-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="de000-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de000-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de000-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de000-115">Not supported.</span></span>|
|<span data-ttu-id="de000-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de000-116">Application</span></span>|<span data-ttu-id="de000-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de000-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de000-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de000-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

## <a name="request-headers"></a><span data-ttu-id="de000-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de000-119">Request headers</span></span>
|<span data-ttu-id="de000-120">Имя</span><span class="sxs-lookup"><span data-stu-id="de000-120">Name</span></span>|<span data-ttu-id="de000-121">Описание</span><span class="sxs-lookup"><span data-stu-id="de000-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="de000-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de000-122">Authorization</span></span>|<span data-ttu-id="de000-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de000-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="de000-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de000-125">Content-Type</span></span>|<span data-ttu-id="de000-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de000-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de000-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de000-128">Request body</span></span>
<span data-ttu-id="de000-129">В теле запроса поставляют представление JSON объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="de000-129">In the request body, supply a JSON representation of the [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

<span data-ttu-id="de000-130">В следующей таблице показаны свойства, необходимые при обновлении [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="de000-130">The following table shows the properties that are required when you update the [educationAssignmentSettings](../resources/educationassignmentsettings.md).</span></span>

|<span data-ttu-id="de000-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="de000-131">Property</span></span>|<span data-ttu-id="de000-132">Тип</span><span class="sxs-lookup"><span data-stu-id="de000-132">Type</span></span>|<span data-ttu-id="de000-133">Описание</span><span class="sxs-lookup"><span data-stu-id="de000-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de000-134">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="de000-134">submissionAnimationDisabled</span></span>|<span data-ttu-id="de000-135">Логический</span><span class="sxs-lookup"><span data-stu-id="de000-135">Boolean</span></span>|<span data-ttu-id="de000-136">Указывает, будет ли показана анимация празднования по очереди.</span><span class="sxs-lookup"><span data-stu-id="de000-136">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="de000-137">Значение `true` указывает, что анимация не будет показана.</span><span class="sxs-lookup"><span data-stu-id="de000-137">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="de000-138">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="de000-138">Default value is `false`.</span></span>|



## <a name="response"></a><span data-ttu-id="de000-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="de000-139">Response</span></span>

<span data-ttu-id="de000-140">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="de000-140">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de000-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="de000-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de000-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="de000-142">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="de000-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="de000-143">Response</span></span>
<span data-ttu-id="de000-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="de000-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

