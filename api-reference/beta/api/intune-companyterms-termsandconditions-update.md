---
title: Update termsAndConditions
description: Обновление свойств объекта termsAndConditions.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39df5d745604a750dde7567f2ee5059c8e9f5b54
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39929933"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="3e66d-103">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3e66d-103">Update termsAndConditions</span></span>

> <span data-ttu-id="3e66d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e66d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e66d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e66d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e66d-106">Обновление свойств объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="3e66d-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e66d-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3e66d-107">Prerequisites</span></span>
<span data-ttu-id="3e66d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e66d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e66d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e66d-110">Permission type</span></span>|<span data-ttu-id="3e66d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e66d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e66d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e66d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e66d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e66d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3e66d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e66d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e66d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e66d-115">Not supported.</span></span>|
|<span data-ttu-id="3e66d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e66d-116">Application</span></span>|<span data-ttu-id="3e66d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e66d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e66d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e66d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="3e66d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3e66d-119">Request headers</span></span>
|<span data-ttu-id="3e66d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e66d-120">Header</span></span>|<span data-ttu-id="3e66d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3e66d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e66d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e66d-122">Authorization</span></span>|<span data-ttu-id="3e66d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e66d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e66d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3e66d-124">Accept</span></span>|<span data-ttu-id="3e66d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e66d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e66d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e66d-126">Request body</span></span>
<span data-ttu-id="3e66d-127">В тексте запроса добавьте представление объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e66d-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="3e66d-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="3e66d-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="3e66d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e66d-129">Property</span></span>|<span data-ttu-id="3e66d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3e66d-130">Type</span></span>|<span data-ttu-id="3e66d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3e66d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e66d-132">id</span><span class="sxs-lookup"><span data-stu-id="3e66d-132">id</span></span>|<span data-ttu-id="3e66d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="3e66d-133">String</span></span>|<span data-ttu-id="3e66d-134">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="3e66d-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="3e66d-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e66d-135">createdDateTime</span></span>|<span data-ttu-id="3e66d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e66d-136">DateTimeOffset</span></span>|<span data-ttu-id="3e66d-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3e66d-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="3e66d-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e66d-138">modifiedDateTime</span></span>|<span data-ttu-id="3e66d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e66d-139">DateTimeOffset</span></span>|<span data-ttu-id="3e66d-140">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3e66d-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3e66d-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e66d-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3e66d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e66d-142">DateTimeOffset</span></span>|<span data-ttu-id="3e66d-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3e66d-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3e66d-144">displayName</span><span class="sxs-lookup"><span data-stu-id="3e66d-144">displayName</span></span>|<span data-ttu-id="3e66d-145">Строка</span><span class="sxs-lookup"><span data-stu-id="3e66d-145">String</span></span>|<span data-ttu-id="3e66d-146">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="3e66d-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="3e66d-147">description</span><span class="sxs-lookup"><span data-stu-id="3e66d-147">description</span></span>|<span data-ttu-id="3e66d-148">Строка</span><span class="sxs-lookup"><span data-stu-id="3e66d-148">String</span></span>|<span data-ttu-id="3e66d-149">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="3e66d-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="3e66d-150">title</span><span class="sxs-lookup"><span data-stu-id="3e66d-150">title</span></span>|<span data-ttu-id="3e66d-151">String</span><span class="sxs-lookup"><span data-stu-id="3e66d-151">String</span></span>|<span data-ttu-id="3e66d-152">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="3e66d-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="3e66d-153">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="3e66d-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3e66d-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="3e66d-154">bodyText</span></span>|<span data-ttu-id="3e66d-155">Строка</span><span class="sxs-lookup"><span data-stu-id="3e66d-155">String</span></span>|<span data-ttu-id="3e66d-156">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="3e66d-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="3e66d-157">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="3e66d-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3e66d-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="3e66d-158">acceptanceStatement</span></span>|<span data-ttu-id="3e66d-159">String</span><span class="sxs-lookup"><span data-stu-id="3e66d-159">String</span></span>|<span data-ttu-id="3e66d-160">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="3e66d-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="3e66d-161">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="3e66d-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3e66d-162">version</span><span class="sxs-lookup"><span data-stu-id="3e66d-162">version</span></span>|<span data-ttu-id="3e66d-163">Int32</span><span class="sxs-lookup"><span data-stu-id="3e66d-163">Int32</span></span>|<span data-ttu-id="3e66d-164">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="3e66d-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="3e66d-165">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="3e66d-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="3e66d-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3e66d-166">roleScopeTagIds</span></span>|<span data-ttu-id="3e66d-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3e66d-167">String collection</span></span>|<span data-ttu-id="3e66d-168">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3e66d-168">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="3e66d-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e66d-169">Response</span></span>
<span data-ttu-id="3e66d-170">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3e66d-170">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e66d-171">Пример</span><span class="sxs-lookup"><span data-stu-id="3e66d-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e66d-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e66d-172">Request</span></span>
<span data-ttu-id="3e66d-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e66d-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3e66d-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e66d-174">Response</span></span>
<span data-ttu-id="3e66d-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e66d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





