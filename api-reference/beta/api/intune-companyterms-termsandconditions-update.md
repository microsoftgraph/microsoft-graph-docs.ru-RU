---
title: Update termsAndConditions
description: Обновление свойств объекта termsAndConditions.
ms.openlocfilehash: 448edf2ceb596d7b4905eb78c8e6d6a37403d3da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076578"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="9bfd4-103">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="9bfd4-103">Update termsAndConditions</span></span>

> <span data-ttu-id="9bfd4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bfd4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9bfd4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bfd4-107">Обновление свойств объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="9bfd4-107">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9bfd4-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9bfd4-108">Prerequisites</span></span>
<span data-ttu-id="9bfd4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bfd4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bfd4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bfd4-111">Permission type</span></span>|<span data-ttu-id="9bfd4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bfd4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bfd4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bfd4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bfd4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bfd4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9bfd4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bfd4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bfd4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-116">Not supported.</span></span>|
|<span data-ttu-id="9bfd4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9bfd4-117">Application</span></span>|<span data-ttu-id="9bfd4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bfd4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bfd4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="9bfd4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bfd4-120">Request headers</span></span>
|<span data-ttu-id="9bfd4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9bfd4-121">Header</span></span>|<span data-ttu-id="9bfd4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9bfd4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bfd4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bfd4-123">Authorization</span></span>|<span data-ttu-id="9bfd4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9bfd4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bfd4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9bfd4-125">Accept</span></span>|<span data-ttu-id="9bfd4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bfd4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bfd4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bfd4-127">Request body</span></span>
<span data-ttu-id="9bfd4-128">В тексте запроса добавьте представление объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-128">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="9bfd4-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="9bfd4-129">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="9bfd4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bfd4-130">Property</span></span>|<span data-ttu-id="9bfd4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9bfd4-131">Type</span></span>|<span data-ttu-id="9bfd4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9bfd4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bfd4-133">id</span><span class="sxs-lookup"><span data-stu-id="9bfd4-133">id</span></span>|<span data-ttu-id="9bfd4-134">String</span><span class="sxs-lookup"><span data-stu-id="9bfd4-134">String</span></span>|<span data-ttu-id="9bfd4-135">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="9bfd4-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9bfd4-136">createdDateTime</span></span>|<span data-ttu-id="9bfd4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bfd4-137">DateTimeOffset</span></span>|<span data-ttu-id="9bfd4-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="9bfd4-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bfd4-139">modifiedDateTime</span></span>|<span data-ttu-id="9bfd4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bfd4-140">DateTimeOffset</span></span>|<span data-ttu-id="9bfd4-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9bfd4-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bfd4-142">lastModifiedDateTime</span></span>|<span data-ttu-id="9bfd4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bfd4-143">DateTimeOffset</span></span>|<span data-ttu-id="9bfd4-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9bfd4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="9bfd4-145">displayName</span></span>|<span data-ttu-id="9bfd4-146">String</span><span class="sxs-lookup"><span data-stu-id="9bfd4-146">String</span></span>|<span data-ttu-id="9bfd4-147">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="9bfd4-148">описание</span><span class="sxs-lookup"><span data-stu-id="9bfd4-148">description</span></span>|<span data-ttu-id="9bfd4-149">String</span><span class="sxs-lookup"><span data-stu-id="9bfd4-149">String</span></span>|<span data-ttu-id="9bfd4-150">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="9bfd4-151">title</span><span class="sxs-lookup"><span data-stu-id="9bfd4-151">title</span></span>|<span data-ttu-id="9bfd4-152">String</span><span class="sxs-lookup"><span data-stu-id="9bfd4-152">String</span></span>|<span data-ttu-id="9bfd4-153">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="9bfd4-154">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9bfd4-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="9bfd4-155">bodyText</span></span>|<span data-ttu-id="9bfd4-156">String</span><span class="sxs-lookup"><span data-stu-id="9bfd4-156">String</span></span>|<span data-ttu-id="9bfd4-157">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="9bfd4-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="9bfd4-158">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9bfd4-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="9bfd4-159">acceptanceStatement</span></span>|<span data-ttu-id="9bfd4-160">String</span><span class="sxs-lookup"><span data-stu-id="9bfd4-160">String</span></span>|<span data-ttu-id="9bfd4-161">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="9bfd4-162">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9bfd4-163">version</span><span class="sxs-lookup"><span data-stu-id="9bfd4-163">version</span></span>|<span data-ttu-id="9bfd4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9bfd4-164">Int32</span></span>|<span data-ttu-id="9bfd4-165">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="9bfd4-166">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="9bfd4-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="9bfd4-167">Response</span></span>
<span data-ttu-id="9bfd4-168">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-168">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bfd4-169">Пример</span><span class="sxs-lookup"><span data-stu-id="9bfd4-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="9bfd4-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bfd4-170">Request</span></span>
<span data-ttu-id="9bfd4-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 280

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="9bfd4-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="9bfd4-172">Response</span></span>
<span data-ttu-id="9bfd4-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9bfd4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 505

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```





