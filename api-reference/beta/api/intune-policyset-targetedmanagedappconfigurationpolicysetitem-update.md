---
title: Обновление Таржетедманажедаппконфигуратионполицисетитем
description: Обновление свойств объекта Таржетедманажедаппконфигуратионполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ff43525f99bd623122cf562d7107b9ec19da1dc
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940863"
---
# <a name="update-targetedmanagedappconfigurationpolicysetitem"></a><span data-ttu-id="2f2cc-103">Обновление Таржетедманажедаппконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="2f2cc-103">Update targetedManagedAppConfigurationPolicySetItem</span></span>

> <span data-ttu-id="2f2cc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f2cc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f2cc-106">Обновление свойств объекта [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="2f2cc-106">Update the properties of a [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f2cc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2f2cc-107">Prerequisites</span></span>
<span data-ttu-id="2f2cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f2cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f2cc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f2cc-110">Permission type</span></span>|<span data-ttu-id="2f2cc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f2cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f2cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f2cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f2cc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f2cc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f2cc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f2cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f2cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-115">Not supported.</span></span>|
|<span data-ttu-id="2f2cc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f2cc-116">Application</span></span>|<span data-ttu-id="2f2cc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f2cc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f2cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f2cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="2f2cc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2f2cc-119">Request headers</span></span>
|<span data-ttu-id="2f2cc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f2cc-120">Header</span></span>|<span data-ttu-id="2f2cc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2f2cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f2cc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f2cc-122">Authorization</span></span>|<span data-ttu-id="2f2cc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f2cc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2f2cc-124">Accept</span></span>|<span data-ttu-id="2f2cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f2cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f2cc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f2cc-126">Request body</span></span>
<span data-ttu-id="2f2cc-127">В тексте запроса добавьте представление объекта [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-127">In the request body, supply a JSON representation for the [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="2f2cc-128">В следующей таблице приведены свойства, необходимые при создании [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="2f2cc-128">The following table shows the properties that are required when you create the [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="2f2cc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f2cc-129">Property</span></span>|<span data-ttu-id="2f2cc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2f2cc-130">Type</span></span>|<span data-ttu-id="2f2cc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2f2cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f2cc-132">id</span><span class="sxs-lookup"><span data-stu-id="2f2cc-132">id</span></span>|<span data-ttu-id="2f2cc-133">String</span><span class="sxs-lookup"><span data-stu-id="2f2cc-133">String</span></span>|<span data-ttu-id="2f2cc-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="2f2cc-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f2cc-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="2f2cc-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f2cc-136">createdDateTime</span></span>|<span data-ttu-id="2f2cc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f2cc-137">DateTimeOffset</span></span>|<span data-ttu-id="2f2cc-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="2f2cc-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f2cc-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="2f2cc-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f2cc-140">lastModifiedDateTime</span></span>|<span data-ttu-id="2f2cc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f2cc-141">DateTimeOffset</span></span>|<span data-ttu-id="2f2cc-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="2f2cc-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f2cc-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="2f2cc-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="2f2cc-144">payloadId</span></span>|<span data-ttu-id="2f2cc-145">Строка</span><span class="sxs-lookup"><span data-stu-id="2f2cc-145">String</span></span>|<span data-ttu-id="2f2cc-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="2f2cc-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f2cc-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="2f2cc-148">itemType</span><span class="sxs-lookup"><span data-stu-id="2f2cc-148">itemType</span></span>|<span data-ttu-id="2f2cc-149">Строка</span><span class="sxs-lookup"><span data-stu-id="2f2cc-149">String</span></span>|<span data-ttu-id="2f2cc-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="2f2cc-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f2cc-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="2f2cc-152">displayName</span><span class="sxs-lookup"><span data-stu-id="2f2cc-152">displayName</span></span>|<span data-ttu-id="2f2cc-153">Строка</span><span class="sxs-lookup"><span data-stu-id="2f2cc-153">String</span></span>|<span data-ttu-id="2f2cc-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="2f2cc-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f2cc-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="2f2cc-156">status</span><span class="sxs-lookup"><span data-stu-id="2f2cc-156">status</span></span>|[<span data-ttu-id="2f2cc-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="2f2cc-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="2f2cc-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="2f2cc-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="2f2cc-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="2f2cc-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="2f2cc-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="2f2cc-161">errorCode</span></span>|[<span data-ttu-id="2f2cc-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="2f2cc-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="2f2cc-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="2f2cc-163">Error code if any occured.</span></span> <span data-ttu-id="2f2cc-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="2f2cc-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="2f2cc-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="2f2cc-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="2f2cc-166">guidedDeploymentTags</span></span>|<span data-ttu-id="2f2cc-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2f2cc-167">String collection</span></span>|<span data-ttu-id="2f2cc-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f2cc-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2f2cc-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f2cc-169">Response</span></span>
<span data-ttu-id="2f2cc-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-170">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f2cc-171">Пример</span><span class="sxs-lookup"><span data-stu-id="2f2cc-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f2cc-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f2cc-172">Request</span></span>
<span data-ttu-id="2f2cc-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f2cc-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f2cc-174">Response</span></span>
<span data-ttu-id="2f2cc-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f2cc-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





