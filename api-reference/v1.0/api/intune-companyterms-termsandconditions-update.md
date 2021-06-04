---
title: Update termsAndConditions
description: Обновление свойств объекта termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 49c9d7f1c80c039822ac798cc1de4d721288a0b4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754016"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="be682-103">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="be682-103">Update termsAndConditions</span></span>

<span data-ttu-id="be682-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be682-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be682-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be682-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be682-106">Обновление свойств объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="be682-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be682-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="be682-107">Prerequisites</span></span>
<span data-ttu-id="be682-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be682-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be682-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be682-110">Permission type</span></span>|<span data-ttu-id="be682-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be682-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be682-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be682-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be682-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be682-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="be682-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be682-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be682-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be682-115">Not supported.</span></span>|
|<span data-ttu-id="be682-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="be682-116">Application</span></span>|<span data-ttu-id="be682-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be682-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be682-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be682-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="be682-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="be682-119">Request headers</span></span>
|<span data-ttu-id="be682-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be682-120">Header</span></span>|<span data-ttu-id="be682-121">Значение</span><span class="sxs-lookup"><span data-stu-id="be682-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be682-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be682-122">Authorization</span></span>|<span data-ttu-id="be682-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be682-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be682-124">Accept</span><span class="sxs-lookup"><span data-stu-id="be682-124">Accept</span></span>|<span data-ttu-id="be682-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be682-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be682-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be682-126">Request body</span></span>
<span data-ttu-id="be682-127">В тексте запроса добавьте представление объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be682-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="be682-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="be682-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="be682-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="be682-129">Property</span></span>|<span data-ttu-id="be682-130">Тип</span><span class="sxs-lookup"><span data-stu-id="be682-130">Type</span></span>|<span data-ttu-id="be682-131">Описание</span><span class="sxs-lookup"><span data-stu-id="be682-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be682-132">id</span><span class="sxs-lookup"><span data-stu-id="be682-132">id</span></span>|<span data-ttu-id="be682-133">String</span><span class="sxs-lookup"><span data-stu-id="be682-133">String</span></span>|<span data-ttu-id="be682-134">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="be682-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="be682-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be682-135">createdDateTime</span></span>|<span data-ttu-id="be682-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be682-136">DateTimeOffset</span></span>|<span data-ttu-id="be682-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="be682-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="be682-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be682-138">lastModifiedDateTime</span></span>|<span data-ttu-id="be682-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be682-139">DateTimeOffset</span></span>|<span data-ttu-id="be682-140">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="be682-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="be682-141">displayName</span><span class="sxs-lookup"><span data-stu-id="be682-141">displayName</span></span>|<span data-ttu-id="be682-142">String</span><span class="sxs-lookup"><span data-stu-id="be682-142">String</span></span>|<span data-ttu-id="be682-143">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="be682-143">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="be682-144">description</span><span class="sxs-lookup"><span data-stu-id="be682-144">description</span></span>|<span data-ttu-id="be682-145">String</span><span class="sxs-lookup"><span data-stu-id="be682-145">String</span></span>|<span data-ttu-id="be682-146">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="be682-146">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="be682-147">title</span><span class="sxs-lookup"><span data-stu-id="be682-147">title</span></span>|<span data-ttu-id="be682-148">String</span><span class="sxs-lookup"><span data-stu-id="be682-148">String</span></span>|<span data-ttu-id="be682-149">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="be682-149">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="be682-150">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="be682-150">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="be682-151">bodyText</span><span class="sxs-lookup"><span data-stu-id="be682-151">bodyText</span></span>|<span data-ttu-id="be682-152">String</span><span class="sxs-lookup"><span data-stu-id="be682-152">String</span></span>|<span data-ttu-id="be682-153">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="be682-153">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="be682-154">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="be682-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="be682-155">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="be682-155">acceptanceStatement</span></span>|<span data-ttu-id="be682-156">String</span><span class="sxs-lookup"><span data-stu-id="be682-156">String</span></span>|<span data-ttu-id="be682-157">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="be682-157">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="be682-158">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="be682-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="be682-159">version</span><span class="sxs-lookup"><span data-stu-id="be682-159">version</span></span>|<span data-ttu-id="be682-160">Int32</span><span class="sxs-lookup"><span data-stu-id="be682-160">Int32</span></span>|<span data-ttu-id="be682-161">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="be682-161">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="be682-162">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="be682-162">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="be682-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="be682-163">Response</span></span>
<span data-ttu-id="be682-164">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="be682-164">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be682-165">Пример</span><span class="sxs-lookup"><span data-stu-id="be682-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="be682-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="be682-166">Request</span></span>
<span data-ttu-id="be682-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be682-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
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

### <a name="response"></a><span data-ttu-id="be682-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="be682-168">Response</span></span>
<span data-ttu-id="be682-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be682-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```




