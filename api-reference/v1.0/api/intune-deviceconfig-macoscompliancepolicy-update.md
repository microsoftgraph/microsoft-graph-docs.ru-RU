---
title: Update macOSCompliancePolicy
description: Обновление свойств объекта macOSCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 922b63ba99ae17505e36a861c6d12a4b6a195c8c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549862"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="b92f1-103">Update macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b92f1-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="b92f1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b92f1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b92f1-105">Обновление свойств объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b92f1-105">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b92f1-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b92f1-106">Prerequisites</span></span>
<span data-ttu-id="b92f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b92f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b92f1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b92f1-109">Permission type</span></span>|<span data-ttu-id="b92f1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b92f1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b92f1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b92f1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b92f1-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b92f1-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b92f1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b92f1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b92f1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b92f1-114">Not supported.</span></span>|
|<span data-ttu-id="b92f1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b92f1-115">Application</span></span>|<span data-ttu-id="b92f1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b92f1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b92f1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b92f1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b92f1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b92f1-118">Request headers</span></span>
|<span data-ttu-id="b92f1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b92f1-119">Header</span></span>|<span data-ttu-id="b92f1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b92f1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b92f1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b92f1-121">Authorization</span></span>|<span data-ttu-id="b92f1-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b92f1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b92f1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b92f1-123">Accept</span></span>|<span data-ttu-id="b92f1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b92f1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b92f1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b92f1-125">Request body</span></span>
<span data-ttu-id="b92f1-126">В теле запроса добавьте представление объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b92f1-126">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="b92f1-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b92f1-127">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="b92f1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b92f1-128">Property</span></span>|<span data-ttu-id="b92f1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b92f1-129">Type</span></span>|<span data-ttu-id="b92f1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b92f1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b92f1-131">id</span><span class="sxs-lookup"><span data-stu-id="b92f1-131">id</span></span>|<span data-ttu-id="b92f1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b92f1-132">String</span></span>|<span data-ttu-id="b92f1-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b92f1-133">Key of the entity.</span></span> <span data-ttu-id="b92f1-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b92f1-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b92f1-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b92f1-135">createdDateTime</span></span>|<span data-ttu-id="b92f1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b92f1-136">DateTimeOffset</span></span>|<span data-ttu-id="b92f1-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b92f1-137">DateTime the object was created.</span></span> <span data-ttu-id="b92f1-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b92f1-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b92f1-139">description</span><span class="sxs-lookup"><span data-stu-id="b92f1-139">description</span></span>|<span data-ttu-id="b92f1-140">String</span><span class="sxs-lookup"><span data-stu-id="b92f1-140">String</span></span>|<span data-ttu-id="b92f1-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b92f1-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b92f1-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b92f1-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b92f1-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b92f1-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b92f1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b92f1-144">DateTimeOffset</span></span>|<span data-ttu-id="b92f1-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b92f1-145">DateTime the object was last modified.</span></span> <span data-ttu-id="b92f1-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b92f1-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b92f1-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b92f1-147">displayName</span></span>|<span data-ttu-id="b92f1-148">Строка</span><span class="sxs-lookup"><span data-stu-id="b92f1-148">String</span></span>|<span data-ttu-id="b92f1-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b92f1-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b92f1-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b92f1-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b92f1-151">version</span><span class="sxs-lookup"><span data-stu-id="b92f1-151">version</span></span>|<span data-ttu-id="b92f1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b92f1-152">Int32</span></span>|<span data-ttu-id="b92f1-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b92f1-153">Version of the device configuration.</span></span> <span data-ttu-id="b92f1-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b92f1-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b92f1-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b92f1-155">passwordRequired</span></span>|<span data-ttu-id="b92f1-156">Логический</span><span class="sxs-lookup"><span data-stu-id="b92f1-156">Boolean</span></span>|<span data-ttu-id="b92f1-157">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="b92f1-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="b92f1-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b92f1-158">passwordBlockSimple</span></span>|<span data-ttu-id="b92f1-159">Логический</span><span class="sxs-lookup"><span data-stu-id="b92f1-159">Boolean</span></span>|<span data-ttu-id="b92f1-160">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="b92f1-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="b92f1-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b92f1-161">passwordExpirationDays</span></span>|<span data-ttu-id="b92f1-162">Int32</span><span class="sxs-lookup"><span data-stu-id="b92f1-162">Int32</span></span>|<span data-ttu-id="b92f1-163">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="b92f1-163">Number of days before the password expires.</span></span> <span data-ttu-id="b92f1-164">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="b92f1-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b92f1-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b92f1-165">passwordMinimumLength</span></span>|<span data-ttu-id="b92f1-166">Int32</span><span class="sxs-lookup"><span data-stu-id="b92f1-166">Int32</span></span>|<span data-ttu-id="b92f1-167">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="b92f1-167">Minimum length of password.</span></span> <span data-ttu-id="b92f1-168">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="b92f1-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="b92f1-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b92f1-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b92f1-170">Int32</span><span class="sxs-lookup"><span data-stu-id="b92f1-170">Int32</span></span>|<span data-ttu-id="b92f1-171">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="b92f1-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b92f1-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b92f1-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b92f1-173">Int32</span><span class="sxs-lookup"><span data-stu-id="b92f1-173">Int32</span></span>|<span data-ttu-id="b92f1-174">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="b92f1-174">Number of previous passwords to block.</span></span> <span data-ttu-id="b92f1-175">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="b92f1-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b92f1-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b92f1-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b92f1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b92f1-177">Int32</span></span>|<span data-ttu-id="b92f1-178">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="b92f1-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b92f1-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b92f1-179">passwordRequiredType</span></span>|[<span data-ttu-id="b92f1-180">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="b92f1-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b92f1-181">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="b92f1-181">The required password type.</span></span> <span data-ttu-id="b92f1-182">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b92f1-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b92f1-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b92f1-183">osMinimumVersion</span></span>|<span data-ttu-id="b92f1-184">String</span><span class="sxs-lookup"><span data-stu-id="b92f1-184">String</span></span>|<span data-ttu-id="b92f1-185">Минимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="b92f1-185">Minimum MacOS version.</span></span>|
|<span data-ttu-id="b92f1-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b92f1-186">osMaximumVersion</span></span>|<span data-ttu-id="b92f1-187">String</span><span class="sxs-lookup"><span data-stu-id="b92f1-187">String</span></span>|<span data-ttu-id="b92f1-188">Максимальная версия MacOS.</span><span class="sxs-lookup"><span data-stu-id="b92f1-188">Maximum MacOS version.</span></span>|
|<span data-ttu-id="b92f1-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b92f1-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="b92f1-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="b92f1-190">Boolean</span></span>|<span data-ttu-id="b92f1-191">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="b92f1-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="b92f1-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b92f1-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b92f1-193">Логический</span><span class="sxs-lookup"><span data-stu-id="b92f1-193">Boolean</span></span>|<span data-ttu-id="b92f1-194">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="b92f1-194">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="b92f1-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b92f1-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b92f1-196">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="b92f1-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b92f1-197">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="b92f1-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b92f1-198">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b92f1-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b92f1-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b92f1-199">storageRequireEncryption</span></span>|<span data-ttu-id="b92f1-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="b92f1-200">Boolean</span></span>|<span data-ttu-id="b92f1-201">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="b92f1-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="b92f1-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="b92f1-202">firewallEnabled</span></span>|<span data-ttu-id="b92f1-203">Логический</span><span class="sxs-lookup"><span data-stu-id="b92f1-203">Boolean</span></span>|<span data-ttu-id="b92f1-204">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="b92f1-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="b92f1-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="b92f1-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="b92f1-206">Логический</span><span class="sxs-lookup"><span data-stu-id="b92f1-206">Boolean</span></span>|<span data-ttu-id="b92f1-207">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="b92f1-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="b92f1-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="b92f1-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="b92f1-209">Логический</span><span class="sxs-lookup"><span data-stu-id="b92f1-209">Boolean</span></span>|<span data-ttu-id="b92f1-210">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="b92f1-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="b92f1-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="b92f1-211">Response</span></span>
<span data-ttu-id="b92f1-212">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b92f1-212">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b92f1-213">Пример</span><span class="sxs-lookup"><span data-stu-id="b92f1-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="b92f1-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="b92f1-214">Request</span></span>
<span data-ttu-id="b92f1-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b92f1-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b92f1-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="b92f1-216">Response</span></span>
<span data-ttu-id="b92f1-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b92f1-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



