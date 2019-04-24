---
title: Create windowsPhone81CompliancePolicy
description: Создание объекта windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a76bf59f81c390b1e486545c4f4e1de8ea8649c7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32513267"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="d4532-103">Create windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d4532-103">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="d4532-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4532-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4532-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4532-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4532-106">Создание объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d4532-106">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4532-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d4532-107">Prerequisites</span></span>
<span data-ttu-id="d4532-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4532-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4532-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4532-110">Permission type</span></span>|<span data-ttu-id="d4532-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4532-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4532-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4532-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4532-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4532-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4532-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4532-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4532-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4532-115">Not supported.</span></span>|
|<span data-ttu-id="d4532-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4532-116">Application</span></span>|<span data-ttu-id="d4532-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4532-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4532-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4532-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d4532-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4532-119">Request headers</span></span>
|<span data-ttu-id="d4532-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4532-120">Header</span></span>|<span data-ttu-id="d4532-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d4532-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4532-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4532-122">Authorization</span></span>|<span data-ttu-id="d4532-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4532-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4532-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d4532-124">Accept</span></span>|<span data-ttu-id="d4532-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4532-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4532-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4532-126">Request body</span></span>
<span data-ttu-id="d4532-127">В теле запроса добавьте представление объекта windowsPhone81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4532-127">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="d4532-128">Ниже показаны свойства, которые необходимо указывать при создании объекта windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d4532-128">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="d4532-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4532-129">Property</span></span>|<span data-ttu-id="d4532-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d4532-130">Type</span></span>|<span data-ttu-id="d4532-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d4532-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4532-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d4532-132">roleScopeTagIds</span></span>|<span data-ttu-id="d4532-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d4532-133">String collection</span></span>|<span data-ttu-id="d4532-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d4532-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d4532-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d4532-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4532-136">id</span><span class="sxs-lookup"><span data-stu-id="d4532-136">id</span></span>|<span data-ttu-id="d4532-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d4532-137">String</span></span>|<span data-ttu-id="d4532-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d4532-138">Key of the entity.</span></span> <span data-ttu-id="d4532-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d4532-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4532-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4532-140">createdDateTime</span></span>|<span data-ttu-id="d4532-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4532-141">DateTimeOffset</span></span>|<span data-ttu-id="d4532-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d4532-142">DateTime the object was created.</span></span> <span data-ttu-id="d4532-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d4532-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4532-144">description</span><span class="sxs-lookup"><span data-stu-id="d4532-144">description</span></span>|<span data-ttu-id="d4532-145">String</span><span class="sxs-lookup"><span data-stu-id="d4532-145">String</span></span>|<span data-ttu-id="d4532-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4532-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d4532-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d4532-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4532-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4532-148">lastModifiedDateTime</span></span>|<span data-ttu-id="d4532-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4532-149">DateTimeOffset</span></span>|<span data-ttu-id="d4532-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d4532-150">DateTime the object was last modified.</span></span> <span data-ttu-id="d4532-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d4532-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4532-152">displayName</span><span class="sxs-lookup"><span data-stu-id="d4532-152">displayName</span></span>|<span data-ttu-id="d4532-153">Строка</span><span class="sxs-lookup"><span data-stu-id="d4532-153">String</span></span>|<span data-ttu-id="d4532-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4532-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d4532-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d4532-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4532-156">version</span><span class="sxs-lookup"><span data-stu-id="d4532-156">version</span></span>|<span data-ttu-id="d4532-157">Int32</span><span class="sxs-lookup"><span data-stu-id="d4532-157">Int32</span></span>|<span data-ttu-id="d4532-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4532-158">Version of the device configuration.</span></span> <span data-ttu-id="d4532-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d4532-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d4532-160">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d4532-160">passwordBlockSimple</span></span>|<span data-ttu-id="d4532-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4532-161">Boolean</span></span>|<span data-ttu-id="d4532-162">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="d4532-162">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="d4532-163">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d4532-163">passwordExpirationDays</span></span>|<span data-ttu-id="d4532-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d4532-164">Int32</span></span>|<span data-ttu-id="d4532-165">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="d4532-165">Number of days before the password expires.</span></span>|
|<span data-ttu-id="d4532-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d4532-166">passwordMinimumLength</span></span>|<span data-ttu-id="d4532-167">Int32</span><span class="sxs-lookup"><span data-stu-id="d4532-167">Int32</span></span>|<span data-ttu-id="d4532-168">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="d4532-168">Minimum length of passwords.</span></span>|
|<span data-ttu-id="d4532-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d4532-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d4532-170">Int32</span><span class="sxs-lookup"><span data-stu-id="d4532-170">Int32</span></span>|<span data-ttu-id="d4532-171">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="d4532-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="d4532-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d4532-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="d4532-173">Int32</span><span class="sxs-lookup"><span data-stu-id="d4532-173">Int32</span></span>|<span data-ttu-id="d4532-174">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="d4532-174">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="d4532-175">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d4532-175">passwordRequiredType</span></span>|[<span data-ttu-id="d4532-176">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="d4532-176">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d4532-177">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="d4532-177">The required password type.</span></span> <span data-ttu-id="d4532-178">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d4532-178">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d4532-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d4532-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d4532-180">Int32</span><span class="sxs-lookup"><span data-stu-id="d4532-180">Int32</span></span>|<span data-ttu-id="d4532-181">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="d4532-181">Number of previous passwords to block.</span></span> <span data-ttu-id="d4532-182">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="d4532-182">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d4532-183">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d4532-183">passwordRequired</span></span>|<span data-ttu-id="d4532-184">Логический</span><span class="sxs-lookup"><span data-stu-id="d4532-184">Boolean</span></span>|<span data-ttu-id="d4532-185">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="d4532-185">Whether or not to require a password.</span></span>|
|<span data-ttu-id="d4532-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d4532-186">osMinimumVersion</span></span>|<span data-ttu-id="d4532-187">String</span><span class="sxs-lookup"><span data-stu-id="d4532-187">String</span></span>|<span data-ttu-id="d4532-188">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="d4532-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="d4532-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d4532-189">osMaximumVersion</span></span>|<span data-ttu-id="d4532-190">String</span><span class="sxs-lookup"><span data-stu-id="d4532-190">String</span></span>|<span data-ttu-id="d4532-191">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="d4532-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="d4532-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="d4532-192">storageRequireEncryption</span></span>|<span data-ttu-id="d4532-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4532-193">Boolean</span></span>|<span data-ttu-id="d4532-194">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="d4532-194">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="d4532-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4532-195">Response</span></span>
<span data-ttu-id="d4532-196">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d4532-196">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4532-197">Пример</span><span class="sxs-lookup"><span data-stu-id="d4532-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4532-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4532-198">Request</span></span>
<span data-ttu-id="d4532-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4532-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4532-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4532-200">Response</span></span>
<span data-ttu-id="d4532-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4532-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





