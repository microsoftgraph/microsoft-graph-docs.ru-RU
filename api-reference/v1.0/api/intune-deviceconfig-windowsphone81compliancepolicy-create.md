---
title: Create windowsPhone81CompliancePolicy
description: Создание объекта windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00bc01765c5b6f6fac30c45e93ce65ea3b6da974
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747216"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="0d463-103">Create windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0d463-103">Create windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="0d463-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d463-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d463-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d463-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d463-106">Создание объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d463-106">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d463-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0d463-107">Prerequisites</span></span>
<span data-ttu-id="0d463-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d463-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d463-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d463-110">Permission type</span></span>|<span data-ttu-id="0d463-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d463-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d463-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d463-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d463-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d463-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d463-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d463-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d463-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d463-115">Not supported.</span></span>|
|<span data-ttu-id="0d463-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0d463-116">Application</span></span>|<span data-ttu-id="0d463-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d463-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d463-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d463-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0d463-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d463-119">Request headers</span></span>
|<span data-ttu-id="0d463-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d463-120">Header</span></span>|<span data-ttu-id="0d463-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0d463-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d463-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d463-122">Authorization</span></span>|<span data-ttu-id="0d463-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d463-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d463-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0d463-124">Accept</span></span>|<span data-ttu-id="0d463-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d463-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d463-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d463-126">Request body</span></span>
<span data-ttu-id="0d463-127">В теле запроса добавьте представление объекта windowsPhone81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d463-127">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="0d463-128">Ниже показаны свойства, которые необходимо указывать при создании объекта windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="0d463-128">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="0d463-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d463-129">Property</span></span>|<span data-ttu-id="0d463-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0d463-130">Type</span></span>|<span data-ttu-id="0d463-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0d463-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d463-132">id</span><span class="sxs-lookup"><span data-stu-id="0d463-132">id</span></span>|<span data-ttu-id="0d463-133">String</span><span class="sxs-lookup"><span data-stu-id="0d463-133">String</span></span>|<span data-ttu-id="0d463-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0d463-134">Key of the entity.</span></span> <span data-ttu-id="0d463-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d463-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d463-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d463-136">createdDateTime</span></span>|<span data-ttu-id="0d463-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d463-137">DateTimeOffset</span></span>|<span data-ttu-id="0d463-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0d463-138">DateTime the object was created.</span></span> <span data-ttu-id="0d463-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d463-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d463-140">description</span><span class="sxs-lookup"><span data-stu-id="0d463-140">description</span></span>|<span data-ttu-id="0d463-141">String</span><span class="sxs-lookup"><span data-stu-id="0d463-141">String</span></span>|<span data-ttu-id="0d463-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d463-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0d463-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d463-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d463-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d463-144">lastModifiedDateTime</span></span>|<span data-ttu-id="0d463-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d463-145">DateTimeOffset</span></span>|<span data-ttu-id="0d463-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0d463-146">DateTime the object was last modified.</span></span> <span data-ttu-id="0d463-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d463-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d463-148">displayName</span><span class="sxs-lookup"><span data-stu-id="0d463-148">displayName</span></span>|<span data-ttu-id="0d463-149">String</span><span class="sxs-lookup"><span data-stu-id="0d463-149">String</span></span>|<span data-ttu-id="0d463-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d463-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0d463-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d463-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d463-152">version</span><span class="sxs-lookup"><span data-stu-id="0d463-152">version</span></span>|<span data-ttu-id="0d463-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0d463-153">Int32</span></span>|<span data-ttu-id="0d463-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d463-154">Version of the device configuration.</span></span> <span data-ttu-id="0d463-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d463-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d463-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0d463-156">passwordBlockSimple</span></span>|<span data-ttu-id="0d463-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d463-157">Boolean</span></span>|<span data-ttu-id="0d463-158">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="0d463-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="0d463-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0d463-159">passwordExpirationDays</span></span>|<span data-ttu-id="0d463-160">Int32</span><span class="sxs-lookup"><span data-stu-id="0d463-160">Int32</span></span>|<span data-ttu-id="0d463-161">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="0d463-161">Number of days before the password expires.</span></span>|
|<span data-ttu-id="0d463-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0d463-162">passwordMinimumLength</span></span>|<span data-ttu-id="0d463-163">Int32</span><span class="sxs-lookup"><span data-stu-id="0d463-163">Int32</span></span>|<span data-ttu-id="0d463-164">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="0d463-164">Minimum length of passwords.</span></span>|
|<span data-ttu-id="0d463-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0d463-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0d463-166">Int32</span><span class="sxs-lookup"><span data-stu-id="0d463-166">Int32</span></span>|<span data-ttu-id="0d463-167">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="0d463-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0d463-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0d463-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0d463-169">Int32</span><span class="sxs-lookup"><span data-stu-id="0d463-169">Int32</span></span>|<span data-ttu-id="0d463-170">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="0d463-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0d463-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0d463-171">passwordRequiredType</span></span>|[<span data-ttu-id="0d463-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0d463-172">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0d463-173">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="0d463-173">The required password type.</span></span> <span data-ttu-id="0d463-174">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0d463-174">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0d463-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0d463-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0d463-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0d463-176">Int32</span></span>|<span data-ttu-id="0d463-177">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="0d463-177">Number of previous passwords to block.</span></span> <span data-ttu-id="0d463-178">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="0d463-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="0d463-179">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0d463-179">passwordRequired</span></span>|<span data-ttu-id="0d463-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d463-180">Boolean</span></span>|<span data-ttu-id="0d463-181">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="0d463-181">Whether or not to require a password.</span></span>|
|<span data-ttu-id="0d463-182">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0d463-182">osMinimumVersion</span></span>|<span data-ttu-id="0d463-183">String</span><span class="sxs-lookup"><span data-stu-id="0d463-183">String</span></span>|<span data-ttu-id="0d463-184">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="0d463-184">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="0d463-185">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0d463-185">osMaximumVersion</span></span>|<span data-ttu-id="0d463-186">String</span><span class="sxs-lookup"><span data-stu-id="0d463-186">String</span></span>|<span data-ttu-id="0d463-187">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="0d463-187">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="0d463-188">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0d463-188">storageRequireEncryption</span></span>|<span data-ttu-id="0d463-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d463-189">Boolean</span></span>|<span data-ttu-id="0d463-190">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="0d463-190">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="0d463-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d463-191">Response</span></span>
<span data-ttu-id="0d463-192">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0d463-192">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d463-193">Пример</span><span class="sxs-lookup"><span data-stu-id="0d463-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d463-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d463-194">Request</span></span>
<span data-ttu-id="0d463-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d463-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="0d463-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d463-196">Response</span></span>
<span data-ttu-id="0d463-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d463-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




