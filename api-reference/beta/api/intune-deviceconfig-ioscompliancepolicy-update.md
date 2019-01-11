---
title: Update iosCompliancePolicy
description: Обновление свойств объекта iosCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: db5f4cafa2d12fee7253e14f67d256fda2d03d0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869491"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="8ae99-103">Update iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8ae99-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="8ae99-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8ae99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ae99-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ae99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ae99-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8ae99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ae99-107">Обновление свойств объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ae99-107">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ae99-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8ae99-108">Prerequisites</span></span>
<span data-ttu-id="8ae99-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ae99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ae99-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ae99-111">Permission type</span></span>|<span data-ttu-id="8ae99-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ae99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ae99-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ae99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ae99-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ae99-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ae99-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ae99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ae99-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ae99-116">Not supported.</span></span>|
|<span data-ttu-id="8ae99-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ae99-117">Application</span></span>|<span data-ttu-id="8ae99-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ae99-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ae99-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ae99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="8ae99-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ae99-120">Request headers</span></span>
|<span data-ttu-id="8ae99-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ae99-121">Header</span></span>|<span data-ttu-id="8ae99-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ae99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ae99-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ae99-123">Authorization</span></span>|<span data-ttu-id="8ae99-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8ae99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ae99-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ae99-125">Accept</span></span>|<span data-ttu-id="8ae99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ae99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ae99-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ae99-127">Request body</span></span>
<span data-ttu-id="8ae99-128">В теле запроса добавьте представление объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ae99-128">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="8ae99-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ae99-129">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="8ae99-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ae99-130">Property</span></span>|<span data-ttu-id="8ae99-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8ae99-131">Type</span></span>|<span data-ttu-id="8ae99-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8ae99-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ae99-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ae99-133">roleScopeTagIds</span></span>|<span data-ttu-id="8ae99-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8ae99-134">String collection</span></span>|<span data-ttu-id="8ae99-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8ae99-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ae99-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ae99-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ae99-137">id</span><span class="sxs-lookup"><span data-stu-id="8ae99-137">id</span></span>|<span data-ttu-id="8ae99-138">Строка</span><span class="sxs-lookup"><span data-stu-id="8ae99-138">String</span></span>|<span data-ttu-id="8ae99-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8ae99-139">Key of the entity.</span></span> <span data-ttu-id="8ae99-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ae99-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ae99-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ae99-141">createdDateTime</span></span>|<span data-ttu-id="8ae99-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ae99-142">DateTimeOffset</span></span>|<span data-ttu-id="8ae99-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8ae99-143">DateTime the object was created.</span></span> <span data-ttu-id="8ae99-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ae99-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ae99-145">описание</span><span class="sxs-lookup"><span data-stu-id="8ae99-145">description</span></span>|<span data-ttu-id="8ae99-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8ae99-146">String</span></span>|<span data-ttu-id="8ae99-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ae99-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ae99-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ae99-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ae99-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ae99-149">lastModifiedDateTime</span></span>|<span data-ttu-id="8ae99-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ae99-150">DateTimeOffset</span></span>|<span data-ttu-id="8ae99-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8ae99-151">DateTime the object was last modified.</span></span> <span data-ttu-id="8ae99-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ae99-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ae99-153">displayName</span><span class="sxs-lookup"><span data-stu-id="8ae99-153">displayName</span></span>|<span data-ttu-id="8ae99-154">Строка</span><span class="sxs-lookup"><span data-stu-id="8ae99-154">String</span></span>|<span data-ttu-id="8ae99-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ae99-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ae99-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ae99-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ae99-157">version</span><span class="sxs-lookup"><span data-stu-id="8ae99-157">version</span></span>|<span data-ttu-id="8ae99-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae99-158">Int32</span></span>|<span data-ttu-id="8ae99-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ae99-159">Version of the device configuration.</span></span> <span data-ttu-id="8ae99-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8ae99-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ae99-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8ae99-161">passcodeBlockSimple</span></span>|<span data-ttu-id="8ae99-162">Логический</span><span class="sxs-lookup"><span data-stu-id="8ae99-162">Boolean</span></span>|<span data-ttu-id="8ae99-163">Указывает, следует ли блокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="8ae99-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="8ae99-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8ae99-164">passcodeExpirationDays</span></span>|<span data-ttu-id="8ae99-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae99-165">Int32</span></span>|<span data-ttu-id="8ae99-166">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="8ae99-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="8ae99-167">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="8ae99-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="8ae99-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8ae99-168">passcodeMinimumLength</span></span>|<span data-ttu-id="8ae99-169">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae99-169">Int32</span></span>|<span data-ttu-id="8ae99-170">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="8ae99-170">Minimum length of passcode.</span></span> <span data-ttu-id="8ae99-171">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="8ae99-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="8ae99-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8ae99-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8ae99-173">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae99-173">Int32</span></span>|<span data-ttu-id="8ae99-174">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="8ae99-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="8ae99-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8ae99-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8ae99-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae99-176">Int32</span></span>|<span data-ttu-id="8ae99-177">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="8ae99-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8ae99-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="8ae99-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="8ae99-179">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae99-179">Int32</span></span>|<span data-ttu-id="8ae99-180">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="8ae99-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="8ae99-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="8ae99-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="8ae99-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8ae99-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="8ae99-183">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae99-183">Int32</span></span>|<span data-ttu-id="8ae99-184">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="8ae99-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8ae99-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="8ae99-185">passcodeRequiredType</span></span>|[<span data-ttu-id="8ae99-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8ae99-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8ae99-187">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="8ae99-187">The required passcode type.</span></span> <span data-ttu-id="8ae99-188">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8ae99-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8ae99-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="8ae99-189">passcodeRequired</span></span>|<span data-ttu-id="8ae99-190">Логический</span><span class="sxs-lookup"><span data-stu-id="8ae99-190">Boolean</span></span>|<span data-ttu-id="8ae99-191">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="8ae99-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="8ae99-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8ae99-192">osMinimumVersion</span></span>|<span data-ttu-id="8ae99-193">String</span><span class="sxs-lookup"><span data-stu-id="8ae99-193">String</span></span>|<span data-ttu-id="8ae99-194">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="8ae99-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="8ae99-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8ae99-195">osMaximumVersion</span></span>|<span data-ttu-id="8ae99-196">String</span><span class="sxs-lookup"><span data-stu-id="8ae99-196">String</span></span>|<span data-ttu-id="8ae99-197">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="8ae99-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="8ae99-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="8ae99-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="8ae99-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ae99-199">Boolean</span></span>|<span data-ttu-id="8ae99-200">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="8ae99-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="8ae99-201">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8ae99-201">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="8ae99-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ae99-202">Boolean</span></span>|<span data-ttu-id="8ae99-203">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="8ae99-203">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="8ae99-204">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8ae99-204">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="8ae99-205">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="8ae99-205">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="8ae99-206">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="8ae99-206">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="8ae99-207">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="8ae99-207">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="8ae99-208">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="8ae99-208">managedEmailProfileRequired</span></span>|<span data-ttu-id="8ae99-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ae99-209">Boolean</span></span>|<span data-ttu-id="8ae99-210">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8ae99-210">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="8ae99-211">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="8ae99-211">restrictedApps</span></span>|<span data-ttu-id="8ae99-212">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="8ae99-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8ae99-213">Требуется устройство, чтобы отказаться от указанного приложения, установленные.</span><span class="sxs-lookup"><span data-stu-id="8ae99-213">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="8ae99-214">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="8ae99-214">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8ae99-215">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ae99-215">Response</span></span>
<span data-ttu-id="8ae99-216">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8ae99-216">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ae99-217">Пример</span><span class="sxs-lookup"><span data-stu-id="8ae99-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ae99-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ae99-218">Request</span></span>
<span data-ttu-id="8ae99-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ae99-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1123

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="8ae99-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ae99-220">Response</span></span>
<span data-ttu-id="8ae99-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8ae99-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1289

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





