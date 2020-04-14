---
title: Update windows81CompliancePolicy
description: Обновление свойств объекта windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c46a5f12320f8e6eea80fda6dff54a2b8fb6e44b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43430516"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="98cdc-103">Update windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="98cdc-103">Update windows81CompliancePolicy</span></span>

<span data-ttu-id="98cdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98cdc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98cdc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98cdc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98cdc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98cdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98cdc-107">Обновление свойств объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98cdc-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98cdc-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="98cdc-108">Prerequisites</span></span>
<span data-ttu-id="98cdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98cdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98cdc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98cdc-111">Permission type</span></span>|<span data-ttu-id="98cdc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98cdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98cdc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98cdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98cdc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98cdc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98cdc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98cdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98cdc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98cdc-116">Not supported.</span></span>|
|<span data-ttu-id="98cdc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="98cdc-117">Application</span></span>|<span data-ttu-id="98cdc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98cdc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98cdc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98cdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="98cdc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="98cdc-120">Request headers</span></span>
|<span data-ttu-id="98cdc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98cdc-121">Header</span></span>|<span data-ttu-id="98cdc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="98cdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98cdc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98cdc-123">Authorization</span></span>|<span data-ttu-id="98cdc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98cdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98cdc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98cdc-125">Accept</span></span>|<span data-ttu-id="98cdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98cdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98cdc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98cdc-127">Request body</span></span>
<span data-ttu-id="98cdc-128">В теле запроса добавьте представление объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98cdc-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="98cdc-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98cdc-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="98cdc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="98cdc-130">Property</span></span>|<span data-ttu-id="98cdc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="98cdc-131">Type</span></span>|<span data-ttu-id="98cdc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="98cdc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98cdc-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="98cdc-133">roleScopeTagIds</span></span>|<span data-ttu-id="98cdc-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="98cdc-134">String collection</span></span>|<span data-ttu-id="98cdc-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="98cdc-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="98cdc-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98cdc-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="98cdc-137">id</span><span class="sxs-lookup"><span data-stu-id="98cdc-137">id</span></span>|<span data-ttu-id="98cdc-138">Строка</span><span class="sxs-lookup"><span data-stu-id="98cdc-138">String</span></span>|<span data-ttu-id="98cdc-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="98cdc-139">Key of the entity.</span></span> <span data-ttu-id="98cdc-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98cdc-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="98cdc-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98cdc-141">createdDateTime</span></span>|<span data-ttu-id="98cdc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98cdc-142">DateTimeOffset</span></span>|<span data-ttu-id="98cdc-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="98cdc-143">DateTime the object was created.</span></span> <span data-ttu-id="98cdc-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98cdc-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="98cdc-145">description</span><span class="sxs-lookup"><span data-stu-id="98cdc-145">description</span></span>|<span data-ttu-id="98cdc-146">String</span><span class="sxs-lookup"><span data-stu-id="98cdc-146">String</span></span>|<span data-ttu-id="98cdc-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="98cdc-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="98cdc-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98cdc-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="98cdc-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98cdc-149">lastModifiedDateTime</span></span>|<span data-ttu-id="98cdc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98cdc-150">DateTimeOffset</span></span>|<span data-ttu-id="98cdc-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="98cdc-151">DateTime the object was last modified.</span></span> <span data-ttu-id="98cdc-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98cdc-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="98cdc-153">displayName</span><span class="sxs-lookup"><span data-stu-id="98cdc-153">displayName</span></span>|<span data-ttu-id="98cdc-154">Строка</span><span class="sxs-lookup"><span data-stu-id="98cdc-154">String</span></span>|<span data-ttu-id="98cdc-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="98cdc-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="98cdc-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98cdc-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="98cdc-157">version</span><span class="sxs-lookup"><span data-stu-id="98cdc-157">version</span></span>|<span data-ttu-id="98cdc-158">Int32</span><span class="sxs-lookup"><span data-stu-id="98cdc-158">Int32</span></span>|<span data-ttu-id="98cdc-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="98cdc-159">Version of the device configuration.</span></span> <span data-ttu-id="98cdc-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98cdc-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="98cdc-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="98cdc-161">passwordRequired</span></span>|<span data-ttu-id="98cdc-162">Логический</span><span class="sxs-lookup"><span data-stu-id="98cdc-162">Boolean</span></span>|<span data-ttu-id="98cdc-163">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="98cdc-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="98cdc-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="98cdc-164">passwordBlockSimple</span></span>|<span data-ttu-id="98cdc-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="98cdc-165">Boolean</span></span>|<span data-ttu-id="98cdc-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="98cdc-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="98cdc-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="98cdc-167">passwordExpirationDays</span></span>|<span data-ttu-id="98cdc-168">Int32</span><span class="sxs-lookup"><span data-stu-id="98cdc-168">Int32</span></span>|<span data-ttu-id="98cdc-169">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="98cdc-169">Password expiration in days.</span></span>|
|<span data-ttu-id="98cdc-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="98cdc-170">passwordMinimumLength</span></span>|<span data-ttu-id="98cdc-171">Int32</span><span class="sxs-lookup"><span data-stu-id="98cdc-171">Int32</span></span>|<span data-ttu-id="98cdc-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="98cdc-172">The minimum password length.</span></span>|
|<span data-ttu-id="98cdc-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="98cdc-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="98cdc-174">Int32</span><span class="sxs-lookup"><span data-stu-id="98cdc-174">Int32</span></span>|<span data-ttu-id="98cdc-175">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="98cdc-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="98cdc-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="98cdc-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="98cdc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="98cdc-177">Int32</span></span>|<span data-ttu-id="98cdc-178">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="98cdc-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="98cdc-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="98cdc-179">passwordRequiredType</span></span>|[<span data-ttu-id="98cdc-180">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="98cdc-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="98cdc-181">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="98cdc-181">The required password type.</span></span> <span data-ttu-id="98cdc-182">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="98cdc-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="98cdc-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="98cdc-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="98cdc-184">Int32</span><span class="sxs-lookup"><span data-stu-id="98cdc-184">Int32</span></span>|<span data-ttu-id="98cdc-185">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="98cdc-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="98cdc-186">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="98cdc-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="98cdc-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="98cdc-187">osMinimumVersion</span></span>|<span data-ttu-id="98cdc-188">String</span><span class="sxs-lookup"><span data-stu-id="98cdc-188">String</span></span>|<span data-ttu-id="98cdc-189">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="98cdc-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="98cdc-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="98cdc-190">osMaximumVersion</span></span>|<span data-ttu-id="98cdc-191">String</span><span class="sxs-lookup"><span data-stu-id="98cdc-191">String</span></span>|<span data-ttu-id="98cdc-192">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="98cdc-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="98cdc-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="98cdc-193">storageRequireEncryption</span></span>|<span data-ttu-id="98cdc-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="98cdc-194">Boolean</span></span>|<span data-ttu-id="98cdc-195">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="98cdc-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="98cdc-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="98cdc-196">Response</span></span>
<span data-ttu-id="98cdc-197">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="98cdc-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98cdc-198">Пример</span><span class="sxs-lookup"><span data-stu-id="98cdc-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="98cdc-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="98cdc-199">Request</span></span>
<span data-ttu-id="98cdc-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98cdc-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="98cdc-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="98cdc-201">Response</span></span>
<span data-ttu-id="98cdc-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98cdc-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



