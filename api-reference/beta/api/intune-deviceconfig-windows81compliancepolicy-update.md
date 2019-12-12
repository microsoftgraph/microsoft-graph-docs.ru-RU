---
title: Update windows81CompliancePolicy
description: Обновление свойств объекта windows81CompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5cc97cd2e6ccc4d15f836baf1e6af19f89ab0b3a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947094"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="e31fc-103">Update windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e31fc-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="e31fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e31fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e31fc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e31fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e31fc-106">Обновление свойств объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e31fc-106">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e31fc-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e31fc-107">Prerequisites</span></span>
<span data-ttu-id="e31fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e31fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e31fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e31fc-110">Permission type</span></span>|<span data-ttu-id="e31fc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e31fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e31fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e31fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e31fc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e31fc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e31fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e31fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e31fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e31fc-115">Not supported.</span></span>|
|<span data-ttu-id="e31fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e31fc-116">Application</span></span>|<span data-ttu-id="e31fc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e31fc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e31fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e31fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="e31fc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e31fc-119">Request headers</span></span>
|<span data-ttu-id="e31fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e31fc-120">Header</span></span>|<span data-ttu-id="e31fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e31fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e31fc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e31fc-122">Authorization</span></span>|<span data-ttu-id="e31fc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e31fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e31fc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e31fc-124">Accept</span></span>|<span data-ttu-id="e31fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e31fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e31fc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e31fc-126">Request body</span></span>
<span data-ttu-id="e31fc-127">В теле запроса добавьте представление объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e31fc-127">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="e31fc-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e31fc-128">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="e31fc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e31fc-129">Property</span></span>|<span data-ttu-id="e31fc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e31fc-130">Type</span></span>|<span data-ttu-id="e31fc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e31fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e31fc-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e31fc-132">roleScopeTagIds</span></span>|<span data-ttu-id="e31fc-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e31fc-133">String collection</span></span>|<span data-ttu-id="e31fc-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e31fc-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e31fc-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e31fc-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e31fc-136">id</span><span class="sxs-lookup"><span data-stu-id="e31fc-136">id</span></span>|<span data-ttu-id="e31fc-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e31fc-137">String</span></span>|<span data-ttu-id="e31fc-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e31fc-138">Key of the entity.</span></span> <span data-ttu-id="e31fc-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e31fc-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e31fc-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e31fc-140">createdDateTime</span></span>|<span data-ttu-id="e31fc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e31fc-141">DateTimeOffset</span></span>|<span data-ttu-id="e31fc-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e31fc-142">DateTime the object was created.</span></span> <span data-ttu-id="e31fc-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e31fc-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e31fc-144">description</span><span class="sxs-lookup"><span data-stu-id="e31fc-144">description</span></span>|<span data-ttu-id="e31fc-145">String</span><span class="sxs-lookup"><span data-stu-id="e31fc-145">String</span></span>|<span data-ttu-id="e31fc-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e31fc-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e31fc-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e31fc-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e31fc-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e31fc-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e31fc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e31fc-149">DateTimeOffset</span></span>|<span data-ttu-id="e31fc-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e31fc-150">DateTime the object was last modified.</span></span> <span data-ttu-id="e31fc-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e31fc-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e31fc-152">displayName</span><span class="sxs-lookup"><span data-stu-id="e31fc-152">displayName</span></span>|<span data-ttu-id="e31fc-153">Строка</span><span class="sxs-lookup"><span data-stu-id="e31fc-153">String</span></span>|<span data-ttu-id="e31fc-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e31fc-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e31fc-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e31fc-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e31fc-156">version</span><span class="sxs-lookup"><span data-stu-id="e31fc-156">version</span></span>|<span data-ttu-id="e31fc-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e31fc-157">Int32</span></span>|<span data-ttu-id="e31fc-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e31fc-158">Version of the device configuration.</span></span> <span data-ttu-id="e31fc-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e31fc-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e31fc-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e31fc-160">passwordRequired</span></span>|<span data-ttu-id="e31fc-161">Логический</span><span class="sxs-lookup"><span data-stu-id="e31fc-161">Boolean</span></span>|<span data-ttu-id="e31fc-162">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="e31fc-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="e31fc-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e31fc-163">passwordBlockSimple</span></span>|<span data-ttu-id="e31fc-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="e31fc-164">Boolean</span></span>|<span data-ttu-id="e31fc-165">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="e31fc-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="e31fc-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e31fc-166">passwordExpirationDays</span></span>|<span data-ttu-id="e31fc-167">Int32</span><span class="sxs-lookup"><span data-stu-id="e31fc-167">Int32</span></span>|<span data-ttu-id="e31fc-168">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="e31fc-168">Password expiration in days.</span></span>|
|<span data-ttu-id="e31fc-169">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e31fc-169">passwordMinimumLength</span></span>|<span data-ttu-id="e31fc-170">Int32</span><span class="sxs-lookup"><span data-stu-id="e31fc-170">Int32</span></span>|<span data-ttu-id="e31fc-171">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="e31fc-171">The minimum password length.</span></span>|
|<span data-ttu-id="e31fc-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e31fc-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e31fc-173">Int32</span><span class="sxs-lookup"><span data-stu-id="e31fc-173">Int32</span></span>|<span data-ttu-id="e31fc-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="e31fc-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e31fc-175">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e31fc-175">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e31fc-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e31fc-176">Int32</span></span>|<span data-ttu-id="e31fc-177">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="e31fc-177">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e31fc-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e31fc-178">passwordRequiredType</span></span>|[<span data-ttu-id="e31fc-179">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="e31fc-179">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e31fc-180">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="e31fc-180">The required password type.</span></span> <span data-ttu-id="e31fc-181">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e31fc-181">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e31fc-182">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e31fc-182">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e31fc-183">Int32</span><span class="sxs-lookup"><span data-stu-id="e31fc-183">Int32</span></span>|<span data-ttu-id="e31fc-184">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="e31fc-184">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="e31fc-185">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="e31fc-185">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e31fc-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e31fc-186">osMinimumVersion</span></span>|<span data-ttu-id="e31fc-187">Строка</span><span class="sxs-lookup"><span data-stu-id="e31fc-187">String</span></span>|<span data-ttu-id="e31fc-188">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="e31fc-188">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="e31fc-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e31fc-189">osMaximumVersion</span></span>|<span data-ttu-id="e31fc-190">String</span><span class="sxs-lookup"><span data-stu-id="e31fc-190">String</span></span>|<span data-ttu-id="e31fc-191">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="e31fc-191">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="e31fc-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e31fc-192">storageRequireEncryption</span></span>|<span data-ttu-id="e31fc-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="e31fc-193">Boolean</span></span>|<span data-ttu-id="e31fc-194">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="e31fc-194">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="e31fc-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="e31fc-195">Response</span></span>
<span data-ttu-id="e31fc-196">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e31fc-196">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e31fc-197">Пример</span><span class="sxs-lookup"><span data-stu-id="e31fc-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="e31fc-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="e31fc-198">Request</span></span>
<span data-ttu-id="e31fc-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e31fc-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e31fc-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="e31fc-200">Response</span></span>
<span data-ttu-id="e31fc-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e31fc-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





