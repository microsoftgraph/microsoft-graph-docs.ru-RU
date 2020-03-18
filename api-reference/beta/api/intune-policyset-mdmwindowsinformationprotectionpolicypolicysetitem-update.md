---
title: Обновление Мдмвиндовсинформатионпротектионполициполицисетитем
description: Обновление свойств объекта Мдмвиндовсинформатионпротектионполициполицисетитем.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5fe56566b4426c80fa12d736be0ca8c857d6a92
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802190"
---
# <a name="update-mdmwindowsinformationprotectionpolicypolicysetitem"></a><span data-ttu-id="43ff2-103">Обновление Мдмвиндовсинформатионпротектионполициполицисетитем</span><span class="sxs-lookup"><span data-stu-id="43ff2-103">Update mdmWindowsInformationProtectionPolicyPolicySetItem</span></span>

> <span data-ttu-id="43ff2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43ff2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43ff2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43ff2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43ff2-106">Обновление свойств объекта [мдмвиндовсинформатионпротектионполициполицисетитем](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="43ff2-106">Update the properties of a [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43ff2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43ff2-107">Prerequisites</span></span>
<span data-ttu-id="43ff2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43ff2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43ff2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43ff2-110">Permission type</span></span>|<span data-ttu-id="43ff2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43ff2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43ff2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43ff2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43ff2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43ff2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43ff2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43ff2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43ff2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43ff2-115">Not supported.</span></span>|
|<span data-ttu-id="43ff2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="43ff2-116">Application</span></span>|<span data-ttu-id="43ff2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43ff2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43ff2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43ff2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="43ff2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="43ff2-119">Request headers</span></span>
|<span data-ttu-id="43ff2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43ff2-120">Header</span></span>|<span data-ttu-id="43ff2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="43ff2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43ff2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="43ff2-122">Authorization</span></span>|<span data-ttu-id="43ff2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43ff2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43ff2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="43ff2-124">Accept</span></span>|<span data-ttu-id="43ff2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43ff2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43ff2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43ff2-126">Request body</span></span>
<span data-ttu-id="43ff2-127">В тексте запроса добавьте представление объекта [мдмвиндовсинформатионпротектионполициполицисетитем](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43ff2-127">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object.</span></span>

<span data-ttu-id="43ff2-128">В следующей таблице приведены свойства, необходимые при создании [мдмвиндовсинформатионпротектионполициполицисетитем](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="43ff2-128">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md).</span></span>

|<span data-ttu-id="43ff2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="43ff2-129">Property</span></span>|<span data-ttu-id="43ff2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="43ff2-130">Type</span></span>|<span data-ttu-id="43ff2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="43ff2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43ff2-132">id</span><span class="sxs-lookup"><span data-stu-id="43ff2-132">id</span></span>|<span data-ttu-id="43ff2-133">String</span><span class="sxs-lookup"><span data-stu-id="43ff2-133">String</span></span>|<span data-ttu-id="43ff2-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="43ff2-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="43ff2-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="43ff2-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="43ff2-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43ff2-136">createdDateTime</span></span>|<span data-ttu-id="43ff2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43ff2-137">DateTimeOffset</span></span>|<span data-ttu-id="43ff2-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="43ff2-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="43ff2-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="43ff2-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="43ff2-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43ff2-140">lastModifiedDateTime</span></span>|<span data-ttu-id="43ff2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43ff2-141">DateTimeOffset</span></span>|<span data-ttu-id="43ff2-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="43ff2-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="43ff2-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="43ff2-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="43ff2-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="43ff2-144">payloadId</span></span>|<span data-ttu-id="43ff2-145">String</span><span class="sxs-lookup"><span data-stu-id="43ff2-145">String</span></span>|<span data-ttu-id="43ff2-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="43ff2-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="43ff2-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="43ff2-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="43ff2-148">itemType</span><span class="sxs-lookup"><span data-stu-id="43ff2-148">itemType</span></span>|<span data-ttu-id="43ff2-149">String</span><span class="sxs-lookup"><span data-stu-id="43ff2-149">String</span></span>|<span data-ttu-id="43ff2-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="43ff2-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="43ff2-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="43ff2-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="43ff2-152">displayName</span><span class="sxs-lookup"><span data-stu-id="43ff2-152">displayName</span></span>|<span data-ttu-id="43ff2-153">Строка</span><span class="sxs-lookup"><span data-stu-id="43ff2-153">String</span></span>|<span data-ttu-id="43ff2-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="43ff2-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="43ff2-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="43ff2-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="43ff2-156">status</span><span class="sxs-lookup"><span data-stu-id="43ff2-156">status</span></span>|[<span data-ttu-id="43ff2-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="43ff2-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="43ff2-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="43ff2-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="43ff2-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="43ff2-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="43ff2-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="43ff2-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="43ff2-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="43ff2-161">errorCode</span></span>|[<span data-ttu-id="43ff2-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="43ff2-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="43ff2-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="43ff2-163">Error code if any occured.</span></span> <span data-ttu-id="43ff2-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="43ff2-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="43ff2-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="43ff2-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="43ff2-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="43ff2-166">guidedDeploymentTags</span></span>|<span data-ttu-id="43ff2-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="43ff2-167">String collection</span></span>|<span data-ttu-id="43ff2-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="43ff2-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="43ff2-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="43ff2-169">Response</span></span>
<span data-ttu-id="43ff2-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мдмвиндовсинформатионпротектионполициполицисетитем](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43ff2-170">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43ff2-171">Пример</span><span class="sxs-lookup"><span data-stu-id="43ff2-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="43ff2-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="43ff2-172">Request</span></span>
<span data-ttu-id="43ff2-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43ff2-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
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

### <a name="response"></a><span data-ttu-id="43ff2-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="43ff2-174">Response</span></span>
<span data-ttu-id="43ff2-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43ff2-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




