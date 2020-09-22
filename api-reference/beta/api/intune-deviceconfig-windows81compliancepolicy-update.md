---
title: Update windows81CompliancePolicy
description: Обновление свойств объекта windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8d0462f98432d8cf6475e4962d16cf1fc6a8877c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48005399"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="1f813-103">Update windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="1f813-103">Update windows81CompliancePolicy</span></span>

<span data-ttu-id="1f813-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f813-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f813-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f813-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f813-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f813-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f813-107">Обновление свойств объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f813-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f813-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1f813-108">Prerequisites</span></span>
<span data-ttu-id="1f813-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f813-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f813-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f813-111">Permission type</span></span>|<span data-ttu-id="1f813-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f813-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f813-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f813-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f813-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f813-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f813-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f813-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f813-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f813-116">Not supported.</span></span>|
|<span data-ttu-id="1f813-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f813-117">Application</span></span>|<span data-ttu-id="1f813-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f813-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f813-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f813-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="1f813-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1f813-120">Request headers</span></span>
|<span data-ttu-id="1f813-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f813-121">Header</span></span>|<span data-ttu-id="1f813-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1f813-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f813-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f813-123">Authorization</span></span>|<span data-ttu-id="1f813-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f813-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f813-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f813-125">Accept</span></span>|<span data-ttu-id="1f813-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f813-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f813-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f813-127">Request body</span></span>
<span data-ttu-id="1f813-128">В теле запроса добавьте представление объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f813-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="1f813-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f813-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="1f813-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f813-130">Property</span></span>|<span data-ttu-id="1f813-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1f813-131">Type</span></span>|<span data-ttu-id="1f813-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1f813-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f813-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1f813-133">roleScopeTagIds</span></span>|<span data-ttu-id="1f813-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1f813-134">String collection</span></span>|<span data-ttu-id="1f813-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1f813-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1f813-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f813-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1f813-137">id</span><span class="sxs-lookup"><span data-stu-id="1f813-137">id</span></span>|<span data-ttu-id="1f813-138">String</span><span class="sxs-lookup"><span data-stu-id="1f813-138">String</span></span>|<span data-ttu-id="1f813-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1f813-139">Key of the entity.</span></span> <span data-ttu-id="1f813-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f813-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1f813-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f813-141">createdDateTime</span></span>|<span data-ttu-id="1f813-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f813-142">DateTimeOffset</span></span>|<span data-ttu-id="1f813-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1f813-143">DateTime the object was created.</span></span> <span data-ttu-id="1f813-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f813-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1f813-145">description</span><span class="sxs-lookup"><span data-stu-id="1f813-145">description</span></span>|<span data-ttu-id="1f813-146">String</span><span class="sxs-lookup"><span data-stu-id="1f813-146">String</span></span>|<span data-ttu-id="1f813-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f813-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1f813-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f813-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1f813-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f813-149">lastModifiedDateTime</span></span>|<span data-ttu-id="1f813-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f813-150">DateTimeOffset</span></span>|<span data-ttu-id="1f813-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1f813-151">DateTime the object was last modified.</span></span> <span data-ttu-id="1f813-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f813-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1f813-153">displayName</span><span class="sxs-lookup"><span data-stu-id="1f813-153">displayName</span></span>|<span data-ttu-id="1f813-154">String</span><span class="sxs-lookup"><span data-stu-id="1f813-154">String</span></span>|<span data-ttu-id="1f813-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f813-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1f813-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f813-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1f813-157">version</span><span class="sxs-lookup"><span data-stu-id="1f813-157">version</span></span>|<span data-ttu-id="1f813-158">Int32</span><span class="sxs-lookup"><span data-stu-id="1f813-158">Int32</span></span>|<span data-ttu-id="1f813-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f813-159">Version of the device configuration.</span></span> <span data-ttu-id="1f813-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f813-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1f813-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1f813-161">passwordRequired</span></span>|<span data-ttu-id="1f813-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f813-162">Boolean</span></span>|<span data-ttu-id="1f813-163">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="1f813-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="1f813-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1f813-164">passwordBlockSimple</span></span>|<span data-ttu-id="1f813-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f813-165">Boolean</span></span>|<span data-ttu-id="1f813-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="1f813-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="1f813-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1f813-167">passwordExpirationDays</span></span>|<span data-ttu-id="1f813-168">Int32</span><span class="sxs-lookup"><span data-stu-id="1f813-168">Int32</span></span>|<span data-ttu-id="1f813-169">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="1f813-169">Password expiration in days.</span></span>|
|<span data-ttu-id="1f813-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1f813-170">passwordMinimumLength</span></span>|<span data-ttu-id="1f813-171">Int32</span><span class="sxs-lookup"><span data-stu-id="1f813-171">Int32</span></span>|<span data-ttu-id="1f813-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="1f813-172">The minimum password length.</span></span>|
|<span data-ttu-id="1f813-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1f813-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1f813-174">Int32</span><span class="sxs-lookup"><span data-stu-id="1f813-174">Int32</span></span>|<span data-ttu-id="1f813-175">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="1f813-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="1f813-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1f813-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="1f813-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1f813-177">Int32</span></span>|<span data-ttu-id="1f813-178">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="1f813-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="1f813-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1f813-179">passwordRequiredType</span></span>|[<span data-ttu-id="1f813-180">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="1f813-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="1f813-181">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="1f813-181">The required password type.</span></span> <span data-ttu-id="1f813-182">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="1f813-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="1f813-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1f813-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1f813-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1f813-184">Int32</span></span>|<span data-ttu-id="1f813-185">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="1f813-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="1f813-186">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="1f813-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1f813-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1f813-187">osMinimumVersion</span></span>|<span data-ttu-id="1f813-188">String</span><span class="sxs-lookup"><span data-stu-id="1f813-188">String</span></span>|<span data-ttu-id="1f813-189">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="1f813-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="1f813-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1f813-190">osMaximumVersion</span></span>|<span data-ttu-id="1f813-191">String</span><span class="sxs-lookup"><span data-stu-id="1f813-191">String</span></span>|<span data-ttu-id="1f813-192">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="1f813-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="1f813-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="1f813-193">storageRequireEncryption</span></span>|<span data-ttu-id="1f813-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f813-194">Boolean</span></span>|<span data-ttu-id="1f813-195">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="1f813-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="1f813-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f813-196">Response</span></span>
<span data-ttu-id="1f813-197">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1f813-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f813-198">Пример</span><span class="sxs-lookup"><span data-stu-id="1f813-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f813-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f813-199">Request</span></span>
<span data-ttu-id="1f813-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f813-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 664

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="1f813-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f813-201">Response</span></span>
<span data-ttu-id="1f813-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f813-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 836

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```






