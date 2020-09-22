---
title: Создание объекта windows81CompliancePolicy
description: Создание объекта windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a6acd0c531cc4f580f873939acf929db2f764ccc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48005420"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="5436c-103">Создание объекта windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5436c-103">Create windows81CompliancePolicy</span></span>

<span data-ttu-id="5436c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5436c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5436c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5436c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5436c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5436c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5436c-107">Создание объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5436c-107">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5436c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5436c-108">Prerequisites</span></span>
<span data-ttu-id="5436c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5436c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5436c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5436c-111">Permission type</span></span>|<span data-ttu-id="5436c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5436c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5436c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5436c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5436c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5436c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5436c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5436c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5436c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5436c-116">Not supported.</span></span>|
|<span data-ttu-id="5436c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5436c-117">Application</span></span>|<span data-ttu-id="5436c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5436c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5436c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5436c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5436c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5436c-120">Request headers</span></span>
|<span data-ttu-id="5436c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5436c-121">Header</span></span>|<span data-ttu-id="5436c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5436c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5436c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5436c-123">Authorization</span></span>|<span data-ttu-id="5436c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5436c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5436c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5436c-125">Accept</span></span>|<span data-ttu-id="5436c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5436c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5436c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5436c-127">Request body</span></span>
<span data-ttu-id="5436c-128">В теле запроса добавьте представление объекта windows81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5436c-128">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="5436c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="5436c-129">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="5436c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5436c-130">Property</span></span>|<span data-ttu-id="5436c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5436c-131">Type</span></span>|<span data-ttu-id="5436c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5436c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5436c-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5436c-133">roleScopeTagIds</span></span>|<span data-ttu-id="5436c-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5436c-134">String collection</span></span>|<span data-ttu-id="5436c-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5436c-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5436c-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5436c-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5436c-137">id</span><span class="sxs-lookup"><span data-stu-id="5436c-137">id</span></span>|<span data-ttu-id="5436c-138">String</span><span class="sxs-lookup"><span data-stu-id="5436c-138">String</span></span>|<span data-ttu-id="5436c-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5436c-139">Key of the entity.</span></span> <span data-ttu-id="5436c-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5436c-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5436c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5436c-141">createdDateTime</span></span>|<span data-ttu-id="5436c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5436c-142">DateTimeOffset</span></span>|<span data-ttu-id="5436c-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5436c-143">DateTime the object was created.</span></span> <span data-ttu-id="5436c-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5436c-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5436c-145">description</span><span class="sxs-lookup"><span data-stu-id="5436c-145">description</span></span>|<span data-ttu-id="5436c-146">String</span><span class="sxs-lookup"><span data-stu-id="5436c-146">String</span></span>|<span data-ttu-id="5436c-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5436c-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5436c-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5436c-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5436c-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5436c-149">lastModifiedDateTime</span></span>|<span data-ttu-id="5436c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5436c-150">DateTimeOffset</span></span>|<span data-ttu-id="5436c-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5436c-151">DateTime the object was last modified.</span></span> <span data-ttu-id="5436c-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5436c-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5436c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="5436c-153">displayName</span></span>|<span data-ttu-id="5436c-154">String</span><span class="sxs-lookup"><span data-stu-id="5436c-154">String</span></span>|<span data-ttu-id="5436c-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5436c-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5436c-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5436c-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5436c-157">version</span><span class="sxs-lookup"><span data-stu-id="5436c-157">version</span></span>|<span data-ttu-id="5436c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5436c-158">Int32</span></span>|<span data-ttu-id="5436c-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5436c-159">Version of the device configuration.</span></span> <span data-ttu-id="5436c-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5436c-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5436c-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5436c-161">passwordRequired</span></span>|<span data-ttu-id="5436c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5436c-162">Boolean</span></span>|<span data-ttu-id="5436c-163">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="5436c-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="5436c-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5436c-164">passwordBlockSimple</span></span>|<span data-ttu-id="5436c-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="5436c-165">Boolean</span></span>|<span data-ttu-id="5436c-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="5436c-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="5436c-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5436c-167">passwordExpirationDays</span></span>|<span data-ttu-id="5436c-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5436c-168">Int32</span></span>|<span data-ttu-id="5436c-169">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="5436c-169">Password expiration in days.</span></span>|
|<span data-ttu-id="5436c-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5436c-170">passwordMinimumLength</span></span>|<span data-ttu-id="5436c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5436c-171">Int32</span></span>|<span data-ttu-id="5436c-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="5436c-172">The minimum password length.</span></span>|
|<span data-ttu-id="5436c-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5436c-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5436c-174">Int32</span><span class="sxs-lookup"><span data-stu-id="5436c-174">Int32</span></span>|<span data-ttu-id="5436c-175">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="5436c-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5436c-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5436c-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5436c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5436c-177">Int32</span></span>|<span data-ttu-id="5436c-178">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="5436c-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5436c-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5436c-179">passwordRequiredType</span></span>|[<span data-ttu-id="5436c-180">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="5436c-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5436c-181">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="5436c-181">The required password type.</span></span> <span data-ttu-id="5436c-182">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="5436c-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5436c-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5436c-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5436c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5436c-184">Int32</span></span>|<span data-ttu-id="5436c-185">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="5436c-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="5436c-186">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="5436c-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="5436c-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5436c-187">osMinimumVersion</span></span>|<span data-ttu-id="5436c-188">String</span><span class="sxs-lookup"><span data-stu-id="5436c-188">String</span></span>|<span data-ttu-id="5436c-189">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="5436c-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="5436c-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5436c-190">osMaximumVersion</span></span>|<span data-ttu-id="5436c-191">String</span><span class="sxs-lookup"><span data-stu-id="5436c-191">String</span></span>|<span data-ttu-id="5436c-192">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="5436c-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="5436c-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5436c-193">storageRequireEncryption</span></span>|<span data-ttu-id="5436c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5436c-194">Boolean</span></span>|<span data-ttu-id="5436c-195">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="5436c-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="5436c-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="5436c-196">Response</span></span>
<span data-ttu-id="5436c-197">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5436c-197">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5436c-198">Пример</span><span class="sxs-lookup"><span data-stu-id="5436c-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="5436c-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="5436c-199">Request</span></span>
<span data-ttu-id="5436c-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5436c-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="5436c-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="5436c-201">Response</span></span>
<span data-ttu-id="5436c-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5436c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






