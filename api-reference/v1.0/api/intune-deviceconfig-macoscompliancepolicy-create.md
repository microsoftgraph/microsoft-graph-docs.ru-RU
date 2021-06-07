---
title: Create macOSCompliancePolicy
description: Создание объекта macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 44476093dbcabe5db8a3bd6a8ea18673abd6ecab
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753855"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="bf97c-103">Create macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="bf97c-103">Create macOSCompliancePolicy</span></span>

<span data-ttu-id="bf97c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf97c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf97c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf97c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf97c-106">Создание объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bf97c-106">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf97c-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bf97c-107">Prerequisites</span></span>
<span data-ttu-id="bf97c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf97c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf97c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf97c-110">Permission type</span></span>|<span data-ttu-id="bf97c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf97c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf97c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf97c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf97c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf97c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf97c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf97c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf97c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf97c-115">Not supported.</span></span>|
|<span data-ttu-id="bf97c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bf97c-116">Application</span></span>|<span data-ttu-id="bf97c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf97c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf97c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf97c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="bf97c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bf97c-119">Request headers</span></span>
|<span data-ttu-id="bf97c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf97c-120">Header</span></span>|<span data-ttu-id="bf97c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bf97c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf97c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf97c-122">Authorization</span></span>|<span data-ttu-id="bf97c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf97c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf97c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bf97c-124">Accept</span></span>|<span data-ttu-id="bf97c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf97c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf97c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf97c-126">Request body</span></span>
<span data-ttu-id="bf97c-127">В теле запроса добавьте представление объекта macOSCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf97c-127">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="bf97c-128">Ниже показаны свойства, которые необходимо указывать при создании объекта macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="bf97c-128">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="bf97c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf97c-129">Property</span></span>|<span data-ttu-id="bf97c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bf97c-130">Type</span></span>|<span data-ttu-id="bf97c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bf97c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf97c-132">id</span><span class="sxs-lookup"><span data-stu-id="bf97c-132">id</span></span>|<span data-ttu-id="bf97c-133">String</span><span class="sxs-lookup"><span data-stu-id="bf97c-133">String</span></span>|<span data-ttu-id="bf97c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bf97c-134">Key of the entity.</span></span> <span data-ttu-id="bf97c-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bf97c-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf97c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf97c-136">createdDateTime</span></span>|<span data-ttu-id="bf97c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf97c-137">DateTimeOffset</span></span>|<span data-ttu-id="bf97c-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bf97c-138">DateTime the object was created.</span></span> <span data-ttu-id="bf97c-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bf97c-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf97c-140">description</span><span class="sxs-lookup"><span data-stu-id="bf97c-140">description</span></span>|<span data-ttu-id="bf97c-141">String</span><span class="sxs-lookup"><span data-stu-id="bf97c-141">String</span></span>|<span data-ttu-id="bf97c-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bf97c-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bf97c-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bf97c-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf97c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf97c-144">lastModifiedDateTime</span></span>|<span data-ttu-id="bf97c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf97c-145">DateTimeOffset</span></span>|<span data-ttu-id="bf97c-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bf97c-146">DateTime the object was last modified.</span></span> <span data-ttu-id="bf97c-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bf97c-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf97c-148">displayName</span><span class="sxs-lookup"><span data-stu-id="bf97c-148">displayName</span></span>|<span data-ttu-id="bf97c-149">String</span><span class="sxs-lookup"><span data-stu-id="bf97c-149">String</span></span>|<span data-ttu-id="bf97c-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bf97c-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bf97c-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bf97c-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf97c-152">version</span><span class="sxs-lookup"><span data-stu-id="bf97c-152">version</span></span>|<span data-ttu-id="bf97c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="bf97c-153">Int32</span></span>|<span data-ttu-id="bf97c-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bf97c-154">Version of the device configuration.</span></span> <span data-ttu-id="bf97c-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bf97c-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf97c-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bf97c-156">passwordRequired</span></span>|<span data-ttu-id="bf97c-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf97c-157">Boolean</span></span>|<span data-ttu-id="bf97c-158">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="bf97c-158">Whether or not to require a password.</span></span>|
|<span data-ttu-id="bf97c-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="bf97c-159">passwordBlockSimple</span></span>|<span data-ttu-id="bf97c-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf97c-160">Boolean</span></span>|<span data-ttu-id="bf97c-161">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="bf97c-161">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="bf97c-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bf97c-162">passwordExpirationDays</span></span>|<span data-ttu-id="bf97c-163">Int32</span><span class="sxs-lookup"><span data-stu-id="bf97c-163">Int32</span></span>|<span data-ttu-id="bf97c-164">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="bf97c-164">Number of days before the password expires.</span></span> <span data-ttu-id="bf97c-165">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="bf97c-165">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="bf97c-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bf97c-166">passwordMinimumLength</span></span>|<span data-ttu-id="bf97c-167">Int32</span><span class="sxs-lookup"><span data-stu-id="bf97c-167">Int32</span></span>|<span data-ttu-id="bf97c-168">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="bf97c-168">Minimum length of password.</span></span> <span data-ttu-id="bf97c-169">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="bf97c-169">Valid values 4 to 14</span></span>|
|<span data-ttu-id="bf97c-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bf97c-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bf97c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="bf97c-171">Int32</span></span>|<span data-ttu-id="bf97c-172">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="bf97c-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="bf97c-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bf97c-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bf97c-174">Int32</span><span class="sxs-lookup"><span data-stu-id="bf97c-174">Int32</span></span>|<span data-ttu-id="bf97c-175">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="bf97c-175">Number of previous passwords to block.</span></span> <span data-ttu-id="bf97c-176">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="bf97c-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="bf97c-177">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bf97c-177">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="bf97c-178">Int32</span><span class="sxs-lookup"><span data-stu-id="bf97c-178">Int32</span></span>|<span data-ttu-id="bf97c-179">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="bf97c-179">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="bf97c-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bf97c-180">passwordRequiredType</span></span>|[<span data-ttu-id="bf97c-181">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bf97c-181">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="bf97c-182">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="bf97c-182">The required password type.</span></span> <span data-ttu-id="bf97c-183">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="bf97c-183">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="bf97c-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bf97c-184">osMinimumVersion</span></span>|<span data-ttu-id="bf97c-185">String</span><span class="sxs-lookup"><span data-stu-id="bf97c-185">String</span></span>|<span data-ttu-id="bf97c-186">Минимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="bf97c-186">Minimum MacOS version.</span></span>|
|<span data-ttu-id="bf97c-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bf97c-187">osMaximumVersion</span></span>|<span data-ttu-id="bf97c-188">String</span><span class="sxs-lookup"><span data-stu-id="bf97c-188">String</span></span>|<span data-ttu-id="bf97c-189">Максимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="bf97c-189">Maximum MacOS version.</span></span>|
|<span data-ttu-id="bf97c-190">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="bf97c-190">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="bf97c-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf97c-191">Boolean</span></span>|<span data-ttu-id="bf97c-192">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="bf97c-192">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="bf97c-193">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="bf97c-193">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="bf97c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf97c-194">Boolean</span></span>|<span data-ttu-id="bf97c-195">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="bf97c-195">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="bf97c-196">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="bf97c-196">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="bf97c-197">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="bf97c-197">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="bf97c-198">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="bf97c-198">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="bf97c-199">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="bf97c-199">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="bf97c-200">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="bf97c-200">storageRequireEncryption</span></span>|<span data-ttu-id="bf97c-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf97c-201">Boolean</span></span>|<span data-ttu-id="bf97c-202">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="bf97c-202">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="bf97c-203">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="bf97c-203">firewallEnabled</span></span>|<span data-ttu-id="bf97c-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf97c-204">Boolean</span></span>|<span data-ttu-id="bf97c-205">Следует ли включить брандмауэр или нет.</span><span class="sxs-lookup"><span data-stu-id="bf97c-205">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="bf97c-206">брандмауэрBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="bf97c-206">firewallBlockAllIncoming</span></span>|<span data-ttu-id="bf97c-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf97c-207">Boolean</span></span>|<span data-ttu-id="bf97c-208">Соответствует параметру "Блокировка всех входящих подключений".</span><span class="sxs-lookup"><span data-stu-id="bf97c-208">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="bf97c-209">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="bf97c-209">firewallEnableStealthMode</span></span>|<span data-ttu-id="bf97c-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf97c-210">Boolean</span></span>|<span data-ttu-id="bf97c-211">Соответствует режиму "Включить режим стелс".</span><span class="sxs-lookup"><span data-stu-id="bf97c-211">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="bf97c-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf97c-212">Response</span></span>
<span data-ttu-id="bf97c-213">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bf97c-213">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf97c-214">Пример</span><span class="sxs-lookup"><span data-stu-id="bf97c-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf97c-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf97c-215">Request</span></span>
<span data-ttu-id="bf97c-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf97c-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="bf97c-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf97c-217">Response</span></span>
<span data-ttu-id="bf97c-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf97c-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




