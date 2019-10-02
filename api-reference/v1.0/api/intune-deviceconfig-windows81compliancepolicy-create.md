---
title: Создание объекта windows81CompliancePolicy
description: Создание объекта windows81CompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d40b3060a1a81e57271fe73b6480ac586da30380
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365119"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="7ff78-103">Создание объекта windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7ff78-103">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="7ff78-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ff78-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ff78-105">Создание объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7ff78-105">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ff78-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7ff78-106">Prerequisites</span></span>
<span data-ttu-id="7ff78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ff78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ff78-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ff78-109">Permission type</span></span>|<span data-ttu-id="7ff78-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ff78-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ff78-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ff78-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7ff78-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ff78-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ff78-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ff78-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ff78-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ff78-114">Not supported.</span></span>|
|<span data-ttu-id="7ff78-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ff78-115">Application</span></span>|<span data-ttu-id="7ff78-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ff78-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ff78-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ff78-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7ff78-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ff78-118">Request headers</span></span>
|<span data-ttu-id="7ff78-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ff78-119">Header</span></span>|<span data-ttu-id="7ff78-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7ff78-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ff78-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ff78-121">Authorization</span></span>|<span data-ttu-id="7ff78-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ff78-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ff78-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7ff78-123">Accept</span></span>|<span data-ttu-id="7ff78-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7ff78-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ff78-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ff78-125">Request body</span></span>
<span data-ttu-id="7ff78-126">В теле запроса добавьте представление объекта windows81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ff78-126">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="7ff78-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="7ff78-127">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="7ff78-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ff78-128">Property</span></span>|<span data-ttu-id="7ff78-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7ff78-129">Type</span></span>|<span data-ttu-id="7ff78-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff78-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ff78-131">id</span><span class="sxs-lookup"><span data-stu-id="7ff78-131">id</span></span>|<span data-ttu-id="7ff78-132">Строка</span><span class="sxs-lookup"><span data-stu-id="7ff78-132">String</span></span>|<span data-ttu-id="7ff78-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7ff78-133">Key of the entity.</span></span> <span data-ttu-id="7ff78-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7ff78-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff78-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ff78-135">createdDateTime</span></span>|<span data-ttu-id="7ff78-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ff78-136">DateTimeOffset</span></span>|<span data-ttu-id="7ff78-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7ff78-137">DateTime the object was created.</span></span> <span data-ttu-id="7ff78-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7ff78-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff78-139">description</span><span class="sxs-lookup"><span data-stu-id="7ff78-139">description</span></span>|<span data-ttu-id="7ff78-140">String</span><span class="sxs-lookup"><span data-stu-id="7ff78-140">String</span></span>|<span data-ttu-id="7ff78-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7ff78-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7ff78-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7ff78-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff78-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ff78-143">lastModifiedDateTime</span></span>|<span data-ttu-id="7ff78-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ff78-144">DateTimeOffset</span></span>|<span data-ttu-id="7ff78-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7ff78-145">DateTime the object was last modified.</span></span> <span data-ttu-id="7ff78-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7ff78-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff78-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7ff78-147">displayName</span></span>|<span data-ttu-id="7ff78-148">Строка</span><span class="sxs-lookup"><span data-stu-id="7ff78-148">String</span></span>|<span data-ttu-id="7ff78-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7ff78-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7ff78-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7ff78-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff78-151">version</span><span class="sxs-lookup"><span data-stu-id="7ff78-151">version</span></span>|<span data-ttu-id="7ff78-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff78-152">Int32</span></span>|<span data-ttu-id="7ff78-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7ff78-153">Version of the device configuration.</span></span> <span data-ttu-id="7ff78-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7ff78-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff78-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7ff78-155">passwordRequired</span></span>|<span data-ttu-id="7ff78-156">Логический</span><span class="sxs-lookup"><span data-stu-id="7ff78-156">Boolean</span></span>|<span data-ttu-id="7ff78-157">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="7ff78-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="7ff78-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7ff78-158">passwordBlockSimple</span></span>|<span data-ttu-id="7ff78-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ff78-159">Boolean</span></span>|<span data-ttu-id="7ff78-160">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="7ff78-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="7ff78-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7ff78-161">passwordExpirationDays</span></span>|<span data-ttu-id="7ff78-162">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff78-162">Int32</span></span>|<span data-ttu-id="7ff78-163">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="7ff78-163">Password expiration in days.</span></span>|
|<span data-ttu-id="7ff78-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7ff78-164">passwordMinimumLength</span></span>|<span data-ttu-id="7ff78-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff78-165">Int32</span></span>|<span data-ttu-id="7ff78-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="7ff78-166">The minimum password length.</span></span>|
|<span data-ttu-id="7ff78-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7ff78-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7ff78-168">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff78-168">Int32</span></span>|<span data-ttu-id="7ff78-169">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="7ff78-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7ff78-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7ff78-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7ff78-171">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff78-171">Int32</span></span>|<span data-ttu-id="7ff78-172">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="7ff78-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7ff78-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7ff78-173">passwordRequiredType</span></span>|[<span data-ttu-id="7ff78-174">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="7ff78-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="7ff78-175">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="7ff78-175">The required password type.</span></span> <span data-ttu-id="7ff78-176">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="7ff78-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7ff78-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7ff78-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7ff78-178">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff78-178">Int32</span></span>|<span data-ttu-id="7ff78-179">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="7ff78-179">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="7ff78-180">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="7ff78-180">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7ff78-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7ff78-181">osMinimumVersion</span></span>|<span data-ttu-id="7ff78-182">String</span><span class="sxs-lookup"><span data-stu-id="7ff78-182">String</span></span>|<span data-ttu-id="7ff78-183">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="7ff78-183">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="7ff78-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7ff78-184">osMaximumVersion</span></span>|<span data-ttu-id="7ff78-185">String</span><span class="sxs-lookup"><span data-stu-id="7ff78-185">String</span></span>|<span data-ttu-id="7ff78-186">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="7ff78-186">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="7ff78-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7ff78-187">storageRequireEncryption</span></span>|<span data-ttu-id="7ff78-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ff78-188">Boolean</span></span>|<span data-ttu-id="7ff78-189">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="7ff78-189">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="7ff78-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff78-190">Response</span></span>
<span data-ttu-id="7ff78-191">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ff78-191">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ff78-192">Пример</span><span class="sxs-lookup"><span data-stu-id="7ff78-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ff78-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff78-193">Request</span></span>
<span data-ttu-id="7ff78-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ff78-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ff78-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff78-195">Response</span></span>
<span data-ttu-id="7ff78-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ff78-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




