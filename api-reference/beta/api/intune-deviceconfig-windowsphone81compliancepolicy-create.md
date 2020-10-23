---
title: Create windowsPhone81CompliancePolicy
description: Создание объекта windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 733d19453b7404e107093f7d02f565adcfbdf7f7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704170"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="c770f-103">Create windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c770f-103">Create windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="c770f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c770f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c770f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c770f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c770f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c770f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c770f-107">Создание объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c770f-107">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c770f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c770f-108">Prerequisites</span></span>
<span data-ttu-id="c770f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c770f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c770f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c770f-111">Permission type</span></span>|<span data-ttu-id="c770f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c770f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c770f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c770f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c770f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c770f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c770f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c770f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c770f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c770f-116">Not supported.</span></span>|
|<span data-ttu-id="c770f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c770f-117">Application</span></span>|<span data-ttu-id="c770f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c770f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c770f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c770f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c770f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c770f-120">Request headers</span></span>
|<span data-ttu-id="c770f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c770f-121">Header</span></span>|<span data-ttu-id="c770f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c770f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c770f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c770f-123">Authorization</span></span>|<span data-ttu-id="c770f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c770f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c770f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c770f-125">Accept</span></span>|<span data-ttu-id="c770f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c770f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c770f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c770f-127">Request body</span></span>
<span data-ttu-id="c770f-128">В теле запроса добавьте представление объекта windowsPhone81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c770f-128">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="c770f-129">Ниже показаны свойства, которые необходимо указывать при создании объекта windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="c770f-129">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="c770f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c770f-130">Property</span></span>|<span data-ttu-id="c770f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c770f-131">Type</span></span>|<span data-ttu-id="c770f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c770f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c770f-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c770f-133">roleScopeTagIds</span></span>|<span data-ttu-id="c770f-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c770f-134">String collection</span></span>|<span data-ttu-id="c770f-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c770f-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c770f-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c770f-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c770f-137">id</span><span class="sxs-lookup"><span data-stu-id="c770f-137">id</span></span>|<span data-ttu-id="c770f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c770f-138">String</span></span>|<span data-ttu-id="c770f-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c770f-139">Key of the entity.</span></span> <span data-ttu-id="c770f-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c770f-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c770f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c770f-141">createdDateTime</span></span>|<span data-ttu-id="c770f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c770f-142">DateTimeOffset</span></span>|<span data-ttu-id="c770f-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c770f-143">DateTime the object was created.</span></span> <span data-ttu-id="c770f-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c770f-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c770f-145">description</span><span class="sxs-lookup"><span data-stu-id="c770f-145">description</span></span>|<span data-ttu-id="c770f-146">Строка</span><span class="sxs-lookup"><span data-stu-id="c770f-146">String</span></span>|<span data-ttu-id="c770f-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c770f-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c770f-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c770f-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c770f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c770f-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c770f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c770f-150">DateTimeOffset</span></span>|<span data-ttu-id="c770f-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c770f-151">DateTime the object was last modified.</span></span> <span data-ttu-id="c770f-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c770f-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c770f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c770f-153">displayName</span></span>|<span data-ttu-id="c770f-154">Строка</span><span class="sxs-lookup"><span data-stu-id="c770f-154">String</span></span>|<span data-ttu-id="c770f-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c770f-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c770f-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c770f-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c770f-157">version</span><span class="sxs-lookup"><span data-stu-id="c770f-157">version</span></span>|<span data-ttu-id="c770f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c770f-158">Int32</span></span>|<span data-ttu-id="c770f-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c770f-159">Version of the device configuration.</span></span> <span data-ttu-id="c770f-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c770f-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c770f-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c770f-161">passwordBlockSimple</span></span>|<span data-ttu-id="c770f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c770f-162">Boolean</span></span>|<span data-ttu-id="c770f-163">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="c770f-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="c770f-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c770f-164">passwordExpirationDays</span></span>|<span data-ttu-id="c770f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c770f-165">Int32</span></span>|<span data-ttu-id="c770f-166">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c770f-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="c770f-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c770f-167">passwordMinimumLength</span></span>|<span data-ttu-id="c770f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c770f-168">Int32</span></span>|<span data-ttu-id="c770f-169">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="c770f-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="c770f-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c770f-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c770f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="c770f-171">Int32</span></span>|<span data-ttu-id="c770f-172">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c770f-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c770f-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c770f-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c770f-174">Int32</span><span class="sxs-lookup"><span data-stu-id="c770f-174">Int32</span></span>|<span data-ttu-id="c770f-175">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="c770f-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c770f-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c770f-176">passwordRequiredType</span></span>|[<span data-ttu-id="c770f-177">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c770f-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c770f-178">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c770f-178">The required password type.</span></span> <span data-ttu-id="c770f-179">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="c770f-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c770f-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c770f-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c770f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="c770f-181">Int32</span></span>|<span data-ttu-id="c770f-182">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="c770f-182">Number of previous passwords to block.</span></span> <span data-ttu-id="c770f-183">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="c770f-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c770f-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c770f-184">passwordRequired</span></span>|<span data-ttu-id="c770f-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="c770f-185">Boolean</span></span>|<span data-ttu-id="c770f-186">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c770f-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="c770f-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c770f-187">osMinimumVersion</span></span>|<span data-ttu-id="c770f-188">String</span><span class="sxs-lookup"><span data-stu-id="c770f-188">String</span></span>|<span data-ttu-id="c770f-189">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="c770f-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="c770f-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c770f-190">osMaximumVersion</span></span>|<span data-ttu-id="c770f-191">String</span><span class="sxs-lookup"><span data-stu-id="c770f-191">String</span></span>|<span data-ttu-id="c770f-192">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="c770f-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="c770f-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c770f-193">storageRequireEncryption</span></span>|<span data-ttu-id="c770f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c770f-194">Boolean</span></span>|<span data-ttu-id="c770f-195">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="c770f-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="c770f-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="c770f-196">Response</span></span>
<span data-ttu-id="c770f-197">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c770f-197">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c770f-198">Пример</span><span class="sxs-lookup"><span data-stu-id="c770f-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="c770f-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="c770f-199">Request</span></span>
<span data-ttu-id="c770f-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c770f-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c770f-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="c770f-201">Response</span></span>
<span data-ttu-id="c770f-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c770f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





