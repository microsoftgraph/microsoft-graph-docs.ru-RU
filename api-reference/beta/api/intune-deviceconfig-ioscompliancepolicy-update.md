---
title: Update iosCompliancePolicy
description: Обновление свойств объекта iosCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2207f4f223f6a6b80e9ff563f83c30b048fa1aba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407734"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="667da-103">Update iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="667da-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="667da-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="667da-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="667da-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="667da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="667da-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="667da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="667da-107">Обновление свойств объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="667da-107">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="667da-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="667da-108">Prerequisites</span></span>
<span data-ttu-id="667da-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="667da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="667da-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="667da-111">Permission type</span></span>|<span data-ttu-id="667da-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="667da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="667da-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="667da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="667da-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="667da-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="667da-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="667da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="667da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="667da-116">Not supported.</span></span>|
|<span data-ttu-id="667da-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="667da-117">Application</span></span>|<span data-ttu-id="667da-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="667da-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="667da-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="667da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="667da-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="667da-120">Request headers</span></span>
|<span data-ttu-id="667da-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="667da-121">Header</span></span>|<span data-ttu-id="667da-122">Значение</span><span class="sxs-lookup"><span data-stu-id="667da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="667da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="667da-123">Authorization</span></span>|<span data-ttu-id="667da-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="667da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="667da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="667da-125">Accept</span></span>|<span data-ttu-id="667da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="667da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="667da-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="667da-127">Request body</span></span>
<span data-ttu-id="667da-128">В теле запроса добавьте представление объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="667da-128">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="667da-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="667da-129">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="667da-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="667da-130">Property</span></span>|<span data-ttu-id="667da-131">Тип</span><span class="sxs-lookup"><span data-stu-id="667da-131">Type</span></span>|<span data-ttu-id="667da-132">Описание</span><span class="sxs-lookup"><span data-stu-id="667da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="667da-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="667da-133">roleScopeTagIds</span></span>|<span data-ttu-id="667da-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="667da-134">String collection</span></span>|<span data-ttu-id="667da-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="667da-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="667da-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="667da-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="667da-137">id</span><span class="sxs-lookup"><span data-stu-id="667da-137">id</span></span>|<span data-ttu-id="667da-138">String</span><span class="sxs-lookup"><span data-stu-id="667da-138">String</span></span>|<span data-ttu-id="667da-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="667da-139">Key of the entity.</span></span> <span data-ttu-id="667da-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="667da-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="667da-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="667da-141">createdDateTime</span></span>|<span data-ttu-id="667da-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="667da-142">DateTimeOffset</span></span>|<span data-ttu-id="667da-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="667da-143">DateTime the object was created.</span></span> <span data-ttu-id="667da-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="667da-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="667da-145">description</span><span class="sxs-lookup"><span data-stu-id="667da-145">description</span></span>|<span data-ttu-id="667da-146">String</span><span class="sxs-lookup"><span data-stu-id="667da-146">String</span></span>|<span data-ttu-id="667da-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="667da-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="667da-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="667da-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="667da-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="667da-149">lastModifiedDateTime</span></span>|<span data-ttu-id="667da-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="667da-150">DateTimeOffset</span></span>|<span data-ttu-id="667da-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="667da-151">DateTime the object was last modified.</span></span> <span data-ttu-id="667da-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="667da-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="667da-153">displayName</span><span class="sxs-lookup"><span data-stu-id="667da-153">displayName</span></span>|<span data-ttu-id="667da-154">String</span><span class="sxs-lookup"><span data-stu-id="667da-154">String</span></span>|<span data-ttu-id="667da-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="667da-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="667da-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="667da-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="667da-157">version</span><span class="sxs-lookup"><span data-stu-id="667da-157">version</span></span>|<span data-ttu-id="667da-158">Int32</span><span class="sxs-lookup"><span data-stu-id="667da-158">Int32</span></span>|<span data-ttu-id="667da-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="667da-159">Version of the device configuration.</span></span> <span data-ttu-id="667da-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="667da-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="667da-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="667da-161">passcodeBlockSimple</span></span>|<span data-ttu-id="667da-162">Логический</span><span class="sxs-lookup"><span data-stu-id="667da-162">Boolean</span></span>|<span data-ttu-id="667da-163">Указывает, следует ли блокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="667da-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="667da-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="667da-164">passcodeExpirationDays</span></span>|<span data-ttu-id="667da-165">Int32</span><span class="sxs-lookup"><span data-stu-id="667da-165">Int32</span></span>|<span data-ttu-id="667da-166">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="667da-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="667da-167">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="667da-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="667da-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="667da-168">passcodeMinimumLength</span></span>|<span data-ttu-id="667da-169">Int32</span><span class="sxs-lookup"><span data-stu-id="667da-169">Int32</span></span>|<span data-ttu-id="667da-170">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="667da-170">Minimum length of passcode.</span></span> <span data-ttu-id="667da-171">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="667da-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="667da-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="667da-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="667da-173">Int32</span><span class="sxs-lookup"><span data-stu-id="667da-173">Int32</span></span>|<span data-ttu-id="667da-174">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="667da-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="667da-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="667da-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="667da-176">Int32</span><span class="sxs-lookup"><span data-stu-id="667da-176">Int32</span></span>|<span data-ttu-id="667da-177">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="667da-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="667da-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="667da-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="667da-179">Int32</span><span class="sxs-lookup"><span data-stu-id="667da-179">Int32</span></span>|<span data-ttu-id="667da-180">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="667da-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="667da-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="667da-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="667da-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="667da-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="667da-183">Int32</span><span class="sxs-lookup"><span data-stu-id="667da-183">Int32</span></span>|<span data-ttu-id="667da-184">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="667da-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="667da-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="667da-185">passcodeRequiredType</span></span>|[<span data-ttu-id="667da-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="667da-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="667da-187">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="667da-187">The required passcode type.</span></span> <span data-ttu-id="667da-188">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="667da-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="667da-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="667da-189">passcodeRequired</span></span>|<span data-ttu-id="667da-190">Логический</span><span class="sxs-lookup"><span data-stu-id="667da-190">Boolean</span></span>|<span data-ttu-id="667da-191">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="667da-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="667da-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="667da-192">osMinimumVersion</span></span>|<span data-ttu-id="667da-193">String</span><span class="sxs-lookup"><span data-stu-id="667da-193">String</span></span>|<span data-ttu-id="667da-194">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="667da-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="667da-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="667da-195">osMaximumVersion</span></span>|<span data-ttu-id="667da-196">String</span><span class="sxs-lookup"><span data-stu-id="667da-196">String</span></span>|<span data-ttu-id="667da-197">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="667da-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="667da-198">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="667da-198">osMinimumBuildVersion</span></span>|<span data-ttu-id="667da-199">String</span><span class="sxs-lookup"><span data-stu-id="667da-199">String</span></span>|<span data-ttu-id="667da-200">Версия сборки минимальные операций ввода-ВЫВОДА.</span><span class="sxs-lookup"><span data-stu-id="667da-200">Minimum IOS build version.</span></span>|
|<span data-ttu-id="667da-201">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="667da-201">osMaximumBuildVersion</span></span>|<span data-ttu-id="667da-202">String</span><span class="sxs-lookup"><span data-stu-id="667da-202">String</span></span>|<span data-ttu-id="667da-203">Версия сборки максимальное операций ввода-ВЫВОДА.</span><span class="sxs-lookup"><span data-stu-id="667da-203">Maximum IOS build version.</span></span>|
|<span data-ttu-id="667da-204">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="667da-204">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="667da-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="667da-205">Boolean</span></span>|<span data-ttu-id="667da-206">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="667da-206">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="667da-207">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="667da-207">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="667da-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="667da-208">Boolean</span></span>|<span data-ttu-id="667da-209">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="667da-209">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="667da-210">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="667da-210">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="667da-211">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="667da-211">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="667da-212">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="667da-212">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="667da-213">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="667da-213">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="667da-214">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="667da-214">managedEmailProfileRequired</span></span>|<span data-ttu-id="667da-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="667da-215">Boolean</span></span>|<span data-ttu-id="667da-216">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="667da-216">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="667da-217">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="667da-217">restrictedApps</span></span>|<span data-ttu-id="667da-218">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="667da-218">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="667da-219">Требуется устройство, чтобы отказаться от указанного приложения, установленные.</span><span class="sxs-lookup"><span data-stu-id="667da-219">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="667da-220">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="667da-220">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="667da-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="667da-221">Response</span></span>
<span data-ttu-id="667da-222">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="667da-222">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="667da-223">Пример</span><span class="sxs-lookup"><span data-stu-id="667da-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="667da-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="667da-224">Request</span></span>
<span data-ttu-id="667da-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="667da-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1241

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="667da-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="667da-226">Response</span></span>
<span data-ttu-id="667da-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="667da-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1413

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```




