---
title: Create windowsPhone81CompliancePolicy
description: Создание объекта windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8da9dce6a274a9119a526ee9859ee8fb02ea48b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132305"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="3c999-103">Create windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3c999-103">Create windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="3c999-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c999-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c999-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c999-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c999-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c999-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c999-107">Создание объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3c999-107">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c999-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3c999-108">Prerequisites</span></span>
<span data-ttu-id="3c999-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c999-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c999-111">Permission type</span></span>|<span data-ttu-id="3c999-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c999-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c999-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c999-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c999-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c999-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c999-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c999-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c999-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c999-116">Not supported.</span></span>|
|<span data-ttu-id="3c999-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3c999-117">Application</span></span>|<span data-ttu-id="3c999-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c999-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c999-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c999-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3c999-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3c999-120">Request headers</span></span>
|<span data-ttu-id="3c999-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c999-121">Header</span></span>|<span data-ttu-id="3c999-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3c999-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c999-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c999-123">Authorization</span></span>|<span data-ttu-id="3c999-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c999-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c999-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3c999-125">Accept</span></span>|<span data-ttu-id="3c999-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c999-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c999-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c999-127">Request body</span></span>
<span data-ttu-id="3c999-128">В теле запроса добавьте представление объекта windowsPhone81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c999-128">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="3c999-129">Ниже показаны свойства, которые необходимо указывать при создании объекта windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="3c999-129">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="3c999-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c999-130">Property</span></span>|<span data-ttu-id="3c999-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3c999-131">Type</span></span>|<span data-ttu-id="3c999-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3c999-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c999-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3c999-133">roleScopeTagIds</span></span>|<span data-ttu-id="3c999-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3c999-134">String collection</span></span>|<span data-ttu-id="3c999-135">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="3c999-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3c999-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3c999-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3c999-137">id</span><span class="sxs-lookup"><span data-stu-id="3c999-137">id</span></span>|<span data-ttu-id="3c999-138">Строка</span><span class="sxs-lookup"><span data-stu-id="3c999-138">String</span></span>|<span data-ttu-id="3c999-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3c999-139">Key of the entity.</span></span> <span data-ttu-id="3c999-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3c999-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3c999-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c999-141">createdDateTime</span></span>|<span data-ttu-id="3c999-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c999-142">DateTimeOffset</span></span>|<span data-ttu-id="3c999-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3c999-143">DateTime the object was created.</span></span> <span data-ttu-id="3c999-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3c999-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3c999-145">description</span><span class="sxs-lookup"><span data-stu-id="3c999-145">description</span></span>|<span data-ttu-id="3c999-146">Строка</span><span class="sxs-lookup"><span data-stu-id="3c999-146">String</span></span>|<span data-ttu-id="3c999-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c999-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3c999-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3c999-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3c999-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c999-149">lastModifiedDateTime</span></span>|<span data-ttu-id="3c999-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c999-150">DateTimeOffset</span></span>|<span data-ttu-id="3c999-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3c999-151">DateTime the object was last modified.</span></span> <span data-ttu-id="3c999-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3c999-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3c999-153">displayName</span><span class="sxs-lookup"><span data-stu-id="3c999-153">displayName</span></span>|<span data-ttu-id="3c999-154">Строка</span><span class="sxs-lookup"><span data-stu-id="3c999-154">String</span></span>|<span data-ttu-id="3c999-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c999-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3c999-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3c999-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3c999-157">version</span><span class="sxs-lookup"><span data-stu-id="3c999-157">version</span></span>|<span data-ttu-id="3c999-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3c999-158">Int32</span></span>|<span data-ttu-id="3c999-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c999-159">Version of the device configuration.</span></span> <span data-ttu-id="3c999-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3c999-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3c999-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3c999-161">passwordBlockSimple</span></span>|<span data-ttu-id="3c999-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c999-162">Boolean</span></span>|<span data-ttu-id="3c999-163">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="3c999-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="3c999-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3c999-164">passwordExpirationDays</span></span>|<span data-ttu-id="3c999-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3c999-165">Int32</span></span>|<span data-ttu-id="3c999-166">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="3c999-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="3c999-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3c999-167">passwordMinimumLength</span></span>|<span data-ttu-id="3c999-168">Int32</span><span class="sxs-lookup"><span data-stu-id="3c999-168">Int32</span></span>|<span data-ttu-id="3c999-169">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="3c999-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="3c999-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3c999-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3c999-171">Int32</span><span class="sxs-lookup"><span data-stu-id="3c999-171">Int32</span></span>|<span data-ttu-id="3c999-172">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="3c999-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="3c999-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3c999-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3c999-174">Int32</span><span class="sxs-lookup"><span data-stu-id="3c999-174">Int32</span></span>|<span data-ttu-id="3c999-175">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="3c999-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3c999-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3c999-176">passwordRequiredType</span></span>|[<span data-ttu-id="3c999-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3c999-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3c999-178">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="3c999-178">The required password type.</span></span> <span data-ttu-id="3c999-179">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3c999-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3c999-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3c999-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3c999-181">Int32</span><span class="sxs-lookup"><span data-stu-id="3c999-181">Int32</span></span>|<span data-ttu-id="3c999-182">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="3c999-182">Number of previous passwords to block.</span></span> <span data-ttu-id="3c999-183">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="3c999-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3c999-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3c999-184">passwordRequired</span></span>|<span data-ttu-id="3c999-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c999-185">Boolean</span></span>|<span data-ttu-id="3c999-186">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="3c999-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="3c999-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3c999-187">osMinimumVersion</span></span>|<span data-ttu-id="3c999-188">String</span><span class="sxs-lookup"><span data-stu-id="3c999-188">String</span></span>|<span data-ttu-id="3c999-189">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="3c999-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="3c999-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3c999-190">osMaximumVersion</span></span>|<span data-ttu-id="3c999-191">String</span><span class="sxs-lookup"><span data-stu-id="3c999-191">String</span></span>|<span data-ttu-id="3c999-192">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="3c999-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="3c999-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3c999-193">storageRequireEncryption</span></span>|<span data-ttu-id="3c999-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c999-194">Boolean</span></span>|<span data-ttu-id="3c999-195">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="3c999-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="3c999-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c999-196">Response</span></span>
<span data-ttu-id="3c999-197">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3c999-197">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c999-198">Пример</span><span class="sxs-lookup"><span data-stu-id="3c999-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c999-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c999-199">Request</span></span>
<span data-ttu-id="3c999-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c999-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 669

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="3c999-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c999-201">Response</span></span>
<span data-ttu-id="3c999-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c999-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 841

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




