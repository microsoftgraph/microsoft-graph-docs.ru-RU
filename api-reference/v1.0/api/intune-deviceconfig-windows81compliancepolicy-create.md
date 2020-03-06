---
title: Создание объекта windows81CompliancePolicy
description: Создание объекта windows81CompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 52c4abd8fb0ee58a5ebdd2468997cc4fe5e1bda7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513908"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="5b41f-103">Создание объекта windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5b41f-103">Create windows81CompliancePolicy</span></span>

<span data-ttu-id="5b41f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b41f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b41f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b41f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b41f-106">Создание объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b41f-106">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b41f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5b41f-107">Prerequisites</span></span>
<span data-ttu-id="5b41f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b41f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b41f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b41f-110">Permission type</span></span>|<span data-ttu-id="5b41f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b41f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b41f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b41f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b41f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b41f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b41f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b41f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b41f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b41f-115">Not supported.</span></span>|
|<span data-ttu-id="5b41f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b41f-116">Application</span></span>|<span data-ttu-id="5b41f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b41f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b41f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b41f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5b41f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5b41f-119">Request headers</span></span>
|<span data-ttu-id="5b41f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b41f-120">Header</span></span>|<span data-ttu-id="5b41f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5b41f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b41f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b41f-122">Authorization</span></span>|<span data-ttu-id="5b41f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b41f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b41f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5b41f-124">Accept</span></span>|<span data-ttu-id="5b41f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b41f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b41f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b41f-126">Request body</span></span>
<span data-ttu-id="5b41f-127">В теле запроса добавьте представление объекта windows81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b41f-127">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="5b41f-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="5b41f-128">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="5b41f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b41f-129">Property</span></span>|<span data-ttu-id="5b41f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5b41f-130">Type</span></span>|<span data-ttu-id="5b41f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5b41f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b41f-132">id</span><span class="sxs-lookup"><span data-stu-id="5b41f-132">id</span></span>|<span data-ttu-id="5b41f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5b41f-133">String</span></span>|<span data-ttu-id="5b41f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5b41f-134">Key of the entity.</span></span> <span data-ttu-id="5b41f-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b41f-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b41f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b41f-136">createdDateTime</span></span>|<span data-ttu-id="5b41f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b41f-137">DateTimeOffset</span></span>|<span data-ttu-id="5b41f-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5b41f-138">DateTime the object was created.</span></span> <span data-ttu-id="5b41f-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b41f-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b41f-140">description</span><span class="sxs-lookup"><span data-stu-id="5b41f-140">description</span></span>|<span data-ttu-id="5b41f-141">String</span><span class="sxs-lookup"><span data-stu-id="5b41f-141">String</span></span>|<span data-ttu-id="5b41f-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b41f-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5b41f-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b41f-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b41f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b41f-144">lastModifiedDateTime</span></span>|<span data-ttu-id="5b41f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b41f-145">DateTimeOffset</span></span>|<span data-ttu-id="5b41f-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5b41f-146">DateTime the object was last modified.</span></span> <span data-ttu-id="5b41f-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b41f-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b41f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5b41f-148">displayName</span></span>|<span data-ttu-id="5b41f-149">Строка</span><span class="sxs-lookup"><span data-stu-id="5b41f-149">String</span></span>|<span data-ttu-id="5b41f-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b41f-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5b41f-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b41f-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b41f-152">version</span><span class="sxs-lookup"><span data-stu-id="5b41f-152">version</span></span>|<span data-ttu-id="5b41f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5b41f-153">Int32</span></span>|<span data-ttu-id="5b41f-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b41f-154">Version of the device configuration.</span></span> <span data-ttu-id="5b41f-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b41f-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5b41f-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5b41f-156">passwordRequired</span></span>|<span data-ttu-id="5b41f-157">Логический</span><span class="sxs-lookup"><span data-stu-id="5b41f-157">Boolean</span></span>|<span data-ttu-id="5b41f-158">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="5b41f-158">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="5b41f-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5b41f-159">passwordBlockSimple</span></span>|<span data-ttu-id="5b41f-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b41f-160">Boolean</span></span>|<span data-ttu-id="5b41f-161">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="5b41f-161">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="5b41f-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5b41f-162">passwordExpirationDays</span></span>|<span data-ttu-id="5b41f-163">Int32</span><span class="sxs-lookup"><span data-stu-id="5b41f-163">Int32</span></span>|<span data-ttu-id="5b41f-164">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="5b41f-164">Password expiration in days.</span></span>|
|<span data-ttu-id="5b41f-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5b41f-165">passwordMinimumLength</span></span>|<span data-ttu-id="5b41f-166">Int32</span><span class="sxs-lookup"><span data-stu-id="5b41f-166">Int32</span></span>|<span data-ttu-id="5b41f-167">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="5b41f-167">The minimum password length.</span></span>|
|<span data-ttu-id="5b41f-168">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5b41f-168">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5b41f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="5b41f-169">Int32</span></span>|<span data-ttu-id="5b41f-170">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="5b41f-170">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5b41f-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5b41f-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5b41f-172">Int32</span><span class="sxs-lookup"><span data-stu-id="5b41f-172">Int32</span></span>|<span data-ttu-id="5b41f-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="5b41f-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5b41f-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5b41f-174">passwordRequiredType</span></span>|[<span data-ttu-id="5b41f-175">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="5b41f-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5b41f-176">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="5b41f-176">The required password type.</span></span> <span data-ttu-id="5b41f-177">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="5b41f-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5b41f-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5b41f-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5b41f-179">Int32</span><span class="sxs-lookup"><span data-stu-id="5b41f-179">Int32</span></span>|<span data-ttu-id="5b41f-180">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="5b41f-180">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="5b41f-181">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="5b41f-181">Valid values 0 to 24</span></span>|
|<span data-ttu-id="5b41f-182">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5b41f-182">osMinimumVersion</span></span>|<span data-ttu-id="5b41f-183">Строка</span><span class="sxs-lookup"><span data-stu-id="5b41f-183">String</span></span>|<span data-ttu-id="5b41f-184">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="5b41f-184">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="5b41f-185">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5b41f-185">osMaximumVersion</span></span>|<span data-ttu-id="5b41f-186">String</span><span class="sxs-lookup"><span data-stu-id="5b41f-186">String</span></span>|<span data-ttu-id="5b41f-187">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="5b41f-187">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="5b41f-188">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5b41f-188">storageRequireEncryption</span></span>|<span data-ttu-id="5b41f-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b41f-189">Boolean</span></span>|<span data-ttu-id="5b41f-190">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="5b41f-190">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="5b41f-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b41f-191">Response</span></span>
<span data-ttu-id="5b41f-192">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5b41f-192">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b41f-193">Пример</span><span class="sxs-lookup"><span data-stu-id="5b41f-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b41f-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b41f-194">Request</span></span>
<span data-ttu-id="5b41f-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b41f-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b41f-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b41f-196">Response</span></span>
<span data-ttu-id="5b41f-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b41f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




