---
title: Update termsAndConditions
description: Обновление свойств объекта termsAndConditions.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cf64229a71a40c0af761038a0ec7c58f8e104f8d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354611"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="48a93-103">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="48a93-103">Update termsAndConditions</span></span>

> <span data-ttu-id="48a93-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48a93-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48a93-105">Обновление свойств объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="48a93-105">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48a93-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="48a93-106">Prerequisites</span></span>
<span data-ttu-id="48a93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48a93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48a93-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48a93-109">Permission type</span></span>|<span data-ttu-id="48a93-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48a93-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48a93-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48a93-111">Delegated (work or school account)</span></span>|<span data-ttu-id="48a93-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48a93-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="48a93-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48a93-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48a93-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48a93-114">Not supported.</span></span>|
|<span data-ttu-id="48a93-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48a93-115">Application</span></span>|<span data-ttu-id="48a93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48a93-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48a93-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48a93-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="48a93-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48a93-118">Request headers</span></span>
|<span data-ttu-id="48a93-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48a93-119">Header</span></span>|<span data-ttu-id="48a93-120">Значение</span><span class="sxs-lookup"><span data-stu-id="48a93-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48a93-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48a93-121">Authorization</span></span>|<span data-ttu-id="48a93-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48a93-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48a93-123">Accept</span><span class="sxs-lookup"><span data-stu-id="48a93-123">Accept</span></span>|<span data-ttu-id="48a93-124">application/json</span><span class="sxs-lookup"><span data-stu-id="48a93-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48a93-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48a93-125">Request body</span></span>
<span data-ttu-id="48a93-126">В тексте запроса добавьте представление объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48a93-126">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="48a93-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="48a93-127">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="48a93-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="48a93-128">Property</span></span>|<span data-ttu-id="48a93-129">Тип</span><span class="sxs-lookup"><span data-stu-id="48a93-129">Type</span></span>|<span data-ttu-id="48a93-130">Описание</span><span class="sxs-lookup"><span data-stu-id="48a93-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48a93-131">id</span><span class="sxs-lookup"><span data-stu-id="48a93-131">id</span></span>|<span data-ttu-id="48a93-132">String</span><span class="sxs-lookup"><span data-stu-id="48a93-132">String</span></span>|<span data-ttu-id="48a93-133">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="48a93-133">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="48a93-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48a93-134">createdDateTime</span></span>|<span data-ttu-id="48a93-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48a93-135">DateTimeOffset</span></span>|<span data-ttu-id="48a93-136">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="48a93-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="48a93-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48a93-137">lastModifiedDateTime</span></span>|<span data-ttu-id="48a93-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48a93-138">DateTimeOffset</span></span>|<span data-ttu-id="48a93-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="48a93-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="48a93-140">displayName</span><span class="sxs-lookup"><span data-stu-id="48a93-140">displayName</span></span>|<span data-ttu-id="48a93-141">Строка</span><span class="sxs-lookup"><span data-stu-id="48a93-141">String</span></span>|<span data-ttu-id="48a93-142">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="48a93-142">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="48a93-143">description</span><span class="sxs-lookup"><span data-stu-id="48a93-143">description</span></span>|<span data-ttu-id="48a93-144">Строка</span><span class="sxs-lookup"><span data-stu-id="48a93-144">String</span></span>|<span data-ttu-id="48a93-145">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="48a93-145">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="48a93-146">title</span><span class="sxs-lookup"><span data-stu-id="48a93-146">title</span></span>|<span data-ttu-id="48a93-147">String</span><span class="sxs-lookup"><span data-stu-id="48a93-147">String</span></span>|<span data-ttu-id="48a93-148">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="48a93-148">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="48a93-149">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="48a93-149">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="48a93-150">bodyText</span><span class="sxs-lookup"><span data-stu-id="48a93-150">bodyText</span></span>|<span data-ttu-id="48a93-151">String</span><span class="sxs-lookup"><span data-stu-id="48a93-151">String</span></span>|<span data-ttu-id="48a93-152">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="48a93-152">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="48a93-153">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="48a93-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="48a93-154">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="48a93-154">acceptanceStatement</span></span>|<span data-ttu-id="48a93-155">String</span><span class="sxs-lookup"><span data-stu-id="48a93-155">String</span></span>|<span data-ttu-id="48a93-156">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="48a93-156">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="48a93-157">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="48a93-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="48a93-158">version</span><span class="sxs-lookup"><span data-stu-id="48a93-158">version</span></span>|<span data-ttu-id="48a93-159">Int32</span><span class="sxs-lookup"><span data-stu-id="48a93-159">Int32</span></span>|<span data-ttu-id="48a93-160">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="48a93-160">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="48a93-161">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="48a93-161">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="48a93-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="48a93-162">Response</span></span>
<span data-ttu-id="48a93-163">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="48a93-163">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48a93-164">Пример</span><span class="sxs-lookup"><span data-stu-id="48a93-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="48a93-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="48a93-165">Request</span></span>
<span data-ttu-id="48a93-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48a93-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48a93-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="48a93-167">Response</span></span>
<span data-ttu-id="48a93-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48a93-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




