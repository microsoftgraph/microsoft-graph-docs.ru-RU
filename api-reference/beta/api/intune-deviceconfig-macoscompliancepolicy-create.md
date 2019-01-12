---
title: Create macOSCompliancePolicy
description: Создание объекта macOSCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 68e4e59882a2d861a7a65c6077bfa685f8b5b86b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973680"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="c4186-103">Create macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c4186-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="c4186-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c4186-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4186-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4186-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4186-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c4186-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4186-107">Создание объекта [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4186-107">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c4186-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c4186-108">Prerequisites</span></span>
<span data-ttu-id="c4186-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4186-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4186-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4186-111">Permission type</span></span>|<span data-ttu-id="c4186-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4186-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4186-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4186-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4186-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4186-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4186-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4186-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4186-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4186-116">Not supported.</span></span>|
|<span data-ttu-id="c4186-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4186-117">Application</span></span>|<span data-ttu-id="c4186-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4186-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4186-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4186-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c4186-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4186-120">Request headers</span></span>
|<span data-ttu-id="c4186-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4186-121">Header</span></span>|<span data-ttu-id="c4186-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c4186-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4186-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4186-123">Authorization</span></span>|<span data-ttu-id="c4186-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c4186-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4186-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c4186-125">Accept</span></span>|<span data-ttu-id="c4186-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4186-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4186-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c4186-127">Request body</span></span>
<span data-ttu-id="c4186-128">В теле запроса добавьте представление объекта macOSCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4186-128">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="c4186-129">Ниже показаны свойства, которые необходимо указывать при создании объекта macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="c4186-129">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="c4186-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4186-130">Property</span></span>|<span data-ttu-id="c4186-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c4186-131">Type</span></span>|<span data-ttu-id="c4186-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c4186-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4186-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4186-133">roleScopeTagIds</span></span>|<span data-ttu-id="c4186-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c4186-134">String collection</span></span>|<span data-ttu-id="c4186-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c4186-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c4186-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4186-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4186-137">id</span><span class="sxs-lookup"><span data-stu-id="c4186-137">id</span></span>|<span data-ttu-id="c4186-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c4186-138">String</span></span>|<span data-ttu-id="c4186-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c4186-139">Key of the entity.</span></span> <span data-ttu-id="c4186-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4186-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4186-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4186-141">createdDateTime</span></span>|<span data-ttu-id="c4186-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4186-142">DateTimeOffset</span></span>|<span data-ttu-id="c4186-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c4186-143">DateTime the object was created.</span></span> <span data-ttu-id="c4186-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4186-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4186-145">описание</span><span class="sxs-lookup"><span data-stu-id="c4186-145">description</span></span>|<span data-ttu-id="c4186-146">Строка</span><span class="sxs-lookup"><span data-stu-id="c4186-146">String</span></span>|<span data-ttu-id="c4186-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c4186-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c4186-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4186-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4186-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4186-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c4186-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4186-150">DateTimeOffset</span></span>|<span data-ttu-id="c4186-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c4186-151">DateTime the object was last modified.</span></span> <span data-ttu-id="c4186-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4186-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4186-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c4186-153">displayName</span></span>|<span data-ttu-id="c4186-154">Строка</span><span class="sxs-lookup"><span data-stu-id="c4186-154">String</span></span>|<span data-ttu-id="c4186-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c4186-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c4186-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4186-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4186-157">version</span><span class="sxs-lookup"><span data-stu-id="c4186-157">version</span></span>|<span data-ttu-id="c4186-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c4186-158">Int32</span></span>|<span data-ttu-id="c4186-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c4186-159">Version of the device configuration.</span></span> <span data-ttu-id="c4186-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4186-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4186-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c4186-161">passwordRequired</span></span>|<span data-ttu-id="c4186-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4186-162">Boolean</span></span>|<span data-ttu-id="c4186-163">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c4186-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="c4186-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c4186-164">passwordBlockSimple</span></span>|<span data-ttu-id="c4186-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4186-165">Boolean</span></span>|<span data-ttu-id="c4186-166">Указывает, требуется ли блокировать простые пароли.</span><span class="sxs-lookup"><span data-stu-id="c4186-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="c4186-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c4186-167">passwordExpirationDays</span></span>|<span data-ttu-id="c4186-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c4186-168">Int32</span></span>|<span data-ttu-id="c4186-169">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c4186-169">Number of days before the password expires.</span></span> <span data-ttu-id="c4186-170">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="c4186-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="c4186-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c4186-171">passwordMinimumLength</span></span>|<span data-ttu-id="c4186-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c4186-172">Int32</span></span>|<span data-ttu-id="c4186-173">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="c4186-173">Minimum length of password.</span></span> <span data-ttu-id="c4186-174">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="c4186-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="c4186-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c4186-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c4186-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c4186-176">Int32</span></span>|<span data-ttu-id="c4186-177">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c4186-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c4186-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c4186-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c4186-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c4186-179">Int32</span></span>|<span data-ttu-id="c4186-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="c4186-180">Number of previous passwords to block.</span></span> <span data-ttu-id="c4186-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="c4186-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c4186-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c4186-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c4186-183">Int32</span><span class="sxs-lookup"><span data-stu-id="c4186-183">Int32</span></span>|<span data-ttu-id="c4186-184">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="c4186-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c4186-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c4186-185">passwordRequiredType</span></span>|[<span data-ttu-id="c4186-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c4186-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c4186-187">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c4186-187">The required password type.</span></span> <span data-ttu-id="c4186-188">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="c4186-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c4186-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c4186-189">osMinimumVersion</span></span>|<span data-ttu-id="c4186-190">String</span><span class="sxs-lookup"><span data-stu-id="c4186-190">String</span></span>|<span data-ttu-id="c4186-191">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="c4186-191">Minimum IOS version.</span></span>|
|<span data-ttu-id="c4186-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c4186-192">osMaximumVersion</span></span>|<span data-ttu-id="c4186-193">String</span><span class="sxs-lookup"><span data-stu-id="c4186-193">String</span></span>|<span data-ttu-id="c4186-194">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="c4186-194">Maximum IOS version.</span></span>|
|<span data-ttu-id="c4186-195">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c4186-195">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="c4186-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4186-196">Boolean</span></span>|<span data-ttu-id="c4186-197">Указывает на то, что защита целостности системы для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="c4186-197">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="c4186-198">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c4186-198">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c4186-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4186-199">Boolean</span></span>|<span data-ttu-id="c4186-200">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="c4186-200">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="c4186-201">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c4186-201">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c4186-202">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="c4186-202">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c4186-203">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="c4186-203">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c4186-204">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c4186-204">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c4186-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c4186-205">storageRequireEncryption</span></span>|<span data-ttu-id="c4186-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4186-206">Boolean</span></span>|<span data-ttu-id="c4186-207">Указывает, обязательно ли шифрование данных на устройствах с Mac OS.</span><span class="sxs-lookup"><span data-stu-id="c4186-207">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="c4186-208">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="c4186-208">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="c4186-209">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="c4186-209">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="c4186-210">Система и режим конфиденциальности, который определяет, какие приложения расположений загрузки может выполняться на устройстве macOS.</span><span class="sxs-lookup"><span data-stu-id="c4186-210">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="c4186-211">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="c4186-211">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="c4186-212">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="c4186-212">firewallEnabled</span></span>|<span data-ttu-id="c4186-213">Логический</span><span class="sxs-lookup"><span data-stu-id="c4186-213">Boolean</span></span>|<span data-ttu-id="c4186-214">Является ли брандмауэра должна быть включена или нет.</span><span class="sxs-lookup"><span data-stu-id="c4186-214">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="c4186-215">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="c4186-215">firewallBlockAllIncoming</span></span>|<span data-ttu-id="c4186-216">Логический</span><span class="sxs-lookup"><span data-stu-id="c4186-216">Boolean</span></span>|<span data-ttu-id="c4186-217">Соответствующий параметр «Блокировать все входящие подключения».</span><span class="sxs-lookup"><span data-stu-id="c4186-217">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="c4186-218">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="c4186-218">firewallEnableStealthMode</span></span>|<span data-ttu-id="c4186-219">Логический</span><span class="sxs-lookup"><span data-stu-id="c4186-219">Boolean</span></span>|<span data-ttu-id="c4186-220">Соответствует «Включить режим скрытое».</span><span class="sxs-lookup"><span data-stu-id="c4186-220">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="c4186-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4186-221">Response</span></span>
<span data-ttu-id="c4186-222">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c4186-222">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4186-223">Пример</span><span class="sxs-lookup"><span data-stu-id="c4186-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="c4186-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4186-224">Request</span></span>
<span data-ttu-id="c4186-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4186-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1023

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="c4186-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4186-226">Response</span></span>
<span data-ttu-id="c4186-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c4186-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1131

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```





