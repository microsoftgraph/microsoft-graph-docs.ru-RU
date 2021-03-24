---
title: Создание groupPolicyUploadedDefinitionFile
description: Создайте новый объект GroupPolicyUploadedDefinitionFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b414eeb1211af6ff9f6683d021f74c3be0d48d79
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145728"
---
# <a name="create-grouppolicyuploadeddefinitionfile"></a><span data-ttu-id="256e3-103">Создание groupPolicyUploadedDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="256e3-103">Create groupPolicyUploadedDefinitionFile</span></span>

<span data-ttu-id="256e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="256e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="256e3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="256e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="256e3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="256e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="256e3-107">Создайте новый [объект GroupPolicyUploadedDefinitionFile.](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="256e3-107">Create a new [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="256e3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="256e3-108">Prerequisites</span></span>
<span data-ttu-id="256e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="256e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="256e3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="256e3-111">Permission type</span></span>|<span data-ttu-id="256e3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="256e3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="256e3-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="256e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="256e3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="256e3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="256e3-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="256e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="256e3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="256e3-116">Not supported.</span></span>|
|<span data-ttu-id="256e3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="256e3-117">Application</span></span>|<span data-ttu-id="256e3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="256e3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="256e3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="256e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## <a name="request-headers"></a><span data-ttu-id="256e3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="256e3-120">Request headers</span></span>
|<span data-ttu-id="256e3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="256e3-121">Header</span></span>|<span data-ttu-id="256e3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="256e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="256e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="256e3-123">Authorization</span></span>|<span data-ttu-id="256e3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="256e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="256e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="256e3-125">Accept</span></span>|<span data-ttu-id="256e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="256e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="256e3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="256e3-127">Request body</span></span>
<span data-ttu-id="256e3-128">В теле запроса поставляем представление JSON для объекта groupPolicyUploadedDefinitionFile.</span><span class="sxs-lookup"><span data-stu-id="256e3-128">In the request body, supply a JSON representation for the groupPolicyUploadedDefinitionFile object.</span></span>

<span data-ttu-id="256e3-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyUploadedDefinitionFile.</span><span class="sxs-lookup"><span data-stu-id="256e3-129">The following table shows the properties that are required when you create the groupPolicyUploadedDefinitionFile.</span></span>

|<span data-ttu-id="256e3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="256e3-130">Property</span></span>|<span data-ttu-id="256e3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="256e3-131">Type</span></span>|<span data-ttu-id="256e3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="256e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="256e3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="256e3-133">displayName</span></span>|<span data-ttu-id="256e3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="256e3-134">String</span></span>|<span data-ttu-id="256e3-135">Локализованное удобное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="256e3-135">The localized friendly name of the ADMX file.</span></span> <span data-ttu-id="256e3-136">Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="256e3-136">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="256e3-137">description</span><span class="sxs-lookup"><span data-stu-id="256e3-137">description</span></span>|<span data-ttu-id="256e3-138">Строка</span><span class="sxs-lookup"><span data-stu-id="256e3-138">String</span></span>|<span data-ttu-id="256e3-139">Локализованное описание параметров политики в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="256e3-139">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="256e3-140">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="256e3-140">The default value is empty.</span></span> <span data-ttu-id="256e3-141">Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="256e3-141">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="256e3-142">languageCodes</span><span class="sxs-lookup"><span data-stu-id="256e3-142">languageCodes</span></span>|<span data-ttu-id="256e3-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="256e3-143">String collection</span></span>|<span data-ttu-id="256e3-144">Поддерживаемые языковые коды для файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="256e3-144">The supported language codes for the ADMX file.</span></span> <span data-ttu-id="256e3-145">Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="256e3-145">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="256e3-146">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="256e3-146">targetPrefix</span></span>|<span data-ttu-id="256e3-147">Строка</span><span class="sxs-lookup"><span data-stu-id="256e3-147">String</span></span>|<span data-ttu-id="256e3-148">Указывает логическое имя, которое ссылается на пространство имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="256e3-148">Specifies the logical name that refers to the namespace within the ADMX file.</span></span> <span data-ttu-id="256e3-149">Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="256e3-149">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="256e3-150">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="256e3-150">targetNamespace</span></span>|<span data-ttu-id="256e3-151">Строка</span><span class="sxs-lookup"><span data-stu-id="256e3-151">String</span></span>|<span data-ttu-id="256e3-152">Указывает URI, используемую для определения пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="256e3-152">Specifies the URI used to identify the namespace within the ADMX file.</span></span> <span data-ttu-id="256e3-153">Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="256e3-153">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="256e3-154">policyType</span><span class="sxs-lookup"><span data-stu-id="256e3-154">policyType</span></span>|[<span data-ttu-id="256e3-155">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="256e3-155">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="256e3-156">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="256e3-156">Specifies the type of group policy.</span></span> <span data-ttu-id="256e3-157">Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="256e3-157">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span> <span data-ttu-id="256e3-158">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="256e3-158">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="256e3-159">изменение</span><span class="sxs-lookup"><span data-stu-id="256e3-159">revision</span></span>|<span data-ttu-id="256e3-160">Строка</span><span class="sxs-lookup"><span data-stu-id="256e3-160">String</span></span>|<span data-ttu-id="256e3-161">Версия изменения, связанная с файлом.</span><span class="sxs-lookup"><span data-stu-id="256e3-161">The revision version associated with the file.</span></span> <span data-ttu-id="256e3-162">Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="256e3-162">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="256e3-163">id</span><span class="sxs-lookup"><span data-stu-id="256e3-163">id</span></span>|<span data-ttu-id="256e3-164">Строка</span><span class="sxs-lookup"><span data-stu-id="256e3-164">String</span></span>|<span data-ttu-id="256e3-165">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="256e3-165">Key of the entity.</span></span> <span data-ttu-id="256e3-166">Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="256e3-166">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="256e3-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="256e3-167">lastModifiedDateTime</span></span>|<span data-ttu-id="256e3-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="256e3-168">DateTimeOffset</span></span>|<span data-ttu-id="256e3-169">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="256e3-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="256e3-170">Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="256e3-170">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="256e3-171">fileName</span><span class="sxs-lookup"><span data-stu-id="256e3-171">fileName</span></span>|<span data-ttu-id="256e3-172">String</span><span class="sxs-lookup"><span data-stu-id="256e3-172">String</span></span>|<span data-ttu-id="256e3-173">Имя файла загруженного ADML-файла.</span><span class="sxs-lookup"><span data-stu-id="256e3-173">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="256e3-174">status</span><span class="sxs-lookup"><span data-stu-id="256e3-174">status</span></span>|[<span data-ttu-id="256e3-175">groupPolicyUploadedDefinitionFileStatus</span><span class="sxs-lookup"><span data-stu-id="256e3-175">groupPolicyUploadedDefinitionFileStatus</span></span>](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|<span data-ttu-id="256e3-176">Состояние загрузки загруженного файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="256e3-176">The upload status of the uploaded ADMX file.</span></span> <span data-ttu-id="256e3-177">Возможные значения: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.</span><span class="sxs-lookup"><span data-stu-id="256e3-177">Possible values are: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.</span></span>|
|<span data-ttu-id="256e3-178">содержимое</span><span class="sxs-lookup"><span data-stu-id="256e3-178">content</span></span>|<span data-ttu-id="256e3-179">Binary</span><span class="sxs-lookup"><span data-stu-id="256e3-179">Binary</span></span>|<span data-ttu-id="256e3-180">Содержимое загруженного файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="256e3-180">The contents of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="256e3-181">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="256e3-181">uploadDateTime</span></span>|<span data-ttu-id="256e3-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="256e3-182">DateTimeOffset</span></span>|<span data-ttu-id="256e3-183">Время загрузки загруженного файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="256e3-183">The uploaded time of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="256e3-184">defaultLanguageCode</span><span class="sxs-lookup"><span data-stu-id="256e3-184">defaultLanguageCode</span></span>|<span data-ttu-id="256e3-185">Строка</span><span class="sxs-lookup"><span data-stu-id="256e3-185">String</span></span>|<span data-ttu-id="256e3-186">Язык по умолчанию загруженного файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="256e3-186">The default language of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="256e3-187">groupPolicyUploadedLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="256e3-187">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="256e3-188">[коллекция groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="256e3-188">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="256e3-189">Список ADML-файлов, связанных с загруженным ADMX-файлом.</span><span class="sxs-lookup"><span data-stu-id="256e3-189">The list of ADML files associated with the uploaded ADMX file.</span></span>|



## <a name="response"></a><span data-ttu-id="256e3-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="256e3-190">Response</span></span>
<span data-ttu-id="256e3-191">В случае успеха этот метод возвращает код ответа и `201 Created` [объект groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="256e3-191">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="256e3-192">Пример</span><span class="sxs-lookup"><span data-stu-id="256e3-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="256e3-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="256e3-193">Request</span></span>
<span data-ttu-id="256e3-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="256e3-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles
Content-type: application/json
Content-length: 922

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="256e3-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="256e3-195">Response</span></span>
<span data-ttu-id="256e3-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="256e3-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1035

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "id": "0ce1a8cf-a8cf-0ce1-cfa8-e10ccfa8e10c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




