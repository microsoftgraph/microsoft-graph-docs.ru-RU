---
title: Обновление aospDeviceOwnerCompliancePolicy
description: Обновление свойств объекта aospDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7a90ab0d19a6dba44a42b653556c71b01e2011c
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666019"
---
# <a name="update-aospdeviceownercompliancepolicy"></a><span data-ttu-id="a7f1a-103">Обновление aospDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a7f1a-103">Update aospDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="a7f1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7f1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7f1a-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7f1a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7f1a-107">Обновление свойств объекта [aospDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a7f1a-107">Update the properties of a [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7f1a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a7f1a-108">Prerequisites</span></span>
<span data-ttu-id="a7f1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7f1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7f1a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7f1a-111">Permission type</span></span>|<span data-ttu-id="a7f1a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7f1a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7f1a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7f1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7f1a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7f1a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7f1a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7f1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7f1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-116">Not supported.</span></span>|
|<span data-ttu-id="a7f1a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a7f1a-117">Application</span></span>|<span data-ttu-id="a7f1a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7f1a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7f1a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7f1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a7f1a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a7f1a-120">Request headers</span></span>
|<span data-ttu-id="a7f1a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7f1a-121">Header</span></span>|<span data-ttu-id="a7f1a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a7f1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7f1a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7f1a-123">Authorization</span></span>|<span data-ttu-id="a7f1a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7f1a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7f1a-125">Accept</span></span>|<span data-ttu-id="a7f1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7f1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7f1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7f1a-127">Request body</span></span>
<span data-ttu-id="a7f1a-128">В теле запроса поставляем представление JSON для [объекта aospDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a7f1a-128">In the request body, supply a JSON representation for the [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="a7f1a-129">В следующей таблице показаны свойства, необходимые при создании [aospDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a7f1a-129">The following table shows the properties that are required when you create the [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="a7f1a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7f1a-130">Property</span></span>|<span data-ttu-id="a7f1a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a7f1a-131">Type</span></span>|<span data-ttu-id="a7f1a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a7f1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7f1a-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a7f1a-133">roleScopeTagIds</span></span>|<span data-ttu-id="a7f1a-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a7f1a-134">String collection</span></span>|<span data-ttu-id="a7f1a-135">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a7f1a-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a7f1a-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a7f1a-137">id</span><span class="sxs-lookup"><span data-stu-id="a7f1a-137">id</span></span>|<span data-ttu-id="a7f1a-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a7f1a-138">String</span></span>|<span data-ttu-id="a7f1a-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-139">Key of the entity.</span></span> <span data-ttu-id="a7f1a-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a7f1a-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a7f1a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7f1a-141">createdDateTime</span></span>|<span data-ttu-id="a7f1a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7f1a-142">DateTimeOffset</span></span>|<span data-ttu-id="a7f1a-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-143">DateTime the object was created.</span></span> <span data-ttu-id="a7f1a-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a7f1a-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a7f1a-145">description</span><span class="sxs-lookup"><span data-stu-id="a7f1a-145">description</span></span>|<span data-ttu-id="a7f1a-146">Строка</span><span class="sxs-lookup"><span data-stu-id="a7f1a-146">String</span></span>|<span data-ttu-id="a7f1a-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a7f1a-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a7f1a-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a7f1a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7f1a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="a7f1a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7f1a-150">DateTimeOffset</span></span>|<span data-ttu-id="a7f1a-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-151">DateTime the object was last modified.</span></span> <span data-ttu-id="a7f1a-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a7f1a-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a7f1a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="a7f1a-153">displayName</span></span>|<span data-ttu-id="a7f1a-154">Строка</span><span class="sxs-lookup"><span data-stu-id="a7f1a-154">String</span></span>|<span data-ttu-id="a7f1a-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a7f1a-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a7f1a-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a7f1a-157">version</span><span class="sxs-lookup"><span data-stu-id="a7f1a-157">version</span></span>|<span data-ttu-id="a7f1a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a7f1a-158">Int32</span></span>|<span data-ttu-id="a7f1a-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-159">Version of the device configuration.</span></span> <span data-ttu-id="a7f1a-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a7f1a-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a7f1a-161">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a7f1a-161">osMinimumVersion</span></span>|<span data-ttu-id="a7f1a-162">String</span><span class="sxs-lookup"><span data-stu-id="a7f1a-162">String</span></span>|<span data-ttu-id="a7f1a-163">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-163">Minimum Android version.</span></span>|
|<span data-ttu-id="a7f1a-164">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a7f1a-164">osMaximumVersion</span></span>|<span data-ttu-id="a7f1a-165">String</span><span class="sxs-lookup"><span data-stu-id="a7f1a-165">String</span></span>|<span data-ttu-id="a7f1a-166">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-166">Maximum Android version.</span></span>|
|<span data-ttu-id="a7f1a-167">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="a7f1a-167">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="a7f1a-168">String</span><span class="sxs-lookup"><span data-stu-id="a7f1a-168">String</span></span>|<span data-ttu-id="a7f1a-169">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-169">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="a7f1a-170">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a7f1a-170">passwordRequired</span></span>|<span data-ttu-id="a7f1a-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7f1a-171">Boolean</span></span>|<span data-ttu-id="a7f1a-172">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-172">Require a password to unlock device.</span></span>|
|<span data-ttu-id="a7f1a-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a7f1a-173">passwordRequiredType</span></span>|[<span data-ttu-id="a7f1a-174">AndroidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a7f1a-174">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="a7f1a-175">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-175">Type of characters in password.</span></span> <span data-ttu-id="a7f1a-176">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-176">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="a7f1a-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a7f1a-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a7f1a-178">Int32</span><span class="sxs-lookup"><span data-stu-id="a7f1a-178">Int32</span></span>|<span data-ttu-id="a7f1a-179">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-179">Minutes of inactivity before a password is required.</span></span> <span data-ttu-id="a7f1a-180">Допустимые значения от 1 до 8640</span><span class="sxs-lookup"><span data-stu-id="a7f1a-180">Valid values 1 to 8640</span></span>|
|<span data-ttu-id="a7f1a-181">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a7f1a-181">passwordMinimumLength</span></span>|<span data-ttu-id="a7f1a-182">Int32</span><span class="sxs-lookup"><span data-stu-id="a7f1a-182">Int32</span></span>|<span data-ttu-id="a7f1a-183">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-183">Minimum password length.</span></span> <span data-ttu-id="a7f1a-184">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-184">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a7f1a-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="a7f1a-185">storageRequireEncryption</span></span>|<span data-ttu-id="a7f1a-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7f1a-186">Boolean</span></span>|<span data-ttu-id="a7f1a-187">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-187">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="a7f1a-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7f1a-188">Response</span></span>
<span data-ttu-id="a7f1a-189">В случае успешного использования этот метод возвращает код ответа и обновленный `200 OK` [объект aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-189">If successful, this method returns a `200 OK` response code and an updated [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7f1a-190">Пример</span><span class="sxs-lookup"><span data-stu-id="a7f1a-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7f1a-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7f1a-191">Request</span></span>
<span data-ttu-id="a7f1a-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 593

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumLength": 5,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="a7f1a-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7f1a-193">Response</span></span>
<span data-ttu-id="a7f1a-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7f1a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 765

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "0837b942-b942-0837-42b9-370842b93708",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumLength": 5,
  "storageRequireEncryption": true
}
```




