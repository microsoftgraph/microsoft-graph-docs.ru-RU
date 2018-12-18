---
title: Update macOSCompliancePolicy
description: Обновление свойств объекта macOSCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 08b256fc12dcfd7d2d5e79f0dc0b277244214a2d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321065"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="4dbe9-103">Update macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4dbe9-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="4dbe9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4dbe9-105">Обновление свойств объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4dbe9-105">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4dbe9-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4dbe9-106">Prerequisites</span></span>
<span data-ttu-id="4dbe9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dbe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dbe9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dbe9-109">Permission type</span></span>|<span data-ttu-id="4dbe9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dbe9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dbe9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dbe9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4dbe9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dbe9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4dbe9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dbe9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dbe9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-114">Not supported.</span></span>|
|<span data-ttu-id="4dbe9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dbe9-115">Application</span></span>|<span data-ttu-id="4dbe9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dbe9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dbe9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4dbe9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4dbe9-118">Request headers</span></span>
|<span data-ttu-id="4dbe9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4dbe9-119">Header</span></span>|<span data-ttu-id="4dbe9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4dbe9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dbe9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4dbe9-121">Authorization</span></span>|<span data-ttu-id="4dbe9-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4dbe9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dbe9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4dbe9-123">Accept</span></span>|<span data-ttu-id="4dbe9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4dbe9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dbe9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4dbe9-125">Request body</span></span>
<span data-ttu-id="4dbe9-126">В теле запроса добавьте представление объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-126">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="4dbe9-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4dbe9-127">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="4dbe9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dbe9-128">Property</span></span>|<span data-ttu-id="4dbe9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4dbe9-129">Type</span></span>|<span data-ttu-id="4dbe9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4dbe9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dbe9-131">id</span><span class="sxs-lookup"><span data-stu-id="4dbe9-131">id</span></span>|<span data-ttu-id="4dbe9-132">Строка</span><span class="sxs-lookup"><span data-stu-id="4dbe9-132">String</span></span>|<span data-ttu-id="4dbe9-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-133">Key of the entity.</span></span> <span data-ttu-id="4dbe9-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4dbe9-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dbe9-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4dbe9-135">createdDateTime</span></span>|<span data-ttu-id="4dbe9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dbe9-136">DateTimeOffset</span></span>|<span data-ttu-id="4dbe9-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-137">DateTime the object was created.</span></span> <span data-ttu-id="4dbe9-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4dbe9-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dbe9-139">описание</span><span class="sxs-lookup"><span data-stu-id="4dbe9-139">description</span></span>|<span data-ttu-id="4dbe9-140">Строка</span><span class="sxs-lookup"><span data-stu-id="4dbe9-140">String</span></span>|<span data-ttu-id="4dbe9-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4dbe9-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4dbe9-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dbe9-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4dbe9-143">lastModifiedDateTime</span></span>|<span data-ttu-id="4dbe9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dbe9-144">DateTimeOffset</span></span>|<span data-ttu-id="4dbe9-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-145">DateTime the object was last modified.</span></span> <span data-ttu-id="4dbe9-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4dbe9-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dbe9-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4dbe9-147">displayName</span></span>|<span data-ttu-id="4dbe9-148">Строка</span><span class="sxs-lookup"><span data-stu-id="4dbe9-148">String</span></span>|<span data-ttu-id="4dbe9-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4dbe9-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4dbe9-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dbe9-151">version</span><span class="sxs-lookup"><span data-stu-id="4dbe9-151">version</span></span>|<span data-ttu-id="4dbe9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4dbe9-152">Int32</span></span>|<span data-ttu-id="4dbe9-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-153">Version of the device configuration.</span></span> <span data-ttu-id="4dbe9-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4dbe9-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dbe9-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4dbe9-155">passwordRequired</span></span>|<span data-ttu-id="4dbe9-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dbe9-156">Boolean</span></span>|<span data-ttu-id="4dbe9-157">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="4dbe9-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4dbe9-158">passwordBlockSimple</span></span>|<span data-ttu-id="4dbe9-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dbe9-159">Boolean</span></span>|<span data-ttu-id="4dbe9-160">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="4dbe9-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4dbe9-161">passwordExpirationDays</span></span>|<span data-ttu-id="4dbe9-162">Int32</span><span class="sxs-lookup"><span data-stu-id="4dbe9-162">Int32</span></span>|<span data-ttu-id="4dbe9-163">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-163">Number of days before the password expires.</span></span> <span data-ttu-id="4dbe9-164">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="4dbe9-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4dbe9-165">passwordMinimumLength</span></span>|<span data-ttu-id="4dbe9-166">Int32</span><span class="sxs-lookup"><span data-stu-id="4dbe9-166">Int32</span></span>|<span data-ttu-id="4dbe9-167">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-167">Minimum length of password.</span></span> <span data-ttu-id="4dbe9-168">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="4dbe9-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4dbe9-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4dbe9-170">Int32</span><span class="sxs-lookup"><span data-stu-id="4dbe9-170">Int32</span></span>|<span data-ttu-id="4dbe9-171">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4dbe9-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4dbe9-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4dbe9-173">Int32</span><span class="sxs-lookup"><span data-stu-id="4dbe9-173">Int32</span></span>|<span data-ttu-id="4dbe9-174">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-174">Number of previous passwords to block.</span></span> <span data-ttu-id="4dbe9-175">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="4dbe9-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4dbe9-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4dbe9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4dbe9-177">Int32</span></span>|<span data-ttu-id="4dbe9-178">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4dbe9-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4dbe9-179">passwordRequiredType</span></span>|[<span data-ttu-id="4dbe9-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4dbe9-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4dbe9-181">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-181">The required password type.</span></span> <span data-ttu-id="4dbe9-182">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4dbe9-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4dbe9-183">osMinimumVersion</span></span>|<span data-ttu-id="4dbe9-184">String</span><span class="sxs-lookup"><span data-stu-id="4dbe9-184">String</span></span>|<span data-ttu-id="4dbe9-185">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="4dbe9-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4dbe9-186">osMaximumVersion</span></span>|<span data-ttu-id="4dbe9-187">String</span><span class="sxs-lookup"><span data-stu-id="4dbe9-187">String</span></span>|<span data-ttu-id="4dbe9-188">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="4dbe9-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4dbe9-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="4dbe9-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dbe9-190">Boolean</span></span>|<span data-ttu-id="4dbe9-191">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="4dbe9-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4dbe9-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4dbe9-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dbe9-193">Boolean</span></span>|<span data-ttu-id="4dbe9-194">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="4dbe9-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4dbe9-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="4dbe9-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="4dbe9-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="4dbe9-197">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4dbe9-198">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4dbe9-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4dbe9-199">storageRequireEncryption</span></span>|<span data-ttu-id="4dbe9-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dbe9-200">Boolean</span></span>|<span data-ttu-id="4dbe9-201">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="4dbe9-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="4dbe9-202">firewallEnabled</span></span>|<span data-ttu-id="4dbe9-203">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-203">Boolean</span></span>|<span data-ttu-id="4dbe9-204">Является ли брандмауэра должна быть включена или нет.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="4dbe9-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="4dbe9-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="4dbe9-206">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-206">Boolean</span></span>|<span data-ttu-id="4dbe9-207">Соответствующий параметр «Блокировать все входящие подключения».</span><span class="sxs-lookup"><span data-stu-id="4dbe9-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="4dbe9-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="4dbe9-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="4dbe9-209">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-209">Boolean</span></span>|<span data-ttu-id="4dbe9-210">Соответствует «Включить режим скрытое».</span><span class="sxs-lookup"><span data-stu-id="4dbe9-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="4dbe9-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dbe9-211">Response</span></span>
<span data-ttu-id="4dbe9-212">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-212">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dbe9-213">Пример</span><span class="sxs-lookup"><span data-stu-id="4dbe9-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="4dbe9-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dbe9-214">Request</span></span>
<span data-ttu-id="4dbe9-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4dbe9-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dbe9-216">Response</span></span>
<span data-ttu-id="4dbe9-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4dbe9-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



