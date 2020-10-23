---
title: Создание Граупполициуплоадеддефинитионфиле
description: Создание нового объекта Граупполициуплоадеддефинитионфиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7cd05240b3532d19bed4101fe88153fe57960deb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708104"
---
# <a name="create-grouppolicyuploadeddefinitionfile"></a><span data-ttu-id="01e25-103">Создание Граупполициуплоадеддефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="01e25-103">Create groupPolicyUploadedDefinitionFile</span></span>

<span data-ttu-id="01e25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01e25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01e25-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01e25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01e25-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01e25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01e25-107">Создание нового объекта [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="01e25-107">Create a new [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01e25-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01e25-108">Prerequisites</span></span>
<span data-ttu-id="01e25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01e25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01e25-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01e25-111">Permission type</span></span>|<span data-ttu-id="01e25-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01e25-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01e25-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01e25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01e25-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01e25-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01e25-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01e25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01e25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01e25-116">Not supported.</span></span>|
|<span data-ttu-id="01e25-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01e25-117">Application</span></span>|<span data-ttu-id="01e25-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01e25-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01e25-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01e25-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## <a name="request-headers"></a><span data-ttu-id="01e25-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="01e25-120">Request headers</span></span>
|<span data-ttu-id="01e25-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01e25-121">Header</span></span>|<span data-ttu-id="01e25-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01e25-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01e25-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01e25-123">Authorization</span></span>|<span data-ttu-id="01e25-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01e25-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01e25-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01e25-125">Accept</span></span>|<span data-ttu-id="01e25-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01e25-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01e25-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01e25-127">Request body</span></span>
<span data-ttu-id="01e25-128">В тексте запроса добавьте представление объекта Граупполициуплоадеддефинитионфиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01e25-128">In the request body, supply a JSON representation for the groupPolicyUploadedDefinitionFile object.</span></span>

<span data-ttu-id="01e25-129">В следующей таблице приведены свойства, необходимые при создании Граупполициуплоадеддефинитионфиле.</span><span class="sxs-lookup"><span data-stu-id="01e25-129">The following table shows the properties that are required when you create the groupPolicyUploadedDefinitionFile.</span></span>

|<span data-ttu-id="01e25-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01e25-130">Property</span></span>|<span data-ttu-id="01e25-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01e25-131">Type</span></span>|<span data-ttu-id="01e25-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01e25-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01e25-133">displayName</span><span class="sxs-lookup"><span data-stu-id="01e25-133">displayName</span></span>|<span data-ttu-id="01e25-134">Строка</span><span class="sxs-lookup"><span data-stu-id="01e25-134">String</span></span>|<span data-ttu-id="01e25-135">Локализованное понятное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="01e25-135">The localized friendly name of the ADMX file.</span></span> <span data-ttu-id="01e25-136">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="01e25-136">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="01e25-137">description</span><span class="sxs-lookup"><span data-stu-id="01e25-137">description</span></span>|<span data-ttu-id="01e25-138">Строка</span><span class="sxs-lookup"><span data-stu-id="01e25-138">String</span></span>|<span data-ttu-id="01e25-139">Локализованное описание параметров политики в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="01e25-139">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="01e25-140">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="01e25-140">The default value is empty.</span></span> <span data-ttu-id="01e25-141">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="01e25-141">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="01e25-142">лангуажекодес</span><span class="sxs-lookup"><span data-stu-id="01e25-142">languageCodes</span></span>|<span data-ttu-id="01e25-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="01e25-143">String collection</span></span>|<span data-ttu-id="01e25-144">Поддерживаемые коды языков для ADMX.</span><span class="sxs-lookup"><span data-stu-id="01e25-144">The supported language codes for the ADMX file.</span></span> <span data-ttu-id="01e25-145">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="01e25-145">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="01e25-146">таржетпрефикс</span><span class="sxs-lookup"><span data-stu-id="01e25-146">targetPrefix</span></span>|<span data-ttu-id="01e25-147">Строка</span><span class="sxs-lookup"><span data-stu-id="01e25-147">String</span></span>|<span data-ttu-id="01e25-148">Задает логическое имя, которое ссылается на пространство имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="01e25-148">Specifies the logical name that refers to the namespace within the ADMX file.</span></span> <span data-ttu-id="01e25-149">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="01e25-149">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="01e25-150">Атрибут</span><span class="sxs-lookup"><span data-stu-id="01e25-150">targetNamespace</span></span>|<span data-ttu-id="01e25-151">Строка</span><span class="sxs-lookup"><span data-stu-id="01e25-151">String</span></span>|<span data-ttu-id="01e25-152">Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="01e25-152">Specifies the URI used to identify the namespace within the ADMX file.</span></span> <span data-ttu-id="01e25-153">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="01e25-153">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="01e25-154">полицитипе</span><span class="sxs-lookup"><span data-stu-id="01e25-154">policyType</span></span>|[<span data-ttu-id="01e25-155">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="01e25-155">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="01e25-156">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="01e25-156">Specifies the type of group policy.</span></span> <span data-ttu-id="01e25-157">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="01e25-157">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span> <span data-ttu-id="01e25-158">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="01e25-158">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="01e25-159">последним</span><span class="sxs-lookup"><span data-stu-id="01e25-159">revision</span></span>|<span data-ttu-id="01e25-160">Строка</span><span class="sxs-lookup"><span data-stu-id="01e25-160">String</span></span>|<span data-ttu-id="01e25-161">Версия редакции, связанная с файлом.</span><span class="sxs-lookup"><span data-stu-id="01e25-161">The revision version associated with the file.</span></span> <span data-ttu-id="01e25-162">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="01e25-162">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="01e25-163">id</span><span class="sxs-lookup"><span data-stu-id="01e25-163">id</span></span>|<span data-ttu-id="01e25-164">Строка</span><span class="sxs-lookup"><span data-stu-id="01e25-164">String</span></span>|<span data-ttu-id="01e25-165">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01e25-165">Key of the entity.</span></span> <span data-ttu-id="01e25-166">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="01e25-166">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="01e25-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01e25-167">lastModifiedDateTime</span></span>|<span data-ttu-id="01e25-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01e25-168">DateTimeOffset</span></span>|<span data-ttu-id="01e25-169">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="01e25-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="01e25-170">Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="01e25-170">Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span></span>|
|<span data-ttu-id="01e25-171">fileName</span><span class="sxs-lookup"><span data-stu-id="01e25-171">fileName</span></span>|<span data-ttu-id="01e25-172">String</span><span class="sxs-lookup"><span data-stu-id="01e25-172">String</span></span>|<span data-ttu-id="01e25-173">Имя файла загруженного файла ADML.</span><span class="sxs-lookup"><span data-stu-id="01e25-173">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="01e25-174">status</span><span class="sxs-lookup"><span data-stu-id="01e25-174">status</span></span>|[<span data-ttu-id="01e25-175">groupPolicyUploadedDefinitionFileStatus</span><span class="sxs-lookup"><span data-stu-id="01e25-175">groupPolicyUploadedDefinitionFileStatus</span></span>](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|<span data-ttu-id="01e25-176">Состояние отправки для отправленного ADMX файла.</span><span class="sxs-lookup"><span data-stu-id="01e25-176">The upload status of the uploaded ADMX file.</span></span> <span data-ttu-id="01e25-177">Возможные значения: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.</span><span class="sxs-lookup"><span data-stu-id="01e25-177">Possible values are: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.</span></span>|
|<span data-ttu-id="01e25-178">содержимое</span><span class="sxs-lookup"><span data-stu-id="01e25-178">content</span></span>|<span data-ttu-id="01e25-179">Binary</span><span class="sxs-lookup"><span data-stu-id="01e25-179">Binary</span></span>|<span data-ttu-id="01e25-180">Содержимое отправленного ADMX файла.</span><span class="sxs-lookup"><span data-stu-id="01e25-180">The contents of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="01e25-181">уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="01e25-181">uploadDateTime</span></span>|<span data-ttu-id="01e25-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01e25-182">DateTimeOffset</span></span>|<span data-ttu-id="01e25-183">Время отправки файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="01e25-183">The uploaded time of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="01e25-184">дефаултлангуажекоде</span><span class="sxs-lookup"><span data-stu-id="01e25-184">defaultLanguageCode</span></span>|<span data-ttu-id="01e25-185">Строка</span><span class="sxs-lookup"><span data-stu-id="01e25-185">String</span></span>|<span data-ttu-id="01e25-186">Язык по умолчанию для отправленного файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="01e25-186">The default language of the uploaded ADMX file.</span></span>|
|<span data-ttu-id="01e25-187">граупполициуплоадедлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="01e25-187">groupPolicyUploadedLanguageFiles</span></span>|<span data-ttu-id="01e25-188">Коллекция [граупполициуплоадедлангуажефиле](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)</span><span class="sxs-lookup"><span data-stu-id="01e25-188">[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) collection</span></span>|<span data-ttu-id="01e25-189">Список файлов ADML, связанных с отправленным ADMX файлом.</span><span class="sxs-lookup"><span data-stu-id="01e25-189">The list of ADML files associated with the uploaded ADMX file.</span></span>|



## <a name="response"></a><span data-ttu-id="01e25-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="01e25-190">Response</span></span>
<span data-ttu-id="01e25-191">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01e25-191">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01e25-192">Пример</span><span class="sxs-lookup"><span data-stu-id="01e25-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="01e25-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="01e25-193">Request</span></span>
<span data-ttu-id="01e25-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01e25-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01e25-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="01e25-195">Response</span></span>
<span data-ttu-id="01e25-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01e25-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





