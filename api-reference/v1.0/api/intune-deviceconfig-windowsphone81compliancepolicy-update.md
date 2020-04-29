---
title: Обновление объекта windowsPhone81CompliancePolicy
description: Обновление свойств объекта windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 183edcc5d6559ce0f60cb4864a28c80d7a50b5f7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399394"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="f176c-103">Обновление объекта windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f176c-103">Update windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="f176c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f176c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f176c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f176c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f176c-106">Обновление свойств объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f176c-106">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f176c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f176c-107">Prerequisites</span></span>
<span data-ttu-id="f176c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f176c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f176c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f176c-110">Permission type</span></span>|<span data-ttu-id="f176c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f176c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f176c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f176c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f176c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f176c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f176c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f176c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f176c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f176c-115">Not supported.</span></span>|
|<span data-ttu-id="f176c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f176c-116">Application</span></span>|<span data-ttu-id="f176c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f176c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f176c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f176c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f176c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f176c-119">Request headers</span></span>
|<span data-ttu-id="f176c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f176c-120">Header</span></span>|<span data-ttu-id="f176c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f176c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f176c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f176c-122">Authorization</span></span>|<span data-ttu-id="f176c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f176c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f176c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f176c-124">Accept</span></span>|<span data-ttu-id="f176c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f176c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f176c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f176c-126">Request body</span></span>
<span data-ttu-id="f176c-127">В теле запроса добавьте представление объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f176c-127">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="f176c-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f176c-128">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="f176c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f176c-129">Property</span></span>|<span data-ttu-id="f176c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f176c-130">Type</span></span>|<span data-ttu-id="f176c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f176c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f176c-132">id</span><span class="sxs-lookup"><span data-stu-id="f176c-132">id</span></span>|<span data-ttu-id="f176c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f176c-133">String</span></span>|<span data-ttu-id="f176c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f176c-134">Key of the entity.</span></span> <span data-ttu-id="f176c-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f176c-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f176c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f176c-136">createdDateTime</span></span>|<span data-ttu-id="f176c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f176c-137">DateTimeOffset</span></span>|<span data-ttu-id="f176c-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f176c-138">DateTime the object was created.</span></span> <span data-ttu-id="f176c-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f176c-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f176c-140">description</span><span class="sxs-lookup"><span data-stu-id="f176c-140">description</span></span>|<span data-ttu-id="f176c-141">String</span><span class="sxs-lookup"><span data-stu-id="f176c-141">String</span></span>|<span data-ttu-id="f176c-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f176c-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f176c-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f176c-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f176c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f176c-144">lastModifiedDateTime</span></span>|<span data-ttu-id="f176c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f176c-145">DateTimeOffset</span></span>|<span data-ttu-id="f176c-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f176c-146">DateTime the object was last modified.</span></span> <span data-ttu-id="f176c-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f176c-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f176c-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f176c-148">displayName</span></span>|<span data-ttu-id="f176c-149">Строка</span><span class="sxs-lookup"><span data-stu-id="f176c-149">String</span></span>|<span data-ttu-id="f176c-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f176c-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f176c-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f176c-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f176c-152">version</span><span class="sxs-lookup"><span data-stu-id="f176c-152">version</span></span>|<span data-ttu-id="f176c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f176c-153">Int32</span></span>|<span data-ttu-id="f176c-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f176c-154">Version of the device configuration.</span></span> <span data-ttu-id="f176c-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f176c-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f176c-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f176c-156">passwordBlockSimple</span></span>|<span data-ttu-id="f176c-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f176c-157">Boolean</span></span>|<span data-ttu-id="f176c-158">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="f176c-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="f176c-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f176c-159">passwordExpirationDays</span></span>|<span data-ttu-id="f176c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f176c-160">Int32</span></span>|<span data-ttu-id="f176c-161">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="f176c-161">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f176c-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f176c-162">passwordMinimumLength</span></span>|<span data-ttu-id="f176c-163">Int32</span><span class="sxs-lookup"><span data-stu-id="f176c-163">Int32</span></span>|<span data-ttu-id="f176c-164">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="f176c-164">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f176c-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f176c-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f176c-166">Int32</span><span class="sxs-lookup"><span data-stu-id="f176c-166">Int32</span></span>|<span data-ttu-id="f176c-167">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="f176c-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f176c-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f176c-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f176c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f176c-169">Int32</span></span>|<span data-ttu-id="f176c-170">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="f176c-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f176c-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f176c-171">passwordRequiredType</span></span>|[<span data-ttu-id="f176c-172">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="f176c-172">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f176c-173">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="f176c-173">The required password type.</span></span> <span data-ttu-id="f176c-174">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f176c-174">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f176c-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f176c-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f176c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f176c-176">Int32</span></span>|<span data-ttu-id="f176c-177">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="f176c-177">Number of previous passwords to block.</span></span> <span data-ttu-id="f176c-178">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="f176c-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f176c-179">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f176c-179">passwordRequired</span></span>|<span data-ttu-id="f176c-180">Логический</span><span class="sxs-lookup"><span data-stu-id="f176c-180">Boolean</span></span>|<span data-ttu-id="f176c-181">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="f176c-181">Whether or not to require a password.</span></span>|
|<span data-ttu-id="f176c-182">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f176c-182">osMinimumVersion</span></span>|<span data-ttu-id="f176c-183">String</span><span class="sxs-lookup"><span data-stu-id="f176c-183">String</span></span>|<span data-ttu-id="f176c-184">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f176c-184">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="f176c-185">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f176c-185">osMaximumVersion</span></span>|<span data-ttu-id="f176c-186">String</span><span class="sxs-lookup"><span data-stu-id="f176c-186">String</span></span>|<span data-ttu-id="f176c-187">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f176c-187">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="f176c-188">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f176c-188">storageRequireEncryption</span></span>|<span data-ttu-id="f176c-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="f176c-189">Boolean</span></span>|<span data-ttu-id="f176c-190">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f176c-190">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="f176c-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="f176c-191">Response</span></span>
<span data-ttu-id="f176c-192">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f176c-192">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f176c-193">Пример</span><span class="sxs-lookup"><span data-stu-id="f176c-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="f176c-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="f176c-194">Request</span></span>
<span data-ttu-id="f176c-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f176c-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 607

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="f176c-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="f176c-196">Response</span></span>
<span data-ttu-id="f176c-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f176c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```






