---
title: Create windowsPhone81CompliancePolicy
description: Создание объекта windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a41ff2bb58ad3e13b21a6034045ebb0c7a62d48e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018850"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="290b8-103">Create windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="290b8-103">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="290b8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="290b8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="290b8-105">Создание объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="290b8-105">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="290b8-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="290b8-106">Prerequisites</span></span>
<span data-ttu-id="290b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="290b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="290b8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="290b8-109">Permission type</span></span>|<span data-ttu-id="290b8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="290b8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="290b8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="290b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="290b8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="290b8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="290b8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="290b8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="290b8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="290b8-114">Not supported.</span></span>|
|<span data-ttu-id="290b8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="290b8-115">Application</span></span>|<span data-ttu-id="290b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="290b8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="290b8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="290b8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="290b8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="290b8-118">Request headers</span></span>
|<span data-ttu-id="290b8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="290b8-119">Header</span></span>|<span data-ttu-id="290b8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="290b8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="290b8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="290b8-121">Authorization</span></span>|<span data-ttu-id="290b8-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="290b8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="290b8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="290b8-123">Accept</span></span>|<span data-ttu-id="290b8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="290b8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="290b8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="290b8-125">Request body</span></span>
<span data-ttu-id="290b8-126">В теле запроса добавьте представление объекта windowsPhone81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="290b8-126">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="290b8-127">Ниже показаны свойства, которые необходимо указывать при создании объекта windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="290b8-127">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="290b8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="290b8-128">Property</span></span>|<span data-ttu-id="290b8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="290b8-129">Type</span></span>|<span data-ttu-id="290b8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="290b8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="290b8-131">id</span><span class="sxs-lookup"><span data-stu-id="290b8-131">id</span></span>|<span data-ttu-id="290b8-132">Строка</span><span class="sxs-lookup"><span data-stu-id="290b8-132">String</span></span>|<span data-ttu-id="290b8-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="290b8-133">Key of the entity.</span></span> <span data-ttu-id="290b8-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="290b8-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="290b8-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="290b8-135">createdDateTime</span></span>|<span data-ttu-id="290b8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="290b8-136">DateTimeOffset</span></span>|<span data-ttu-id="290b8-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="290b8-137">DateTime the object was created.</span></span> <span data-ttu-id="290b8-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="290b8-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="290b8-139">description</span><span class="sxs-lookup"><span data-stu-id="290b8-139">description</span></span>|<span data-ttu-id="290b8-140">String</span><span class="sxs-lookup"><span data-stu-id="290b8-140">String</span></span>|<span data-ttu-id="290b8-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="290b8-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="290b8-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="290b8-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="290b8-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="290b8-143">lastModifiedDateTime</span></span>|<span data-ttu-id="290b8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="290b8-144">DateTimeOffset</span></span>|<span data-ttu-id="290b8-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="290b8-145">DateTime the object was last modified.</span></span> <span data-ttu-id="290b8-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="290b8-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="290b8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="290b8-147">displayName</span></span>|<span data-ttu-id="290b8-148">Строка</span><span class="sxs-lookup"><span data-stu-id="290b8-148">String</span></span>|<span data-ttu-id="290b8-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="290b8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="290b8-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="290b8-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="290b8-151">version</span><span class="sxs-lookup"><span data-stu-id="290b8-151">version</span></span>|<span data-ttu-id="290b8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="290b8-152">Int32</span></span>|<span data-ttu-id="290b8-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="290b8-153">Version of the device configuration.</span></span> <span data-ttu-id="290b8-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="290b8-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="290b8-155">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="290b8-155">passwordBlockSimple</span></span>|<span data-ttu-id="290b8-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="290b8-156">Boolean</span></span>|<span data-ttu-id="290b8-157">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="290b8-157">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="290b8-158">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="290b8-158">passwordExpirationDays</span></span>|<span data-ttu-id="290b8-159">Int32</span><span class="sxs-lookup"><span data-stu-id="290b8-159">Int32</span></span>|<span data-ttu-id="290b8-160">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="290b8-160">Number of days before the password expires.</span></span>|
|<span data-ttu-id="290b8-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="290b8-161">passwordMinimumLength</span></span>|<span data-ttu-id="290b8-162">Int32</span><span class="sxs-lookup"><span data-stu-id="290b8-162">Int32</span></span>|<span data-ttu-id="290b8-163">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="290b8-163">Minimum length of passwords.</span></span>|
|<span data-ttu-id="290b8-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="290b8-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="290b8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="290b8-165">Int32</span></span>|<span data-ttu-id="290b8-166">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="290b8-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="290b8-167">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="290b8-167">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="290b8-168">Int32</span><span class="sxs-lookup"><span data-stu-id="290b8-168">Int32</span></span>|<span data-ttu-id="290b8-169">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="290b8-169">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="290b8-170">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="290b8-170">passwordRequiredType</span></span>|[<span data-ttu-id="290b8-171">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="290b8-171">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="290b8-172">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="290b8-172">The required password type.</span></span> <span data-ttu-id="290b8-173">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="290b8-173">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="290b8-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="290b8-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="290b8-175">Int32</span><span class="sxs-lookup"><span data-stu-id="290b8-175">Int32</span></span>|<span data-ttu-id="290b8-176">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="290b8-176">Number of previous passwords to block.</span></span> <span data-ttu-id="290b8-177">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="290b8-177">Valid values 0 to 24</span></span>|
|<span data-ttu-id="290b8-178">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="290b8-178">passwordRequired</span></span>|<span data-ttu-id="290b8-179">Логический</span><span class="sxs-lookup"><span data-stu-id="290b8-179">Boolean</span></span>|<span data-ttu-id="290b8-180">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="290b8-180">Whether or not to require a password.</span></span>|
|<span data-ttu-id="290b8-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="290b8-181">osMinimumVersion</span></span>|<span data-ttu-id="290b8-182">String</span><span class="sxs-lookup"><span data-stu-id="290b8-182">String</span></span>|<span data-ttu-id="290b8-183">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="290b8-183">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="290b8-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="290b8-184">osMaximumVersion</span></span>|<span data-ttu-id="290b8-185">String</span><span class="sxs-lookup"><span data-stu-id="290b8-185">String</span></span>|<span data-ttu-id="290b8-186">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="290b8-186">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="290b8-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="290b8-187">storageRequireEncryption</span></span>|<span data-ttu-id="290b8-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="290b8-188">Boolean</span></span>|<span data-ttu-id="290b8-189">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="290b8-189">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="290b8-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="290b8-190">Response</span></span>
<span data-ttu-id="290b8-191">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="290b8-191">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="290b8-192">Пример</span><span class="sxs-lookup"><span data-stu-id="290b8-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="290b8-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="290b8-193">Request</span></span>
<span data-ttu-id="290b8-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="290b8-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="290b8-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="290b8-195">Response</span></span>
<span data-ttu-id="290b8-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="290b8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



