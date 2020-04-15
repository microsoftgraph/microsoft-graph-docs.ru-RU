---
title: Update macOSCompliancePolicy
description: Обновление свойств объекта macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea216de2f7bf9b7709e120c529db255389395fb4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468853"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="6e218-103">Update macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6e218-103">Update macOSCompliancePolicy</span></span>

<span data-ttu-id="6e218-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e218-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e218-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e218-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e218-106">Обновление свойств объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e218-106">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e218-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6e218-107">Prerequisites</span></span>
<span data-ttu-id="6e218-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e218-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e218-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e218-110">Permission type</span></span>|<span data-ttu-id="6e218-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e218-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e218-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e218-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e218-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e218-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e218-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e218-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e218-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e218-115">Not supported.</span></span>|
|<span data-ttu-id="6e218-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e218-116">Application</span></span>|<span data-ttu-id="6e218-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e218-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e218-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e218-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6e218-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6e218-119">Request headers</span></span>
|<span data-ttu-id="6e218-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e218-120">Header</span></span>|<span data-ttu-id="6e218-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6e218-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e218-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e218-122">Authorization</span></span>|<span data-ttu-id="6e218-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e218-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e218-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6e218-124">Accept</span></span>|<span data-ttu-id="6e218-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6e218-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e218-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6e218-126">Request body</span></span>
<span data-ttu-id="6e218-127">В теле запроса добавьте представление объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e218-127">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="6e218-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e218-128">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="6e218-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e218-129">Property</span></span>|<span data-ttu-id="6e218-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6e218-130">Type</span></span>|<span data-ttu-id="6e218-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6e218-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e218-132">id</span><span class="sxs-lookup"><span data-stu-id="6e218-132">id</span></span>|<span data-ttu-id="6e218-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6e218-133">String</span></span>|<span data-ttu-id="6e218-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6e218-134">Key of the entity.</span></span> <span data-ttu-id="6e218-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e218-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e218-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e218-136">createdDateTime</span></span>|<span data-ttu-id="6e218-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e218-137">DateTimeOffset</span></span>|<span data-ttu-id="6e218-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6e218-138">DateTime the object was created.</span></span> <span data-ttu-id="6e218-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e218-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e218-140">description</span><span class="sxs-lookup"><span data-stu-id="6e218-140">description</span></span>|<span data-ttu-id="6e218-141">String</span><span class="sxs-lookup"><span data-stu-id="6e218-141">String</span></span>|<span data-ttu-id="6e218-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e218-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e218-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e218-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e218-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e218-144">lastModifiedDateTime</span></span>|<span data-ttu-id="6e218-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e218-145">DateTimeOffset</span></span>|<span data-ttu-id="6e218-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6e218-146">DateTime the object was last modified.</span></span> <span data-ttu-id="6e218-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e218-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e218-148">displayName</span><span class="sxs-lookup"><span data-stu-id="6e218-148">displayName</span></span>|<span data-ttu-id="6e218-149">Строка</span><span class="sxs-lookup"><span data-stu-id="6e218-149">String</span></span>|<span data-ttu-id="6e218-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e218-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e218-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e218-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e218-152">version</span><span class="sxs-lookup"><span data-stu-id="6e218-152">version</span></span>|<span data-ttu-id="6e218-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6e218-153">Int32</span></span>|<span data-ttu-id="6e218-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e218-154">Version of the device configuration.</span></span> <span data-ttu-id="6e218-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e218-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e218-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6e218-156">passwordRequired</span></span>|<span data-ttu-id="6e218-157">Логический</span><span class="sxs-lookup"><span data-stu-id="6e218-157">Boolean</span></span>|<span data-ttu-id="6e218-158">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="6e218-158">Whether or not to require a password.</span></span>|
|<span data-ttu-id="6e218-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6e218-159">passwordBlockSimple</span></span>|<span data-ttu-id="6e218-160">Логический</span><span class="sxs-lookup"><span data-stu-id="6e218-160">Boolean</span></span>|<span data-ttu-id="6e218-161">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="6e218-161">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="6e218-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6e218-162">passwordExpirationDays</span></span>|<span data-ttu-id="6e218-163">Int32</span><span class="sxs-lookup"><span data-stu-id="6e218-163">Int32</span></span>|<span data-ttu-id="6e218-164">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="6e218-164">Number of days before the password expires.</span></span> <span data-ttu-id="6e218-165">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="6e218-165">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6e218-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6e218-166">passwordMinimumLength</span></span>|<span data-ttu-id="6e218-167">Int32</span><span class="sxs-lookup"><span data-stu-id="6e218-167">Int32</span></span>|<span data-ttu-id="6e218-168">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="6e218-168">Minimum length of password.</span></span> <span data-ttu-id="6e218-169">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="6e218-169">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6e218-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6e218-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6e218-171">Int32</span><span class="sxs-lookup"><span data-stu-id="6e218-171">Int32</span></span>|<span data-ttu-id="6e218-172">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="6e218-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6e218-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6e218-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6e218-174">Int32</span><span class="sxs-lookup"><span data-stu-id="6e218-174">Int32</span></span>|<span data-ttu-id="6e218-175">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="6e218-175">Number of previous passwords to block.</span></span> <span data-ttu-id="6e218-176">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="6e218-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6e218-177">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6e218-177">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6e218-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6e218-178">Int32</span></span>|<span data-ttu-id="6e218-179">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="6e218-179">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6e218-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6e218-180">passwordRequiredType</span></span>|[<span data-ttu-id="6e218-181">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="6e218-181">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6e218-182">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="6e218-182">The required password type.</span></span> <span data-ttu-id="6e218-183">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6e218-183">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6e218-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6e218-184">osMinimumVersion</span></span>|<span data-ttu-id="6e218-185">String</span><span class="sxs-lookup"><span data-stu-id="6e218-185">String</span></span>|<span data-ttu-id="6e218-186">Минимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="6e218-186">Minimum MacOS version.</span></span>|
|<span data-ttu-id="6e218-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6e218-187">osMaximumVersion</span></span>|<span data-ttu-id="6e218-188">String</span><span class="sxs-lookup"><span data-stu-id="6e218-188">String</span></span>|<span data-ttu-id="6e218-189">Максимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="6e218-189">Maximum MacOS version.</span></span>|
|<span data-ttu-id="6e218-190">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6e218-190">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="6e218-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e218-191">Boolean</span></span>|<span data-ttu-id="6e218-192">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="6e218-192">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="6e218-193">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6e218-193">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6e218-194">Логический</span><span class="sxs-lookup"><span data-stu-id="6e218-194">Boolean</span></span>|<span data-ttu-id="6e218-195">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="6e218-195">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="6e218-196">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6e218-196">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6e218-197">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="6e218-197">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6e218-198">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="6e218-198">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6e218-199">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6e218-199">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6e218-200">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6e218-200">storageRequireEncryption</span></span>|<span data-ttu-id="6e218-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e218-201">Boolean</span></span>|<span data-ttu-id="6e218-202">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="6e218-202">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="6e218-203">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="6e218-203">firewallEnabled</span></span>|<span data-ttu-id="6e218-204">Логический</span><span class="sxs-lookup"><span data-stu-id="6e218-204">Boolean</span></span>|<span data-ttu-id="6e218-205">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="6e218-205">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="6e218-206">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="6e218-206">firewallBlockAllIncoming</span></span>|<span data-ttu-id="6e218-207">Логический</span><span class="sxs-lookup"><span data-stu-id="6e218-207">Boolean</span></span>|<span data-ttu-id="6e218-208">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="6e218-208">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="6e218-209">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="6e218-209">firewallEnableStealthMode</span></span>|<span data-ttu-id="6e218-210">Логический</span><span class="sxs-lookup"><span data-stu-id="6e218-210">Boolean</span></span>|<span data-ttu-id="6e218-211">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="6e218-211">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="6e218-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e218-212">Response</span></span>
<span data-ttu-id="6e218-213">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6e218-213">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e218-214">Пример</span><span class="sxs-lookup"><span data-stu-id="6e218-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e218-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e218-215">Request</span></span>
<span data-ttu-id="6e218-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e218-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 849

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="6e218-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e218-217">Response</span></span>
<span data-ttu-id="6e218-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e218-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1021

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
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
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```






