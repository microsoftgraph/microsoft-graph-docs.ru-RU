---
title: Создание mdmWindowsInformationProtectionPolicyPolicySetItem
description: Создание нового объекта mdmWindowsInformationProtectionPolicyPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a8b33d3100e98ea634f1b48d712117274e311c2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156683"
---
# <a name="create-mdmwindowsinformationprotectionpolicypolicysetitem"></a><span data-ttu-id="b705e-103">Создание mdmWindowsInformationProtectionPolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="b705e-103">Create mdmWindowsInformationProtectionPolicyPolicySetItem</span></span>

<span data-ttu-id="b705e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b705e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b705e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b705e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b705e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b705e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b705e-107">Создание нового [объекта mdmWindowsInformationProtectionPolicyPolicySetItem.](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b705e-107">Create a new [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b705e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b705e-108">Prerequisites</span></span>
<span data-ttu-id="b705e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b705e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b705e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b705e-111">Permission type</span></span>|<span data-ttu-id="b705e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b705e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b705e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b705e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b705e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b705e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b705e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b705e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b705e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b705e-116">Not supported.</span></span>|
|<span data-ttu-id="b705e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b705e-117">Application</span></span>|<span data-ttu-id="b705e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b705e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b705e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b705e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="b705e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b705e-120">Request headers</span></span>
|<span data-ttu-id="b705e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b705e-121">Header</span></span>|<span data-ttu-id="b705e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b705e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b705e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b705e-123">Authorization</span></span>|<span data-ttu-id="b705e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b705e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b705e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b705e-125">Accept</span></span>|<span data-ttu-id="b705e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b705e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b705e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b705e-127">Request body</span></span>
<span data-ttu-id="b705e-128">В теле запроса поставляем представление JSON для объекта mdmWindowsInformationProtectionPolicyPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b705e-128">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicyPolicySetItem object.</span></span>

<span data-ttu-id="b705e-129">В следующей таблице показаны свойства, необходимые при создании mdmWindowsInformationProtectionPolicyPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b705e-129">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicyPolicySetItem.</span></span>

|<span data-ttu-id="b705e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b705e-130">Property</span></span>|<span data-ttu-id="b705e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b705e-131">Type</span></span>|<span data-ttu-id="b705e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b705e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b705e-133">id</span><span class="sxs-lookup"><span data-stu-id="b705e-133">id</span></span>|<span data-ttu-id="b705e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b705e-134">String</span></span>|<span data-ttu-id="b705e-135">Клавиша MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b705e-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="b705e-136">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b705e-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b705e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b705e-137">createdDateTime</span></span>|<span data-ttu-id="b705e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b705e-138">DateTimeOffset</span></span>|<span data-ttu-id="b705e-139">Время создания PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b705e-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="b705e-140">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b705e-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b705e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b705e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b705e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b705e-142">DateTimeOffset</span></span>|<span data-ttu-id="b705e-143">Последнее измененное время политикиSetItem.</span><span class="sxs-lookup"><span data-stu-id="b705e-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="b705e-144">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b705e-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b705e-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="b705e-145">payloadId</span></span>|<span data-ttu-id="b705e-146">Строка</span><span class="sxs-lookup"><span data-stu-id="b705e-146">String</span></span>|<span data-ttu-id="b705e-147">PayloadId of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b705e-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="b705e-148">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b705e-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b705e-149">itemType</span><span class="sxs-lookup"><span data-stu-id="b705e-149">itemType</span></span>|<span data-ttu-id="b705e-150">Строка</span><span class="sxs-lookup"><span data-stu-id="b705e-150">String</span></span>|<span data-ttu-id="b705e-151">policySetType policySetItem.</span><span class="sxs-lookup"><span data-stu-id="b705e-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="b705e-152">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b705e-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b705e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b705e-153">displayName</span></span>|<span data-ttu-id="b705e-154">Строка</span><span class="sxs-lookup"><span data-stu-id="b705e-154">String</span></span>|<span data-ttu-id="b705e-155">DisplayName of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b705e-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="b705e-156">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b705e-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b705e-157">status</span><span class="sxs-lookup"><span data-stu-id="b705e-157">status</span></span>|[<span data-ttu-id="b705e-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="b705e-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="b705e-159">Состояние PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b705e-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="b705e-160">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="b705e-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b705e-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b705e-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="b705e-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="b705e-162">errorCode</span></span>|[<span data-ttu-id="b705e-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="b705e-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="b705e-164">Код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="b705e-164">Error code if any occured.</span></span> <span data-ttu-id="b705e-165">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="b705e-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b705e-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="b705e-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="b705e-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="b705e-167">guidedDeploymentTags</span></span>|<span data-ttu-id="b705e-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b705e-168">String collection</span></span>|<span data-ttu-id="b705e-169">Теги управляемого развертывания, унаследованной [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b705e-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b705e-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="b705e-170">Response</span></span>
<span data-ttu-id="b705e-171">В случае успеха этот метод возвращает код ответа и `201 Created` [объект mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b705e-171">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b705e-172">Пример</span><span class="sxs-lookup"><span data-stu-id="b705e-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="b705e-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="b705e-173">Request</span></span>
<span data-ttu-id="b705e-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b705e-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b705e-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="b705e-175">Response</span></span>
<span data-ttu-id="b705e-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b705e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem",
  "id": "4ac5be70-be70-4ac5-70be-c54a70bec54a",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```




