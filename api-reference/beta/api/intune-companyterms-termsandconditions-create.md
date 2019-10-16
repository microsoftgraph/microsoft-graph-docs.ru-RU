---
title: Создание объекта termsAndConditions
description: Создание объекта termsAndConditions.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4652d429478af1513e6ff12ed01ccc4babde5dbb
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534927"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="e8048-103">Создание объекта termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="e8048-103">Create termsAndConditions</span></span>

> <span data-ttu-id="e8048-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8048-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8048-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8048-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8048-106">Создание объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="e8048-106">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8048-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e8048-107">Prerequisites</span></span>
<span data-ttu-id="e8048-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8048-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8048-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8048-110">Permission type</span></span>|<span data-ttu-id="e8048-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8048-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8048-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8048-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8048-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8048-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e8048-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8048-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8048-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8048-115">Not supported.</span></span>|
|<span data-ttu-id="e8048-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e8048-116">Application</span></span>|<span data-ttu-id="e8048-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8048-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8048-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8048-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="e8048-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8048-119">Request headers</span></span>
|<span data-ttu-id="e8048-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8048-120">Header</span></span>|<span data-ttu-id="e8048-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e8048-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8048-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8048-122">Authorization</span></span>|<span data-ttu-id="e8048-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8048-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8048-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e8048-124">Accept</span></span>|<span data-ttu-id="e8048-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8048-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8048-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8048-126">Request body</span></span>
<span data-ttu-id="e8048-127">В тексте запроса добавьте представление объекта termsAndConditions в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8048-127">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="e8048-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="e8048-128">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="e8048-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8048-129">Property</span></span>|<span data-ttu-id="e8048-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e8048-130">Type</span></span>|<span data-ttu-id="e8048-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e8048-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8048-132">id</span><span class="sxs-lookup"><span data-stu-id="e8048-132">id</span></span>|<span data-ttu-id="e8048-133">String</span><span class="sxs-lookup"><span data-stu-id="e8048-133">String</span></span>|<span data-ttu-id="e8048-134">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="e8048-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="e8048-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8048-135">createdDateTime</span></span>|<span data-ttu-id="e8048-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8048-136">DateTimeOffset</span></span>|<span data-ttu-id="e8048-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e8048-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="e8048-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8048-138">modifiedDateTime</span></span>|<span data-ttu-id="e8048-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8048-139">DateTimeOffset</span></span>|<span data-ttu-id="e8048-140">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e8048-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e8048-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8048-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e8048-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8048-142">DateTimeOffset</span></span>|<span data-ttu-id="e8048-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e8048-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e8048-144">displayName</span><span class="sxs-lookup"><span data-stu-id="e8048-144">displayName</span></span>|<span data-ttu-id="e8048-145">Строка</span><span class="sxs-lookup"><span data-stu-id="e8048-145">String</span></span>|<span data-ttu-id="e8048-146">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="e8048-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="e8048-147">description</span><span class="sxs-lookup"><span data-stu-id="e8048-147">description</span></span>|<span data-ttu-id="e8048-148">Строка</span><span class="sxs-lookup"><span data-stu-id="e8048-148">String</span></span>|<span data-ttu-id="e8048-149">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="e8048-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="e8048-150">title</span><span class="sxs-lookup"><span data-stu-id="e8048-150">title</span></span>|<span data-ttu-id="e8048-151">String</span><span class="sxs-lookup"><span data-stu-id="e8048-151">String</span></span>|<span data-ttu-id="e8048-152">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="e8048-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="e8048-153">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="e8048-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e8048-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="e8048-154">bodyText</span></span>|<span data-ttu-id="e8048-155">String</span><span class="sxs-lookup"><span data-stu-id="e8048-155">String</span></span>|<span data-ttu-id="e8048-156">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="e8048-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="e8048-157">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="e8048-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e8048-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="e8048-158">acceptanceStatement</span></span>|<span data-ttu-id="e8048-159">String</span><span class="sxs-lookup"><span data-stu-id="e8048-159">String</span></span>|<span data-ttu-id="e8048-160">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="e8048-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="e8048-161">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="e8048-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e8048-162">version</span><span class="sxs-lookup"><span data-stu-id="e8048-162">version</span></span>|<span data-ttu-id="e8048-163">Int32</span><span class="sxs-lookup"><span data-stu-id="e8048-163">Int32</span></span>|<span data-ttu-id="e8048-164">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="e8048-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="e8048-165">Увеличивается, когда администратор вносит изменения в условия и хочет, чтобы пользователи повторно приняли измененную политику.</span><span class="sxs-lookup"><span data-stu-id="e8048-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="e8048-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8048-166">roleScopeTagIds</span></span>|<span data-ttu-id="e8048-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e8048-167">String collection</span></span>|<span data-ttu-id="e8048-168">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e8048-168">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="e8048-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8048-169">Response</span></span>
<span data-ttu-id="e8048-170">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8048-170">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8048-171">Пример</span><span class="sxs-lookup"><span data-stu-id="e8048-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8048-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8048-172">Request</span></span>
<span data-ttu-id="e8048-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8048-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
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

### <a name="response"></a><span data-ttu-id="e8048-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8048-174">Response</span></span>
<span data-ttu-id="e8048-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8048-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






