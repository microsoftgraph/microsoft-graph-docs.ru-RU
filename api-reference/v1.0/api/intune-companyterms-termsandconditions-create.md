---
title: Создание объекта termsAndConditions
description: Создание объекта termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a4861aab5113eab6658458fbec58846a1bf8c508
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760716"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="ff15f-103">Создание объекта termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ff15f-103">Create termsAndConditions</span></span>

<span data-ttu-id="ff15f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff15f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff15f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff15f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff15f-106">Создание объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="ff15f-106">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff15f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff15f-107">Prerequisites</span></span>
<span data-ttu-id="ff15f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff15f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff15f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff15f-110">Permission type</span></span>|<span data-ttu-id="ff15f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff15f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff15f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff15f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff15f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff15f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ff15f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff15f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff15f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff15f-115">Not supported.</span></span>|
|<span data-ttu-id="ff15f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ff15f-116">Application</span></span>|<span data-ttu-id="ff15f-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff15f-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff15f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff15f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="ff15f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ff15f-119">Request headers</span></span>
|<span data-ttu-id="ff15f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff15f-120">Header</span></span>|<span data-ttu-id="ff15f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ff15f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff15f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff15f-122">Authorization</span></span>|<span data-ttu-id="ff15f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff15f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff15f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ff15f-124">Accept</span></span>|<span data-ttu-id="ff15f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff15f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff15f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff15f-126">Request body</span></span>
<span data-ttu-id="ff15f-127">В тексте запроса добавьте представление объекта termsAndConditions в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff15f-127">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="ff15f-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="ff15f-128">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="ff15f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff15f-129">Property</span></span>|<span data-ttu-id="ff15f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ff15f-130">Type</span></span>|<span data-ttu-id="ff15f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ff15f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff15f-132">id</span><span class="sxs-lookup"><span data-stu-id="ff15f-132">id</span></span>|<span data-ttu-id="ff15f-133">String</span><span class="sxs-lookup"><span data-stu-id="ff15f-133">String</span></span>|<span data-ttu-id="ff15f-134">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="ff15f-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="ff15f-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff15f-135">createdDateTime</span></span>|<span data-ttu-id="ff15f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff15f-136">DateTimeOffset</span></span>|<span data-ttu-id="ff15f-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ff15f-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="ff15f-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff15f-138">lastModifiedDateTime</span></span>|<span data-ttu-id="ff15f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff15f-139">DateTimeOffset</span></span>|<span data-ttu-id="ff15f-140">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ff15f-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ff15f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="ff15f-141">displayName</span></span>|<span data-ttu-id="ff15f-142">String</span><span class="sxs-lookup"><span data-stu-id="ff15f-142">String</span></span>|<span data-ttu-id="ff15f-143">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="ff15f-143">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="ff15f-144">description</span><span class="sxs-lookup"><span data-stu-id="ff15f-144">description</span></span>|<span data-ttu-id="ff15f-145">String</span><span class="sxs-lookup"><span data-stu-id="ff15f-145">String</span></span>|<span data-ttu-id="ff15f-146">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="ff15f-146">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="ff15f-147">title</span><span class="sxs-lookup"><span data-stu-id="ff15f-147">title</span></span>|<span data-ttu-id="ff15f-148">String</span><span class="sxs-lookup"><span data-stu-id="ff15f-148">String</span></span>|<span data-ttu-id="ff15f-149">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="ff15f-149">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="ff15f-150">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="ff15f-150">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="ff15f-151">bodyText</span><span class="sxs-lookup"><span data-stu-id="ff15f-151">bodyText</span></span>|<span data-ttu-id="ff15f-152">String</span><span class="sxs-lookup"><span data-stu-id="ff15f-152">String</span></span>|<span data-ttu-id="ff15f-153">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="ff15f-153">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="ff15f-154">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="ff15f-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="ff15f-155">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="ff15f-155">acceptanceStatement</span></span>|<span data-ttu-id="ff15f-156">String</span><span class="sxs-lookup"><span data-stu-id="ff15f-156">String</span></span>|<span data-ttu-id="ff15f-157">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="ff15f-157">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="ff15f-158">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="ff15f-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="ff15f-159">version</span><span class="sxs-lookup"><span data-stu-id="ff15f-159">version</span></span>|<span data-ttu-id="ff15f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="ff15f-160">Int32</span></span>|<span data-ttu-id="ff15f-161">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="ff15f-161">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="ff15f-162">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="ff15f-162">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="ff15f-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff15f-163">Response</span></span>
<span data-ttu-id="ff15f-164">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff15f-164">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff15f-165">Пример</span><span class="sxs-lookup"><span data-stu-id="ff15f-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff15f-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff15f-166">Request</span></span>
<span data-ttu-id="ff15f-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff15f-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
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

### <a name="response"></a><span data-ttu-id="ff15f-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff15f-168">Response</span></span>
<span data-ttu-id="ff15f-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff15f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




