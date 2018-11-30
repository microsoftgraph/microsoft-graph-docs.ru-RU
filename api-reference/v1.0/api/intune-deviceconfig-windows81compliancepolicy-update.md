---
title: Update windows81CompliancePolicy
description: Обновление свойств объекта windows81CompliancePolicy.
ms.openlocfilehash: 52e76e1be627633f6bba0a78c451afb8b184d265
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026773"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="54cf5-103">Update windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="54cf5-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="54cf5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="54cf5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54cf5-105">Обновление свойств объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54cf5-105">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54cf5-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="54cf5-106">Prerequisites</span></span>
<span data-ttu-id="54cf5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54cf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54cf5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54cf5-109">Permission type</span></span>|<span data-ttu-id="54cf5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54cf5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54cf5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54cf5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="54cf5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54cf5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54cf5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54cf5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54cf5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54cf5-114">Not supported.</span></span>|
|<span data-ttu-id="54cf5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54cf5-115">Application</span></span>|<span data-ttu-id="54cf5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54cf5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54cf5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54cf5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="54cf5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54cf5-118">Request headers</span></span>
|<span data-ttu-id="54cf5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54cf5-119">Header</span></span>|<span data-ttu-id="54cf5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="54cf5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54cf5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="54cf5-121">Authorization</span></span>|<span data-ttu-id="54cf5-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="54cf5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54cf5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="54cf5-123">Accept</span></span>|<span data-ttu-id="54cf5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="54cf5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54cf5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="54cf5-125">Request body</span></span>
<span data-ttu-id="54cf5-126">В теле запроса добавьте представление объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54cf5-126">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="54cf5-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54cf5-127">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="54cf5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="54cf5-128">Property</span></span>|<span data-ttu-id="54cf5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="54cf5-129">Type</span></span>|<span data-ttu-id="54cf5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="54cf5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54cf5-131">id</span><span class="sxs-lookup"><span data-stu-id="54cf5-131">id</span></span>|<span data-ttu-id="54cf5-132">String</span><span class="sxs-lookup"><span data-stu-id="54cf5-132">String</span></span>|<span data-ttu-id="54cf5-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="54cf5-133">Key of the entity.</span></span> <span data-ttu-id="54cf5-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54cf5-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54cf5-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54cf5-135">createdDateTime</span></span>|<span data-ttu-id="54cf5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54cf5-136">DateTimeOffset</span></span>|<span data-ttu-id="54cf5-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="54cf5-137">DateTime the object was created.</span></span> <span data-ttu-id="54cf5-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54cf5-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54cf5-139">описание</span><span class="sxs-lookup"><span data-stu-id="54cf5-139">description</span></span>|<span data-ttu-id="54cf5-140">String</span><span class="sxs-lookup"><span data-stu-id="54cf5-140">String</span></span>|<span data-ttu-id="54cf5-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54cf5-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54cf5-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54cf5-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54cf5-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54cf5-143">lastModifiedDateTime</span></span>|<span data-ttu-id="54cf5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54cf5-144">DateTimeOffset</span></span>|<span data-ttu-id="54cf5-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="54cf5-145">DateTime the object was last modified.</span></span> <span data-ttu-id="54cf5-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54cf5-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54cf5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="54cf5-147">displayName</span></span>|<span data-ttu-id="54cf5-148">String</span><span class="sxs-lookup"><span data-stu-id="54cf5-148">String</span></span>|<span data-ttu-id="54cf5-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54cf5-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54cf5-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54cf5-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54cf5-151">version</span><span class="sxs-lookup"><span data-stu-id="54cf5-151">version</span></span>|<span data-ttu-id="54cf5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="54cf5-152">Int32</span></span>|<span data-ttu-id="54cf5-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54cf5-153">Version of the device configuration.</span></span> <span data-ttu-id="54cf5-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54cf5-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54cf5-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="54cf5-155">passwordRequired</span></span>|<span data-ttu-id="54cf5-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="54cf5-156">Boolean</span></span>|<span data-ttu-id="54cf5-157">Указывает, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="54cf5-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="54cf5-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="54cf5-158">passwordBlockSimple</span></span>|<span data-ttu-id="54cf5-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="54cf5-159">Boolean</span></span>|<span data-ttu-id="54cf5-160">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="54cf5-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="54cf5-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="54cf5-161">passwordExpirationDays</span></span>|<span data-ttu-id="54cf5-162">Int32</span><span class="sxs-lookup"><span data-stu-id="54cf5-162">Int32</span></span>|<span data-ttu-id="54cf5-163">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="54cf5-163">Password expiration in days.</span></span>|
|<span data-ttu-id="54cf5-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="54cf5-164">passwordMinimumLength</span></span>|<span data-ttu-id="54cf5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="54cf5-165">Int32</span></span>|<span data-ttu-id="54cf5-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="54cf5-166">The minimum password length.</span></span>|
|<span data-ttu-id="54cf5-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="54cf5-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="54cf5-168">Int32</span><span class="sxs-lookup"><span data-stu-id="54cf5-168">Int32</span></span>|<span data-ttu-id="54cf5-169">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="54cf5-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="54cf5-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="54cf5-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="54cf5-171">Int32</span><span class="sxs-lookup"><span data-stu-id="54cf5-171">Int32</span></span>|<span data-ttu-id="54cf5-172">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="54cf5-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="54cf5-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="54cf5-173">passwordRequiredType</span></span>|[<span data-ttu-id="54cf5-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="54cf5-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="54cf5-175">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="54cf5-175">The required password type.</span></span> <span data-ttu-id="54cf5-176">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="54cf5-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="54cf5-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="54cf5-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="54cf5-178">Int32</span><span class="sxs-lookup"><span data-stu-id="54cf5-178">Int32</span></span>|<span data-ttu-id="54cf5-179">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="54cf5-179">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="54cf5-180">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="54cf5-180">Valid values 0 to 24</span></span>|
|<span data-ttu-id="54cf5-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="54cf5-181">osMinimumVersion</span></span>|<span data-ttu-id="54cf5-182">String</span><span class="sxs-lookup"><span data-stu-id="54cf5-182">String</span></span>|<span data-ttu-id="54cf5-183">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="54cf5-183">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="54cf5-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="54cf5-184">osMaximumVersion</span></span>|<span data-ttu-id="54cf5-185">String</span><span class="sxs-lookup"><span data-stu-id="54cf5-185">String</span></span>|<span data-ttu-id="54cf5-186">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="54cf5-186">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="54cf5-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="54cf5-187">storageRequireEncryption</span></span>|<span data-ttu-id="54cf5-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="54cf5-188">Boolean</span></span>|<span data-ttu-id="54cf5-189">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="54cf5-189">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="54cf5-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="54cf5-190">Response</span></span>
<span data-ttu-id="54cf5-191">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="54cf5-191">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54cf5-192">Пример</span><span class="sxs-lookup"><span data-stu-id="54cf5-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="54cf5-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="54cf5-193">Request</span></span>
<span data-ttu-id="54cf5-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54cf5-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="54cf5-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="54cf5-195">Response</span></span>
<span data-ttu-id="54cf5-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="54cf5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



