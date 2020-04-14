---
title: Создание Граупполициуплоадеддефинитионфиле
description: Создание нового объекта Граупполициуплоадеддефинитионфиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 828464d5a0e620a713eac7187b6a8883ea7a2648
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388652"
---
# <a name="create-grouppolicyuploadeddefinitionfile"></a><span data-ttu-id="1a781-103">Создание Граупполициуплоадеддефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="1a781-103">Create groupPolicyUploadedDefinitionFile</span></span>

<span data-ttu-id="1a781-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a781-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a781-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a781-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a781-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a781-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a781-107">Создание нового объекта [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="1a781-107">Create a new [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a781-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1a781-108">Prerequisites</span></span>
<span data-ttu-id="1a781-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a781-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a781-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a781-111">Permission type</span></span>|<span data-ttu-id="1a781-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a781-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a781-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a781-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a781-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a781-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a781-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a781-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a781-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a781-116">Not supported.</span></span>|
|<span data-ttu-id="1a781-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1a781-117">Application</span></span>|<span data-ttu-id="1a781-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a781-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a781-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a781-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## <a name="request-headers"></a><span data-ttu-id="1a781-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1a781-120">Request headers</span></span>
|<span data-ttu-id="1a781-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a781-121">Header</span></span>|<span data-ttu-id="1a781-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1a781-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a781-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a781-123">Authorization</span></span>|<span data-ttu-id="1a781-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a781-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a781-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1a781-125">Accept</span></span>|<span data-ttu-id="1a781-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a781-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a781-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a781-127">Request body</span></span>
<span data-ttu-id="1a781-128">В тексте запроса добавьте представление объекта Граупполициуплоадеддефинитионфиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a781-128">In the request body, supply a JSON representation for the groupPolicyUploadedDefinitionFile object.</span></span>

<span data-ttu-id="1a781-129">В следующей таблице приведены свойства, необходимые при создании Граупполициуплоадеддефинитионфиле.</span><span class="sxs-lookup"><span data-stu-id="1a781-129">The following table shows the properties that are required when you create the groupPolicyUploadedDefinitionFile.</span></span>

|<span data-ttu-id="1a781-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a781-130">Property</span></span>|<span data-ttu-id="1a781-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1a781-131">Type</span></span>|<span data-ttu-id="1a781-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1a781-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a781-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1a781-133">displayName</span></span>|<span data-ttu-id="1a781-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1a781-134">String</span></span>|<span data-ttu-id="1a781-135">Локализованное понятное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="1a781-135">The localized friendly name of the ADMX file.</span></span> <span data-ttu-id="1a781-136">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="1a781-136">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="1a781-137">description</span><span class="sxs-lookup"><span data-stu-id="1a781-137">description</span></span>|<span data-ttu-id="1a781-138">String</span><span class="sxs-lookup"><span data-stu-id="1a781-138">String</span></span>|<span data-ttu-id="1a781-139">Локализованное описание параметров политики в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="1a781-139">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="1a781-140">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="1a781-140">The default value is empty.</span></span> <span data-ttu-id="1a781-141">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="1a781-141">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="1a781-142">лангуажекодес</span><span class="sxs-lookup"><span data-stu-id="1a781-142">languageCodes</span></span>|<span data-ttu-id="1a781-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1a781-143">String collection</span></span>|<span data-ttu-id="1a781-144">Поддерживаемые коды языков для ADMX.</span><span class="sxs-lookup"><span data-stu-id="1a781-144">The supported language codes for the ADMX file.</span></span> <span data-ttu-id="1a781-145">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="1a781-145">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="1a781-146">таржетпрефикс</span><span class="sxs-lookup"><span data-stu-id="1a781-146">targetPrefix</span></span>|<span data-ttu-id="1a781-147">String</span><span class="sxs-lookup"><span data-stu-id="1a781-147">String</span></span>|<span data-ttu-id="1a781-148">Задает логическое имя, которое ссылается на пространство имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="1a781-148">Specifies the logical name that refers to the namespace within the ADMX file.</span></span> <span data-ttu-id="1a781-149">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="1a781-149">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="1a781-150">Атрибут</span><span class="sxs-lookup"><span data-stu-id="1a781-150">targetNamespace</span></span>|<span data-ttu-id="1a781-151">String</span><span class="sxs-lookup"><span data-stu-id="1a781-151">String</span></span>|<span data-ttu-id="1a781-152">Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="1a781-152">Specifies the URI used to identify the namespace within the ADMX file.</span></span> <span data-ttu-id="1a781-153">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="1a781-153">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="1a781-154">полицитипе</span><span class="sxs-lookup"><span data-stu-id="1a781-154">policyType</span></span>|[<span data-ttu-id="1a781-155">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="1a781-155">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="1a781-156">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="1a781-156">Specifies the type of group policy.</span></span> <span data-ttu-id="1a781-157">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="1a781-157">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span> <span data-ttu-id="1a781-158">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="1a781-158">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="1a781-159">последним</span><span class="sxs-lookup"><span data-stu-id="1a781-159">revision</span></span>|<span data-ttu-id="1a781-160">String</span><span class="sxs-lookup"><span data-stu-id="1a781-160">String</span></span>|<span data-ttu-id="1a781-161">Версия редакции, связанная с файлом.</span><span class="sxs-lookup"><span data-stu-id="1a781-161">The revision version associated with the file.</span></span> <span data-ttu-id="1a781-162">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="1a781-162">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="1a781-163">id</span><span class="sxs-lookup"><span data-stu-id="1a781-163">id</span></span>|<span data-ttu-id="1a781-164">Строка</span><span class="sxs-lookup"><span data-stu-id="1a781-164">String</span></span>|<span data-ttu-id="1a781-165">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1a781-165">Key of the entity.</span></span> <span data-ttu-id="1a781-166">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="1a781-166">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="1a781-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a781-167">lastModifiedDateTime</span></span>|<span data-ttu-id="1a781-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a781-168">DateTimeOffset</span></span>|<span data-ttu-id="1a781-169">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1a781-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="1a781-170">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="1a781-170">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="1a781-171">fileName</span><span class="sxs-lookup"><span data-stu-id="1a781-171">fileName</span></span>|<span data-ttu-id="1a781-172">String</span><span class="sxs-lookup"><span data-stu-id="1a781-172">String</span></span>|<span data-ttu-id="1a781-173">Имя файла загруженного файла ADML.</span><span class="sxs-lookup"><span data-stu-id="1a781-173">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="1a781-174">status</span><span class="sxs-lookup"><span data-stu-id="1a781-174">status</span></span>|[<span data-ttu-id="1a781-175">граупполициуплоадеддефинитионфилестатус</span><span class="sxs-lookup"><span data-stu-id="1a781-175">groupPolicyUploadedDefinitionFileStatus</span></span>](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|<span data-ttu-id="1a781-176">Состояние отправки для отправленного ADMX файла.</span><span class="sxs-lookup"><span data-stu-id="1a781-176">The upload status of the uploaded ADMX file.</span></span> <span data-ttu-id="1a781-177">Возможные значения: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.</span><span class="sxs-lookup"><span data-stu-id="1a781-177">Possible values are: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.</span></span>|
|<span data-ttu-id="1a781-178">содержимое</span><span class="sxs-lookup"><span data-stu-id="1a781-178">content</span></span>|<span data-ttu-id="1a781-179">Binary</span><span class="sxs-lookup"><span data-stu-id="1a781-179">Binary</span></span>|<span data-ttu-id="1a781-180">Содержимое отправленного ADMX файла.</span><span class="sxs-lookup"><span data-stu-id="1a781-180">The contents of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="1a781-181">уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="1a781-181">uploadDateTime</span></span>|<span data-ttu-id="1a781-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a781-182">DateTimeOffset</span></span>|<span data-ttu-id="1a781-183">Время отправки файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="1a781-183">The uploaded time of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="1a781-184">дефаултлангуажекоде</span><span class="sxs-lookup"><span data-stu-id="1a781-184">defaultLanguageCode</span></span>|<span data-ttu-id="1a781-185">String</span><span class="sxs-lookup"><span data-stu-id="1a781-185">String</span></span>|<span data-ttu-id="1a781-186">Язык по умолчанию для отправленного файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="1a781-186">The default language of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="1a781-187">граупполициуплоадедлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="1a781-187">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="1a781-188">Коллекция [граупполициуплоадедлангуажефиле](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="1a781-188">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="1a781-189">Список файлов ADML, связанных с отправленным ADMX файлом.</span><span class="sxs-lookup"><span data-stu-id="1a781-189">The list of ADML files associated with the uploaded ADMX file.</span></span>|



## <a name="response"></a><span data-ttu-id="1a781-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a781-190">Response</span></span>
<span data-ttu-id="1a781-191">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a781-191">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a781-192">Пример</span><span class="sxs-lookup"><span data-stu-id="1a781-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a781-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a781-193">Request</span></span>
<span data-ttu-id="1a781-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a781-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1a781-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a781-195">Response</span></span>
<span data-ttu-id="1a781-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a781-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



