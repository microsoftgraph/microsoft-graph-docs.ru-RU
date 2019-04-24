---
title: Update windows81CompliancePolicy
description: Обновление свойств объекта windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c9248ac5e09c5149bf408728ac5bc7cd4cd7ba8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32515472"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="08e6c-103">Update windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="08e6c-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="08e6c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08e6c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08e6c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08e6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08e6c-106">Обновление свойств объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08e6c-106">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08e6c-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="08e6c-107">Prerequisites</span></span>
<span data-ttu-id="08e6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08e6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08e6c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08e6c-110">Permission type</span></span>|<span data-ttu-id="08e6c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08e6c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08e6c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08e6c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08e6c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08e6c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08e6c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08e6c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08e6c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08e6c-115">Not supported.</span></span>|
|<span data-ttu-id="08e6c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08e6c-116">Application</span></span>|<span data-ttu-id="08e6c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08e6c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08e6c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08e6c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="08e6c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08e6c-119">Request headers</span></span>
|<span data-ttu-id="08e6c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08e6c-120">Header</span></span>|<span data-ttu-id="08e6c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="08e6c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08e6c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08e6c-122">Authorization</span></span>|<span data-ttu-id="08e6c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08e6c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08e6c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="08e6c-124">Accept</span></span>|<span data-ttu-id="08e6c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08e6c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08e6c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08e6c-126">Request body</span></span>
<span data-ttu-id="08e6c-127">В теле запроса добавьте представление объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08e6c-127">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="08e6c-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08e6c-128">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="08e6c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="08e6c-129">Property</span></span>|<span data-ttu-id="08e6c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="08e6c-130">Type</span></span>|<span data-ttu-id="08e6c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="08e6c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08e6c-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08e6c-132">roleScopeTagIds</span></span>|<span data-ttu-id="08e6c-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="08e6c-133">String collection</span></span>|<span data-ttu-id="08e6c-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="08e6c-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="08e6c-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08e6c-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08e6c-136">id</span><span class="sxs-lookup"><span data-stu-id="08e6c-136">id</span></span>|<span data-ttu-id="08e6c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="08e6c-137">String</span></span>|<span data-ttu-id="08e6c-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="08e6c-138">Key of the entity.</span></span> <span data-ttu-id="08e6c-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08e6c-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08e6c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08e6c-140">createdDateTime</span></span>|<span data-ttu-id="08e6c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08e6c-141">DateTimeOffset</span></span>|<span data-ttu-id="08e6c-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="08e6c-142">DateTime the object was created.</span></span> <span data-ttu-id="08e6c-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08e6c-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08e6c-144">description</span><span class="sxs-lookup"><span data-stu-id="08e6c-144">description</span></span>|<span data-ttu-id="08e6c-145">String</span><span class="sxs-lookup"><span data-stu-id="08e6c-145">String</span></span>|<span data-ttu-id="08e6c-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08e6c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="08e6c-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08e6c-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08e6c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08e6c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="08e6c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08e6c-149">DateTimeOffset</span></span>|<span data-ttu-id="08e6c-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="08e6c-150">DateTime the object was last modified.</span></span> <span data-ttu-id="08e6c-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08e6c-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08e6c-152">displayName</span><span class="sxs-lookup"><span data-stu-id="08e6c-152">displayName</span></span>|<span data-ttu-id="08e6c-153">Строка</span><span class="sxs-lookup"><span data-stu-id="08e6c-153">String</span></span>|<span data-ttu-id="08e6c-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08e6c-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="08e6c-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08e6c-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08e6c-156">version</span><span class="sxs-lookup"><span data-stu-id="08e6c-156">version</span></span>|<span data-ttu-id="08e6c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="08e6c-157">Int32</span></span>|<span data-ttu-id="08e6c-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08e6c-158">Version of the device configuration.</span></span> <span data-ttu-id="08e6c-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08e6c-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="08e6c-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="08e6c-160">passwordRequired</span></span>|<span data-ttu-id="08e6c-161">Логический</span><span class="sxs-lookup"><span data-stu-id="08e6c-161">Boolean</span></span>|<span data-ttu-id="08e6c-162">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="08e6c-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="08e6c-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="08e6c-163">passwordBlockSimple</span></span>|<span data-ttu-id="08e6c-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="08e6c-164">Boolean</span></span>|<span data-ttu-id="08e6c-165">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="08e6c-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="08e6c-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="08e6c-166">passwordExpirationDays</span></span>|<span data-ttu-id="08e6c-167">Int32</span><span class="sxs-lookup"><span data-stu-id="08e6c-167">Int32</span></span>|<span data-ttu-id="08e6c-168">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="08e6c-168">Password expiration in days.</span></span>|
|<span data-ttu-id="08e6c-169">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="08e6c-169">passwordMinimumLength</span></span>|<span data-ttu-id="08e6c-170">Int32</span><span class="sxs-lookup"><span data-stu-id="08e6c-170">Int32</span></span>|<span data-ttu-id="08e6c-171">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="08e6c-171">The minimum password length.</span></span>|
|<span data-ttu-id="08e6c-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="08e6c-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="08e6c-173">Int32</span><span class="sxs-lookup"><span data-stu-id="08e6c-173">Int32</span></span>|<span data-ttu-id="08e6c-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="08e6c-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="08e6c-175">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="08e6c-175">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="08e6c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="08e6c-176">Int32</span></span>|<span data-ttu-id="08e6c-177">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="08e6c-177">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="08e6c-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="08e6c-178">passwordRequiredType</span></span>|[<span data-ttu-id="08e6c-179">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="08e6c-179">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="08e6c-180">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="08e6c-180">The required password type.</span></span> <span data-ttu-id="08e6c-181">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="08e6c-181">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="08e6c-182">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="08e6c-182">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="08e6c-183">Int32</span><span class="sxs-lookup"><span data-stu-id="08e6c-183">Int32</span></span>|<span data-ttu-id="08e6c-184">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="08e6c-184">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="08e6c-185">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="08e6c-185">Valid values 0 to 24</span></span>|
|<span data-ttu-id="08e6c-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="08e6c-186">osMinimumVersion</span></span>|<span data-ttu-id="08e6c-187">String</span><span class="sxs-lookup"><span data-stu-id="08e6c-187">String</span></span>|<span data-ttu-id="08e6c-188">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="08e6c-188">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="08e6c-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="08e6c-189">osMaximumVersion</span></span>|<span data-ttu-id="08e6c-190">String</span><span class="sxs-lookup"><span data-stu-id="08e6c-190">String</span></span>|<span data-ttu-id="08e6c-191">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="08e6c-191">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="08e6c-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="08e6c-192">storageRequireEncryption</span></span>|<span data-ttu-id="08e6c-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="08e6c-193">Boolean</span></span>|<span data-ttu-id="08e6c-194">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="08e6c-194">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="08e6c-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="08e6c-195">Response</span></span>
<span data-ttu-id="08e6c-196">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="08e6c-196">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08e6c-197">Пример</span><span class="sxs-lookup"><span data-stu-id="08e6c-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="08e6c-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="08e6c-198">Request</span></span>
<span data-ttu-id="08e6c-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08e6c-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 664

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="08e6c-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="08e6c-200">Response</span></span>
<span data-ttu-id="08e6c-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08e6c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 836

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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





