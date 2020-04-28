---
title: Создание Таржетедманажедаппконфигуратионполицисетитем
description: Создание нового объекта Таржетедманажедаппконфигуратионполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 159c764f5536e08af0f9610b4b307890139e5e47
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383636"
---
# <a name="create-targetedmanagedappconfigurationpolicysetitem"></a><span data-ttu-id="0ba78-103">Создание Таржетедманажедаппконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="0ba78-103">Create targetedManagedAppConfigurationPolicySetItem</span></span>

<span data-ttu-id="0ba78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ba78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ba78-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ba78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ba78-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ba78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ba78-107">Создание нового объекта [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="0ba78-107">Create a new [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ba78-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0ba78-108">Prerequisites</span></span>
<span data-ttu-id="0ba78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ba78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ba78-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ba78-111">Permission type</span></span>|<span data-ttu-id="0ba78-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ba78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ba78-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ba78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ba78-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ba78-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ba78-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ba78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ba78-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ba78-116">Not supported.</span></span>|
|<span data-ttu-id="0ba78-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ba78-117">Application</span></span>|<span data-ttu-id="0ba78-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ba78-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ba78-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ba78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="0ba78-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0ba78-120">Request headers</span></span>
|<span data-ttu-id="0ba78-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ba78-121">Header</span></span>|<span data-ttu-id="0ba78-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0ba78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ba78-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ba78-123">Authorization</span></span>|<span data-ttu-id="0ba78-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ba78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ba78-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ba78-125">Accept</span></span>|<span data-ttu-id="0ba78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ba78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ba78-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ba78-127">Request body</span></span>
<span data-ttu-id="0ba78-128">В тексте запроса добавьте представление объекта Таржетедманажедаппконфигуратионполицисетитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ba78-128">In the request body, supply a JSON representation for the targetedManagedAppConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="0ba78-129">В следующей таблице приведены свойства, необходимые при создании Таржетедманажедаппконфигуратионполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="0ba78-129">The following table shows the properties that are required when you create the targetedManagedAppConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="0ba78-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ba78-130">Property</span></span>|<span data-ttu-id="0ba78-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0ba78-131">Type</span></span>|<span data-ttu-id="0ba78-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0ba78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ba78-133">id</span><span class="sxs-lookup"><span data-stu-id="0ba78-133">id</span></span>|<span data-ttu-id="0ba78-134">String</span><span class="sxs-lookup"><span data-stu-id="0ba78-134">String</span></span>|<span data-ttu-id="0ba78-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="0ba78-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="0ba78-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ba78-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0ba78-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ba78-137">createdDateTime</span></span>|<span data-ttu-id="0ba78-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ba78-138">DateTimeOffset</span></span>|<span data-ttu-id="0ba78-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="0ba78-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="0ba78-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ba78-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0ba78-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ba78-141">lastModifiedDateTime</span></span>|<span data-ttu-id="0ba78-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ba78-142">DateTimeOffset</span></span>|<span data-ttu-id="0ba78-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="0ba78-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="0ba78-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ba78-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0ba78-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="0ba78-145">payloadId</span></span>|<span data-ttu-id="0ba78-146">String</span><span class="sxs-lookup"><span data-stu-id="0ba78-146">String</span></span>|<span data-ttu-id="0ba78-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="0ba78-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="0ba78-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ba78-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0ba78-149">itemType</span><span class="sxs-lookup"><span data-stu-id="0ba78-149">itemType</span></span>|<span data-ttu-id="0ba78-150">String</span><span class="sxs-lookup"><span data-stu-id="0ba78-150">String</span></span>|<span data-ttu-id="0ba78-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="0ba78-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="0ba78-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ba78-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0ba78-153">displayName</span><span class="sxs-lookup"><span data-stu-id="0ba78-153">displayName</span></span>|<span data-ttu-id="0ba78-154">Строка</span><span class="sxs-lookup"><span data-stu-id="0ba78-154">String</span></span>|<span data-ttu-id="0ba78-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="0ba78-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="0ba78-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ba78-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="0ba78-157">status</span><span class="sxs-lookup"><span data-stu-id="0ba78-157">status</span></span>|[<span data-ttu-id="0ba78-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="0ba78-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="0ba78-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="0ba78-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="0ba78-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="0ba78-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="0ba78-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="0ba78-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="0ba78-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="0ba78-162">errorCode</span></span>|[<span data-ttu-id="0ba78-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="0ba78-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="0ba78-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="0ba78-164">Error code if any occured.</span></span> <span data-ttu-id="0ba78-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="0ba78-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="0ba78-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="0ba78-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="0ba78-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="0ba78-167">guidedDeploymentTags</span></span>|<span data-ttu-id="0ba78-168">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="0ba78-168">String collection</span></span>|<span data-ttu-id="0ba78-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ba78-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0ba78-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ba78-170">Response</span></span>
<span data-ttu-id="0ba78-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ba78-171">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ba78-172">Пример</span><span class="sxs-lookup"><span data-stu-id="0ba78-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ba78-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ba78-173">Request</span></span>
<span data-ttu-id="0ba78-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ba78-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
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

### <a name="response"></a><span data-ttu-id="0ba78-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ba78-175">Response</span></span>
<span data-ttu-id="0ba78-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ba78-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



