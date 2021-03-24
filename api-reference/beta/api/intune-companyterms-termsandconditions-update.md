---
title: Update termsAndConditions
description: Обновление свойств объекта termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1d3b1120c60e20dbc0cc12cb27a903bcfd7c6b0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133628"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="4a281-103">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4a281-103">Update termsAndConditions</span></span>

<span data-ttu-id="4a281-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a281-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a281-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a281-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a281-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a281-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a281-107">Обновление свойств объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="4a281-107">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a281-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4a281-108">Prerequisites</span></span>
<span data-ttu-id="4a281-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a281-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a281-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a281-111">Permission type</span></span>|<span data-ttu-id="4a281-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a281-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a281-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a281-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a281-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a281-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4a281-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a281-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a281-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a281-116">Not supported.</span></span>|
|<span data-ttu-id="4a281-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4a281-117">Application</span></span>|<span data-ttu-id="4a281-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a281-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a281-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a281-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="4a281-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4a281-120">Request headers</span></span>
|<span data-ttu-id="4a281-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a281-121">Header</span></span>|<span data-ttu-id="4a281-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4a281-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a281-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a281-123">Authorization</span></span>|<span data-ttu-id="4a281-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a281-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a281-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4a281-125">Accept</span></span>|<span data-ttu-id="4a281-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a281-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a281-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a281-127">Request body</span></span>
<span data-ttu-id="4a281-128">В тексте запроса добавьте представление объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a281-128">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="4a281-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="4a281-129">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="4a281-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a281-130">Property</span></span>|<span data-ttu-id="4a281-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4a281-131">Type</span></span>|<span data-ttu-id="4a281-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4a281-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a281-133">id</span><span class="sxs-lookup"><span data-stu-id="4a281-133">id</span></span>|<span data-ttu-id="4a281-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4a281-134">String</span></span>|<span data-ttu-id="4a281-135">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="4a281-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="4a281-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a281-136">createdDateTime</span></span>|<span data-ttu-id="4a281-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a281-137">DateTimeOffset</span></span>|<span data-ttu-id="4a281-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4a281-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="4a281-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a281-139">modifiedDateTime</span></span>|<span data-ttu-id="4a281-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a281-140">DateTimeOffset</span></span>|<span data-ttu-id="4a281-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4a281-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4a281-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a281-142">lastModifiedDateTime</span></span>|<span data-ttu-id="4a281-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a281-143">DateTimeOffset</span></span>|<span data-ttu-id="4a281-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4a281-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4a281-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4a281-145">displayName</span></span>|<span data-ttu-id="4a281-146">Строка</span><span class="sxs-lookup"><span data-stu-id="4a281-146">String</span></span>|<span data-ttu-id="4a281-147">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="4a281-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="4a281-148">description</span><span class="sxs-lookup"><span data-stu-id="4a281-148">description</span></span>|<span data-ttu-id="4a281-149">Строка</span><span class="sxs-lookup"><span data-stu-id="4a281-149">String</span></span>|<span data-ttu-id="4a281-150">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="4a281-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="4a281-151">title</span><span class="sxs-lookup"><span data-stu-id="4a281-151">title</span></span>|<span data-ttu-id="4a281-152">Строка</span><span class="sxs-lookup"><span data-stu-id="4a281-152">String</span></span>|<span data-ttu-id="4a281-153">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="4a281-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="4a281-154">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="4a281-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="4a281-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="4a281-155">bodyText</span></span>|<span data-ttu-id="4a281-156">String</span><span class="sxs-lookup"><span data-stu-id="4a281-156">String</span></span>|<span data-ttu-id="4a281-157">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="4a281-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="4a281-158">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="4a281-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="4a281-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="4a281-159">acceptanceStatement</span></span>|<span data-ttu-id="4a281-160">String</span><span class="sxs-lookup"><span data-stu-id="4a281-160">String</span></span>|<span data-ttu-id="4a281-161">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="4a281-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="4a281-162">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="4a281-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="4a281-163">version</span><span class="sxs-lookup"><span data-stu-id="4a281-163">version</span></span>|<span data-ttu-id="4a281-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4a281-164">Int32</span></span>|<span data-ttu-id="4a281-165">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="4a281-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="4a281-166">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="4a281-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="4a281-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4a281-167">roleScopeTagIds</span></span>|<span data-ttu-id="4a281-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4a281-168">String collection</span></span>|<span data-ttu-id="4a281-169">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="4a281-169">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="4a281-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a281-170">Response</span></span>
<span data-ttu-id="4a281-171">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4a281-171">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a281-172">Пример</span><span class="sxs-lookup"><span data-stu-id="4a281-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a281-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a281-173">Request</span></span>
<span data-ttu-id="4a281-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a281-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="4a281-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a281-175">Response</span></span>
<span data-ttu-id="4a281-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a281-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

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
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




