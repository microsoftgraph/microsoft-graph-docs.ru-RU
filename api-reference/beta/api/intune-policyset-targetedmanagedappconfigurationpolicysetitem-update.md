---
title: Обновление Таржетедманажедаппконфигуратионполицисетитем
description: Обновление свойств объекта Таржетедманажедаппконфигуратионполицисетитем.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6028d982bb2320e00a5d438c10c0d06e926d385
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802029"
---
# <a name="update-targetedmanagedappconfigurationpolicysetitem"></a><span data-ttu-id="d608f-103">Обновление Таржетедманажедаппконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="d608f-103">Update targetedManagedAppConfigurationPolicySetItem</span></span>

> <span data-ttu-id="d608f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d608f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d608f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d608f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d608f-106">Обновление свойств объекта [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="d608f-106">Update the properties of a [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d608f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d608f-107">Prerequisites</span></span>
<span data-ttu-id="d608f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d608f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d608f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d608f-110">Permission type</span></span>|<span data-ttu-id="d608f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d608f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d608f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d608f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d608f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d608f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d608f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d608f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d608f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d608f-115">Not supported.</span></span>|
|<span data-ttu-id="d608f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d608f-116">Application</span></span>|<span data-ttu-id="d608f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d608f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d608f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d608f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="d608f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d608f-119">Request headers</span></span>
|<span data-ttu-id="d608f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d608f-120">Header</span></span>|<span data-ttu-id="d608f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d608f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d608f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d608f-122">Authorization</span></span>|<span data-ttu-id="d608f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d608f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d608f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d608f-124">Accept</span></span>|<span data-ttu-id="d608f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d608f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d608f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d608f-126">Request body</span></span>
<span data-ttu-id="d608f-127">В тексте запроса добавьте представление объекта [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d608f-127">In the request body, supply a JSON representation for the [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="d608f-128">В следующей таблице приведены свойства, необходимые при создании [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="d608f-128">The following table shows the properties that are required when you create the [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="d608f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d608f-129">Property</span></span>|<span data-ttu-id="d608f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d608f-130">Type</span></span>|<span data-ttu-id="d608f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d608f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d608f-132">id</span><span class="sxs-lookup"><span data-stu-id="d608f-132">id</span></span>|<span data-ttu-id="d608f-133">String</span><span class="sxs-lookup"><span data-stu-id="d608f-133">String</span></span>|<span data-ttu-id="d608f-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="d608f-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="d608f-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d608f-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d608f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d608f-136">createdDateTime</span></span>|<span data-ttu-id="d608f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d608f-137">DateTimeOffset</span></span>|<span data-ttu-id="d608f-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="d608f-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="d608f-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d608f-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d608f-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d608f-140">lastModifiedDateTime</span></span>|<span data-ttu-id="d608f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d608f-141">DateTimeOffset</span></span>|<span data-ttu-id="d608f-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="d608f-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="d608f-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d608f-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d608f-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="d608f-144">payloadId</span></span>|<span data-ttu-id="d608f-145">String</span><span class="sxs-lookup"><span data-stu-id="d608f-145">String</span></span>|<span data-ttu-id="d608f-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="d608f-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="d608f-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d608f-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d608f-148">itemType</span><span class="sxs-lookup"><span data-stu-id="d608f-148">itemType</span></span>|<span data-ttu-id="d608f-149">String</span><span class="sxs-lookup"><span data-stu-id="d608f-149">String</span></span>|<span data-ttu-id="d608f-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="d608f-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="d608f-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d608f-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d608f-152">displayName</span><span class="sxs-lookup"><span data-stu-id="d608f-152">displayName</span></span>|<span data-ttu-id="d608f-153">Строка</span><span class="sxs-lookup"><span data-stu-id="d608f-153">String</span></span>|<span data-ttu-id="d608f-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="d608f-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="d608f-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d608f-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="d608f-156">status</span><span class="sxs-lookup"><span data-stu-id="d608f-156">status</span></span>|[<span data-ttu-id="d608f-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="d608f-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="d608f-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="d608f-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="d608f-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="d608f-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="d608f-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d608f-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="d608f-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="d608f-161">errorCode</span></span>|[<span data-ttu-id="d608f-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="d608f-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="d608f-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="d608f-163">Error code if any occured.</span></span> <span data-ttu-id="d608f-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="d608f-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="d608f-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="d608f-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="d608f-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="d608f-166">guidedDeploymentTags</span></span>|<span data-ttu-id="d608f-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d608f-167">String collection</span></span>|<span data-ttu-id="d608f-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d608f-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d608f-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="d608f-169">Response</span></span>
<span data-ttu-id="d608f-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d608f-170">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d608f-171">Пример</span><span class="sxs-lookup"><span data-stu-id="d608f-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="d608f-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="d608f-172">Request</span></span>
<span data-ttu-id="d608f-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d608f-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 326

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfigurationPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="d608f-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="d608f-174">Response</span></span>
<span data-ttu-id="d608f-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d608f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 498

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfigurationPolicySetItem",
  "id": "f86d3112-3112-f86d-1231-6df812316df8",
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




