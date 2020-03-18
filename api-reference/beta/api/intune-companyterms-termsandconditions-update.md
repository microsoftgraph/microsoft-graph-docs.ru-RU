---
title: Update termsAndConditions
description: Обновление свойств объекта termsAndConditions.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a866b17861c3c11047607f4af6691fc810648142
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760153"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="6fc48-103">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6fc48-103">Update termsAndConditions</span></span>

> <span data-ttu-id="6fc48-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fc48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fc48-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fc48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fc48-106">Обновление свойств объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="6fc48-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fc48-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6fc48-107">Prerequisites</span></span>
<span data-ttu-id="6fc48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fc48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fc48-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fc48-110">Permission type</span></span>|<span data-ttu-id="6fc48-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fc48-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fc48-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fc48-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6fc48-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fc48-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6fc48-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fc48-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fc48-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fc48-115">Not supported.</span></span>|
|<span data-ttu-id="6fc48-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6fc48-116">Application</span></span>|<span data-ttu-id="6fc48-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fc48-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fc48-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fc48-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="6fc48-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6fc48-119">Request headers</span></span>
|<span data-ttu-id="6fc48-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6fc48-120">Header</span></span>|<span data-ttu-id="6fc48-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6fc48-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fc48-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fc48-122">Authorization</span></span>|<span data-ttu-id="6fc48-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fc48-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fc48-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6fc48-124">Accept</span></span>|<span data-ttu-id="6fc48-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6fc48-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fc48-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6fc48-126">Request body</span></span>
<span data-ttu-id="6fc48-127">В тексте запроса добавьте представление объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fc48-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="6fc48-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="6fc48-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="6fc48-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fc48-129">Property</span></span>|<span data-ttu-id="6fc48-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6fc48-130">Type</span></span>|<span data-ttu-id="6fc48-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6fc48-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc48-132">id</span><span class="sxs-lookup"><span data-stu-id="6fc48-132">id</span></span>|<span data-ttu-id="6fc48-133">String</span><span class="sxs-lookup"><span data-stu-id="6fc48-133">String</span></span>|<span data-ttu-id="6fc48-134">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="6fc48-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="6fc48-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fc48-135">createdDateTime</span></span>|<span data-ttu-id="6fc48-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc48-136">DateTimeOffset</span></span>|<span data-ttu-id="6fc48-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6fc48-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="6fc48-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fc48-138">modifiedDateTime</span></span>|<span data-ttu-id="6fc48-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc48-139">DateTimeOffset</span></span>|<span data-ttu-id="6fc48-140">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6fc48-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6fc48-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fc48-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6fc48-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc48-142">DateTimeOffset</span></span>|<span data-ttu-id="6fc48-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6fc48-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6fc48-144">displayName</span><span class="sxs-lookup"><span data-stu-id="6fc48-144">displayName</span></span>|<span data-ttu-id="6fc48-145">Строка</span><span class="sxs-lookup"><span data-stu-id="6fc48-145">String</span></span>|<span data-ttu-id="6fc48-146">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="6fc48-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="6fc48-147">description</span><span class="sxs-lookup"><span data-stu-id="6fc48-147">description</span></span>|<span data-ttu-id="6fc48-148">Строка</span><span class="sxs-lookup"><span data-stu-id="6fc48-148">String</span></span>|<span data-ttu-id="6fc48-149">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="6fc48-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="6fc48-150">title</span><span class="sxs-lookup"><span data-stu-id="6fc48-150">title</span></span>|<span data-ttu-id="6fc48-151">String</span><span class="sxs-lookup"><span data-stu-id="6fc48-151">String</span></span>|<span data-ttu-id="6fc48-152">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="6fc48-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="6fc48-153">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="6fc48-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6fc48-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="6fc48-154">bodyText</span></span>|<span data-ttu-id="6fc48-155">String</span><span class="sxs-lookup"><span data-stu-id="6fc48-155">String</span></span>|<span data-ttu-id="6fc48-156">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="6fc48-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="6fc48-157">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="6fc48-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6fc48-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="6fc48-158">acceptanceStatement</span></span>|<span data-ttu-id="6fc48-159">String</span><span class="sxs-lookup"><span data-stu-id="6fc48-159">String</span></span>|<span data-ttu-id="6fc48-160">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="6fc48-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="6fc48-161">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="6fc48-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6fc48-162">version</span><span class="sxs-lookup"><span data-stu-id="6fc48-162">version</span></span>|<span data-ttu-id="6fc48-163">Int32</span><span class="sxs-lookup"><span data-stu-id="6fc48-163">Int32</span></span>|<span data-ttu-id="6fc48-164">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="6fc48-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="6fc48-165">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="6fc48-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="6fc48-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6fc48-166">roleScopeTagIds</span></span>|<span data-ttu-id="6fc48-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6fc48-167">String collection</span></span>|<span data-ttu-id="6fc48-168">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6fc48-168">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="6fc48-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="6fc48-169">Response</span></span>
<span data-ttu-id="6fc48-170">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6fc48-170">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fc48-171">Пример</span><span class="sxs-lookup"><span data-stu-id="6fc48-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fc48-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fc48-172">Request</span></span>
<span data-ttu-id="6fc48-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6fc48-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6fc48-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fc48-174">Response</span></span>
<span data-ttu-id="6fc48-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6fc48-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




