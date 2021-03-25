---
title: Update groupPolicyDefinitionFile
description: Обновление свойств объекта groupPolicyDefinitionFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0910406f564f86decf211285ed472f57792267c5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158894"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="b4a45-103">Update groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="b4a45-103">Update groupPolicyDefinitionFile</span></span>

<span data-ttu-id="b4a45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4a45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4a45-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4a45-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4a45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4a45-107">Обновление свойств объекта [groupPolicyDefinitionFile.](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="b4a45-107">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4a45-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b4a45-108">Prerequisites</span></span>
<span data-ttu-id="b4a45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4a45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4a45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4a45-111">Permission type</span></span>|<span data-ttu-id="b4a45-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4a45-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4a45-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4a45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4a45-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4a45-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4a45-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4a45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4a45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a45-116">Not supported.</span></span>|
|<span data-ttu-id="b4a45-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b4a45-117">Application</span></span>|<span data-ttu-id="b4a45-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4a45-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4a45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4a45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="b4a45-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b4a45-120">Request headers</span></span>
|<span data-ttu-id="b4a45-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4a45-121">Header</span></span>|<span data-ttu-id="b4a45-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b4a45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4a45-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4a45-123">Authorization</span></span>|<span data-ttu-id="b4a45-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4a45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4a45-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4a45-125">Accept</span></span>|<span data-ttu-id="b4a45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4a45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4a45-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4a45-127">Request body</span></span>
<span data-ttu-id="b4a45-128">В теле запроса поставляем представление JSON для [объекта groupPolicyDefinitionFile.](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="b4a45-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="b4a45-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyDefinitionFile.](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)</span><span class="sxs-lookup"><span data-stu-id="b4a45-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="b4a45-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4a45-130">Property</span></span>|<span data-ttu-id="b4a45-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b4a45-131">Type</span></span>|<span data-ttu-id="b4a45-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b4a45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4a45-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b4a45-133">displayName</span></span>|<span data-ttu-id="b4a45-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b4a45-134">String</span></span>|<span data-ttu-id="b4a45-135">Локализованное удобное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="b4a45-135">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="b4a45-136">description</span><span class="sxs-lookup"><span data-stu-id="b4a45-136">description</span></span>|<span data-ttu-id="b4a45-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b4a45-137">String</span></span>|<span data-ttu-id="b4a45-138">Локализованное описание параметров политики в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="b4a45-138">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="b4a45-139">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="b4a45-139">The default value is empty.</span></span>|
|<span data-ttu-id="b4a45-140">languageCodes</span><span class="sxs-lookup"><span data-stu-id="b4a45-140">languageCodes</span></span>|<span data-ttu-id="b4a45-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b4a45-141">String collection</span></span>|<span data-ttu-id="b4a45-142">Поддерживаемые языковые коды для файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="b4a45-142">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="b4a45-143">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="b4a45-143">targetPrefix</span></span>|<span data-ttu-id="b4a45-144">Строка</span><span class="sxs-lookup"><span data-stu-id="b4a45-144">String</span></span>|<span data-ttu-id="b4a45-145">Указывает логическое имя, которое ссылается на пространство имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="b4a45-145">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="b4a45-146">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="b4a45-146">targetNamespace</span></span>|<span data-ttu-id="b4a45-147">Строка</span><span class="sxs-lookup"><span data-stu-id="b4a45-147">String</span></span>|<span data-ttu-id="b4a45-148">Указывает URI, используемую для определения пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="b4a45-148">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="b4a45-149">policyType</span><span class="sxs-lookup"><span data-stu-id="b4a45-149">policyType</span></span>|[<span data-ttu-id="b4a45-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="b4a45-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="b4a45-151">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="b4a45-151">Specifies the type of group policy.</span></span> <span data-ttu-id="b4a45-152">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="b4a45-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="b4a45-153">изменение</span><span class="sxs-lookup"><span data-stu-id="b4a45-153">revision</span></span>|<span data-ttu-id="b4a45-154">Строка</span><span class="sxs-lookup"><span data-stu-id="b4a45-154">String</span></span>|<span data-ttu-id="b4a45-155">Версия изменения, связанная с файлом.</span><span class="sxs-lookup"><span data-stu-id="b4a45-155">The revision version associated with the file.</span></span>|
|<span data-ttu-id="b4a45-156">id</span><span class="sxs-lookup"><span data-stu-id="b4a45-156">id</span></span>|<span data-ttu-id="b4a45-157">Строка</span><span class="sxs-lookup"><span data-stu-id="b4a45-157">String</span></span>|<span data-ttu-id="b4a45-158">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b4a45-158">Key of the entity.</span></span>|
|<span data-ttu-id="b4a45-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4a45-159">lastModifiedDateTime</span></span>|<span data-ttu-id="b4a45-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4a45-160">DateTimeOffset</span></span>|<span data-ttu-id="b4a45-161">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b4a45-161">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="b4a45-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4a45-162">Response</span></span>
<span data-ttu-id="b4a45-163">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b4a45-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4a45-164">Пример</span><span class="sxs-lookup"><span data-stu-id="b4a45-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4a45-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4a45-165">Request</span></span>
<span data-ttu-id="b4a45-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4a45-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 358

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value"
}
```

### <a name="response"></a><span data-ttu-id="b4a45-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4a45-167">Response</span></span>
<span data-ttu-id="b4a45-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4a45-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




