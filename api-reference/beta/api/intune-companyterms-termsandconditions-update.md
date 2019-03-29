---
title: Update termsAndConditions
description: Обновление свойств объекта termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1855a5b3c4933b7304b9b984ab96aaaaab0b675
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957418"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="40a43-103">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="40a43-103">Update termsAndConditions</span></span>

> <span data-ttu-id="40a43-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40a43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40a43-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40a43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40a43-106">Обновление свойств объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="40a43-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40a43-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="40a43-107">Prerequisites</span></span>
<span data-ttu-id="40a43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40a43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40a43-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40a43-110">Permission type</span></span>|<span data-ttu-id="40a43-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40a43-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40a43-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40a43-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40a43-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40a43-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="40a43-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40a43-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40a43-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40a43-115">Not supported.</span></span>|
|<span data-ttu-id="40a43-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40a43-116">Application</span></span>|<span data-ttu-id="40a43-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40a43-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40a43-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40a43-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="40a43-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40a43-119">Request headers</span></span>
|<span data-ttu-id="40a43-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40a43-120">Header</span></span>|<span data-ttu-id="40a43-121">Значение</span><span class="sxs-lookup"><span data-stu-id="40a43-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40a43-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40a43-122">Authorization</span></span>|<span data-ttu-id="40a43-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40a43-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40a43-124">Accept</span><span class="sxs-lookup"><span data-stu-id="40a43-124">Accept</span></span>|<span data-ttu-id="40a43-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40a43-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40a43-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40a43-126">Request body</span></span>
<span data-ttu-id="40a43-127">В тексте запроса добавьте представление объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40a43-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="40a43-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="40a43-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="40a43-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="40a43-129">Property</span></span>|<span data-ttu-id="40a43-130">Тип</span><span class="sxs-lookup"><span data-stu-id="40a43-130">Type</span></span>|<span data-ttu-id="40a43-131">Описание</span><span class="sxs-lookup"><span data-stu-id="40a43-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40a43-132">id</span><span class="sxs-lookup"><span data-stu-id="40a43-132">id</span></span>|<span data-ttu-id="40a43-133">Строка</span><span class="sxs-lookup"><span data-stu-id="40a43-133">String</span></span>|<span data-ttu-id="40a43-134">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="40a43-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="40a43-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40a43-135">createdDateTime</span></span>|<span data-ttu-id="40a43-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40a43-136">DateTimeOffset</span></span>|<span data-ttu-id="40a43-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="40a43-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="40a43-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40a43-138">modifiedDateTime</span></span>|<span data-ttu-id="40a43-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40a43-139">DateTimeOffset</span></span>|<span data-ttu-id="40a43-140">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="40a43-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="40a43-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40a43-141">lastModifiedDateTime</span></span>|<span data-ttu-id="40a43-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40a43-142">DateTimeOffset</span></span>|<span data-ttu-id="40a43-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="40a43-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="40a43-144">displayName</span><span class="sxs-lookup"><span data-stu-id="40a43-144">displayName</span></span>|<span data-ttu-id="40a43-145">String</span><span class="sxs-lookup"><span data-stu-id="40a43-145">String</span></span>|<span data-ttu-id="40a43-146">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="40a43-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="40a43-147">description</span><span class="sxs-lookup"><span data-stu-id="40a43-147">description</span></span>|<span data-ttu-id="40a43-148">String</span><span class="sxs-lookup"><span data-stu-id="40a43-148">String</span></span>|<span data-ttu-id="40a43-149">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="40a43-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="40a43-150">title</span><span class="sxs-lookup"><span data-stu-id="40a43-150">title</span></span>|<span data-ttu-id="40a43-151">Строка</span><span class="sxs-lookup"><span data-stu-id="40a43-151">String</span></span>|<span data-ttu-id="40a43-152">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="40a43-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="40a43-153">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="40a43-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="40a43-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="40a43-154">bodyText</span></span>|<span data-ttu-id="40a43-155">String</span><span class="sxs-lookup"><span data-stu-id="40a43-155">String</span></span>|<span data-ttu-id="40a43-156">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="40a43-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="40a43-157">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="40a43-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="40a43-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="40a43-158">acceptanceStatement</span></span>|<span data-ttu-id="40a43-159">String</span><span class="sxs-lookup"><span data-stu-id="40a43-159">String</span></span>|<span data-ttu-id="40a43-160">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="40a43-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="40a43-161">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="40a43-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="40a43-162">version</span><span class="sxs-lookup"><span data-stu-id="40a43-162">version</span></span>|<span data-ttu-id="40a43-163">Int32</span><span class="sxs-lookup"><span data-stu-id="40a43-163">Int32</span></span>|<span data-ttu-id="40a43-164">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="40a43-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="40a43-165">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="40a43-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="40a43-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="40a43-166">Response</span></span>
<span data-ttu-id="40a43-167">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="40a43-167">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40a43-168">Пример</span><span class="sxs-lookup"><span data-stu-id="40a43-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="40a43-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="40a43-169">Request</span></span>
<span data-ttu-id="40a43-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40a43-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="40a43-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="40a43-171">Response</span></span>
<span data-ttu-id="40a43-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40a43-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




