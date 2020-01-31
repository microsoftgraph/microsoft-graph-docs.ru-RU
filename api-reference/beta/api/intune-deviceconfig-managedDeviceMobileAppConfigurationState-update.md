---
title: Обновление Манажеддевицемобилеаппконфигуратионстате
description: Обновление свойств объекта Манажеддевицемобилеаппконфигуратионстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43c22912df6f92418c98b4745567df542da1c78c
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636322"
---
# <a name="update-manageddevicemobileappconfigurationstate"></a><span data-ttu-id="688e8-103">Обновление Манажеддевицемобилеаппконфигуратионстате</span><span class="sxs-lookup"><span data-stu-id="688e8-103">Update managedDeviceMobileAppConfigurationState</span></span>

> <span data-ttu-id="688e8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="688e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="688e8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="688e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="688e8-106">Обновление свойств объекта Манажеддевицемобилеаппконфигуратионстате.</span><span class="sxs-lookup"><span data-stu-id="688e8-106">Update the properties of a managedDeviceMobileAppConfigurationState object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="688e8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="688e8-107">Prerequisites</span></span>
<span data-ttu-id="688e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="688e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="688e8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="688e8-110">Permission type</span></span>|<span data-ttu-id="688e8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="688e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="688e8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="688e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="688e8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="688e8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="688e8-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="688e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="688e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="688e8-115">Not supported.</span></span>|
|<span data-ttu-id="688e8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="688e8-116">Application</span></span>|<span data-ttu-id="688e8-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="688e8-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="688e8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="688e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates/{managedDeviceMobileAppConfigurationStateId}
```

## <a name="request-headers"></a><span data-ttu-id="688e8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="688e8-119">Request headers</span></span>
|<span data-ttu-id="688e8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="688e8-120">Header</span></span>|<span data-ttu-id="688e8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="688e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="688e8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="688e8-122">Authorization</span></span>|<span data-ttu-id="688e8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="688e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="688e8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="688e8-124">Accept</span></span>|<span data-ttu-id="688e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="688e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="688e8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="688e8-126">Request body</span></span>
<span data-ttu-id="688e8-127">В тексте запроса добавьте представление объекта Манажеддевицемобилеаппконфигуратионстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="688e8-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationState object.</span></span>

<span data-ttu-id="688e8-128">В следующей таблице приведены свойства, необходимые при создании Манажеддевицемобилеаппконфигуратионстате.</span><span class="sxs-lookup"><span data-stu-id="688e8-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationState.</span></span>

|<span data-ttu-id="688e8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="688e8-129">Property</span></span>|<span data-ttu-id="688e8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="688e8-130">Type</span></span>|<span data-ttu-id="688e8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="688e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="688e8-132">id</span><span class="sxs-lookup"><span data-stu-id="688e8-132">id</span></span>|<span data-ttu-id="688e8-133">String</span><span class="sxs-lookup"><span data-stu-id="688e8-133">String</span></span>|<span data-ttu-id="688e8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="688e8-134">Key of the entity.</span></span>|
|<span data-ttu-id="688e8-135">settingStates</span><span class="sxs-lookup"><span data-stu-id="688e8-135">settingStates</span></span>|<span data-ttu-id="688e8-136">Коллекция Манажеддевицемобилеаппконфигуратионсеттингстате</span><span class="sxs-lookup"><span data-stu-id="688e8-136">managedDeviceMobileAppConfigurationSettingState collection</span></span>|<span data-ttu-id="688e8-137">**TODO: Добавление описания.**</span><span class="sxs-lookup"><span data-stu-id="688e8-137">**TODO: Add description.**</span></span>|
|<span data-ttu-id="688e8-138">displayName</span><span class="sxs-lookup"><span data-stu-id="688e8-138">displayName</span></span>|<span data-ttu-id="688e8-139">Строка</span><span class="sxs-lookup"><span data-stu-id="688e8-139">String</span></span>|<span data-ttu-id="688e8-140">Имя политики для policyBase.</span><span class="sxs-lookup"><span data-stu-id="688e8-140">The name of the policy for this policyBase</span></span>|
|<span data-ttu-id="688e8-141">version</span><span class="sxs-lookup"><span data-stu-id="688e8-141">version</span></span>|<span data-ttu-id="688e8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="688e8-142">Int32</span></span>|<span data-ttu-id="688e8-143">Версия политики.</span><span class="sxs-lookup"><span data-stu-id="688e8-143">The version of the policy</span></span>|
|<span data-ttu-id="688e8-144">platformType</span><span class="sxs-lookup"><span data-stu-id="688e8-144">platformType</span></span>|<span data-ttu-id="688e8-145">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="688e8-145">policyPlatformType</span></span>|<span data-ttu-id="688e8-146">Тип платформы, к которой применяется политика.</span><span class="sxs-lookup"><span data-stu-id="688e8-146">Platform type that the policy applies to.</span></span> <span data-ttu-id="688e8-147">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="688e8-147">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="688e8-148">state</span><span class="sxs-lookup"><span data-stu-id="688e8-148">state</span></span>|<span data-ttu-id="688e8-149">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="688e8-149">complianceStatus</span></span>|<span data-ttu-id="688e8-150">Состояние соответствия политике.</span><span class="sxs-lookup"><span data-stu-id="688e8-150">The compliance state of the policy.</span></span> <span data-ttu-id="688e8-151">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="688e8-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="688e8-152">settingCount</span><span class="sxs-lookup"><span data-stu-id="688e8-152">settingCount</span></span>|<span data-ttu-id="688e8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="688e8-153">Int32</span></span>|<span data-ttu-id="688e8-154">Количество параметров в политике.</span><span class="sxs-lookup"><span data-stu-id="688e8-154">Count of how many setting a policy holds</span></span>|
|<span data-ttu-id="688e8-155">userId</span><span class="sxs-lookup"><span data-stu-id="688e8-155">userId</span></span>|<span data-ttu-id="688e8-156">String</span><span class="sxs-lookup"><span data-stu-id="688e8-156">String</span></span>|<span data-ttu-id="688e8-157">Уникальный идентификатор пользователя, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="688e8-157">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="688e8-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="688e8-158">userPrincipalName</span></span>|<span data-ttu-id="688e8-159">String</span><span class="sxs-lookup"><span data-stu-id="688e8-159">String</span></span>|<span data-ttu-id="688e8-160">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="688e8-160">User Principal Name</span></span>|



## <a name="response"></a><span data-ttu-id="688e8-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="688e8-161">Response</span></span>
<span data-ttu-id="688e8-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект манажеддевицемобилеаппконфигуратионстате в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="688e8-162">If successful, this method returns a `200 OK` response code and an updated managedDeviceMobileAppConfigurationState object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="688e8-163">Пример</span><span class="sxs-lookup"><span data-stu-id="688e8-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="688e8-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="688e8-164">Request</span></span>
<span data-ttu-id="688e8-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="688e8-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates/{managedDeviceMobileAppConfigurationStateId}
Content-type: application/json
Content-length: 1093

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "androidForWork",
  "state": "notApplicable",
  "settingCount": 12,
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="688e8-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="688e8-166">Response</span></span>
<span data-ttu-id="688e8-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="688e8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1142

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "id": "659554f2-54f2-6595-f254-9565f2549565",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "androidForWork",
  "state": "notApplicable",
  "settingCount": 12,
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value"
}
```



