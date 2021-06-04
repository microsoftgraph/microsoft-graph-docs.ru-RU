---
title: Создание объекта windows81CompliancePolicy
description: Создание объекта windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b5cc71fa9e35021afae933079a76ea257328b37a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752660"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="5205c-103">Создание объекта windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5205c-103">Create windows81CompliancePolicy</span></span>

<span data-ttu-id="5205c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5205c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5205c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5205c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5205c-106">Создание объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5205c-106">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5205c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5205c-107">Prerequisites</span></span>
<span data-ttu-id="5205c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5205c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5205c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5205c-110">Permission type</span></span>|<span data-ttu-id="5205c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5205c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5205c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5205c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5205c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5205c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5205c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5205c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5205c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5205c-115">Not supported.</span></span>|
|<span data-ttu-id="5205c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5205c-116">Application</span></span>|<span data-ttu-id="5205c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5205c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5205c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5205c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5205c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5205c-119">Request headers</span></span>
|<span data-ttu-id="5205c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5205c-120">Header</span></span>|<span data-ttu-id="5205c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5205c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5205c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5205c-122">Authorization</span></span>|<span data-ttu-id="5205c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5205c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5205c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5205c-124">Accept</span></span>|<span data-ttu-id="5205c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5205c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5205c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5205c-126">Request body</span></span>
<span data-ttu-id="5205c-127">В теле запроса добавьте представление объекта windows81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5205c-127">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="5205c-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="5205c-128">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="5205c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5205c-129">Property</span></span>|<span data-ttu-id="5205c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5205c-130">Type</span></span>|<span data-ttu-id="5205c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5205c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5205c-132">id</span><span class="sxs-lookup"><span data-stu-id="5205c-132">id</span></span>|<span data-ttu-id="5205c-133">String</span><span class="sxs-lookup"><span data-stu-id="5205c-133">String</span></span>|<span data-ttu-id="5205c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5205c-134">Key of the entity.</span></span> <span data-ttu-id="5205c-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5205c-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5205c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5205c-136">createdDateTime</span></span>|<span data-ttu-id="5205c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5205c-137">DateTimeOffset</span></span>|<span data-ttu-id="5205c-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5205c-138">DateTime the object was created.</span></span> <span data-ttu-id="5205c-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5205c-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5205c-140">description</span><span class="sxs-lookup"><span data-stu-id="5205c-140">description</span></span>|<span data-ttu-id="5205c-141">String</span><span class="sxs-lookup"><span data-stu-id="5205c-141">String</span></span>|<span data-ttu-id="5205c-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5205c-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5205c-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5205c-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5205c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5205c-144">lastModifiedDateTime</span></span>|<span data-ttu-id="5205c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5205c-145">DateTimeOffset</span></span>|<span data-ttu-id="5205c-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5205c-146">DateTime the object was last modified.</span></span> <span data-ttu-id="5205c-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5205c-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5205c-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5205c-148">displayName</span></span>|<span data-ttu-id="5205c-149">String</span><span class="sxs-lookup"><span data-stu-id="5205c-149">String</span></span>|<span data-ttu-id="5205c-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5205c-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5205c-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5205c-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5205c-152">version</span><span class="sxs-lookup"><span data-stu-id="5205c-152">version</span></span>|<span data-ttu-id="5205c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5205c-153">Int32</span></span>|<span data-ttu-id="5205c-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5205c-154">Version of the device configuration.</span></span> <span data-ttu-id="5205c-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5205c-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5205c-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5205c-156">passwordRequired</span></span>|<span data-ttu-id="5205c-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="5205c-157">Boolean</span></span>|<span data-ttu-id="5205c-158">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="5205c-158">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="5205c-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5205c-159">passwordBlockSimple</span></span>|<span data-ttu-id="5205c-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="5205c-160">Boolean</span></span>|<span data-ttu-id="5205c-161">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="5205c-161">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="5205c-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5205c-162">passwordExpirationDays</span></span>|<span data-ttu-id="5205c-163">Int32</span><span class="sxs-lookup"><span data-stu-id="5205c-163">Int32</span></span>|<span data-ttu-id="5205c-164">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="5205c-164">Password expiration in days.</span></span>|
|<span data-ttu-id="5205c-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5205c-165">passwordMinimumLength</span></span>|<span data-ttu-id="5205c-166">Int32</span><span class="sxs-lookup"><span data-stu-id="5205c-166">Int32</span></span>|<span data-ttu-id="5205c-167">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="5205c-167">The minimum password length.</span></span>|
|<span data-ttu-id="5205c-168">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5205c-168">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5205c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="5205c-169">Int32</span></span>|<span data-ttu-id="5205c-170">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="5205c-170">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5205c-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5205c-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5205c-172">Int32</span><span class="sxs-lookup"><span data-stu-id="5205c-172">Int32</span></span>|<span data-ttu-id="5205c-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="5205c-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5205c-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5205c-174">passwordRequiredType</span></span>|[<span data-ttu-id="5205c-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5205c-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5205c-176">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="5205c-176">The required password type.</span></span> <span data-ttu-id="5205c-177">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="5205c-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5205c-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5205c-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5205c-179">Int32</span><span class="sxs-lookup"><span data-stu-id="5205c-179">Int32</span></span>|<span data-ttu-id="5205c-180">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="5205c-180">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="5205c-181">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="5205c-181">Valid values 0 to 24</span></span>|
|<span data-ttu-id="5205c-182">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5205c-182">osMinimumVersion</span></span>|<span data-ttu-id="5205c-183">String</span><span class="sxs-lookup"><span data-stu-id="5205c-183">String</span></span>|<span data-ttu-id="5205c-184">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="5205c-184">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="5205c-185">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5205c-185">osMaximumVersion</span></span>|<span data-ttu-id="5205c-186">String</span><span class="sxs-lookup"><span data-stu-id="5205c-186">String</span></span>|<span data-ttu-id="5205c-187">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="5205c-187">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="5205c-188">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5205c-188">storageRequireEncryption</span></span>|<span data-ttu-id="5205c-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="5205c-189">Boolean</span></span>|<span data-ttu-id="5205c-190">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="5205c-190">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="5205c-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="5205c-191">Response</span></span>
<span data-ttu-id="5205c-192">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5205c-192">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5205c-193">Пример</span><span class="sxs-lookup"><span data-stu-id="5205c-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="5205c-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="5205c-194">Request</span></span>
<span data-ttu-id="5205c-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5205c-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="5205c-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="5205c-196">Response</span></span>
<span data-ttu-id="5205c-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5205c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
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




