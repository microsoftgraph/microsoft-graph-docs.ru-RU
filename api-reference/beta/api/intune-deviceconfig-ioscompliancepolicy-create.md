---
title: Create iosCompliancePolicy
description: Создание объекта iosCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 08d932b4120aad82a52a7356c3778cde5362f17c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949176"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="cc922-103">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="cc922-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="cc922-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc922-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc922-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc922-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc922-106">Создание объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cc922-106">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc922-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cc922-107">Prerequisites</span></span>
<span data-ttu-id="cc922-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc922-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc922-110">Permission type</span></span>|<span data-ttu-id="cc922-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc922-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc922-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc922-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc922-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc922-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc922-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc922-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc922-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc922-115">Not supported.</span></span>|
|<span data-ttu-id="cc922-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc922-116">Application</span></span>|<span data-ttu-id="cc922-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc922-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc922-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc922-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="cc922-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cc922-119">Request headers</span></span>
|<span data-ttu-id="cc922-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc922-120">Header</span></span>|<span data-ttu-id="cc922-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cc922-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc922-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc922-122">Authorization</span></span>|<span data-ttu-id="cc922-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc922-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc922-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cc922-124">Accept</span></span>|<span data-ttu-id="cc922-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc922-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc922-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cc922-126">Request body</span></span>
<span data-ttu-id="cc922-127">В тексте запроса добавьте представление объекта iosCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc922-127">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="cc922-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="cc922-128">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="cc922-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc922-129">Property</span></span>|<span data-ttu-id="cc922-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cc922-130">Type</span></span>|<span data-ttu-id="cc922-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cc922-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc922-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cc922-132">roleScopeTagIds</span></span>|<span data-ttu-id="cc922-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cc922-133">String collection</span></span>|<span data-ttu-id="cc922-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cc922-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cc922-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cc922-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cc922-136">description</span><span class="sxs-lookup"><span data-stu-id="cc922-136">description</span></span>|<span data-ttu-id="cc922-137">String</span><span class="sxs-lookup"><span data-stu-id="cc922-137">String</span></span>|<span data-ttu-id="cc922-138">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cc922-138">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cc922-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cc922-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cc922-140">displayName</span><span class="sxs-lookup"><span data-stu-id="cc922-140">displayName</span></span>|<span data-ttu-id="cc922-141">Строка</span><span class="sxs-lookup"><span data-stu-id="cc922-141">String</span></span>|<span data-ttu-id="cc922-142">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cc922-142">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cc922-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cc922-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cc922-144">version</span><span class="sxs-lookup"><span data-stu-id="cc922-144">version</span></span>|<span data-ttu-id="cc922-145">Int32</span><span class="sxs-lookup"><span data-stu-id="cc922-145">Int32</span></span>|<span data-ttu-id="cc922-146">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cc922-146">Version of the device configuration.</span></span> <span data-ttu-id="cc922-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cc922-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cc922-148">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="cc922-148">passcodeBlockSimple</span></span>|<span data-ttu-id="cc922-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc922-149">Boolean</span></span>|<span data-ttu-id="cc922-150">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="cc922-150">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="cc922-151">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cc922-151">passcodeExpirationDays</span></span>|<span data-ttu-id="cc922-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cc922-152">Int32</span></span>|<span data-ttu-id="cc922-153">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="cc922-153">Number of days before the passcode expires.</span></span> <span data-ttu-id="cc922-154">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="cc922-154">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="cc922-155">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cc922-155">passcodeMinimumLength</span></span>|<span data-ttu-id="cc922-156">Int32</span><span class="sxs-lookup"><span data-stu-id="cc922-156">Int32</span></span>|<span data-ttu-id="cc922-157">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="cc922-157">Minimum length of passcode.</span></span> <span data-ttu-id="cc922-158">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="cc922-158">Valid values 4 to 14</span></span>|
|<span data-ttu-id="cc922-159">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cc922-159">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cc922-160">Int32</span><span class="sxs-lookup"><span data-stu-id="cc922-160">Int32</span></span>|<span data-ttu-id="cc922-161">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="cc922-161">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="cc922-162">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="cc922-162">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="cc922-163">Int32</span><span class="sxs-lookup"><span data-stu-id="cc922-163">Int32</span></span>|<span data-ttu-id="cc922-164">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="cc922-164">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="cc922-165">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="cc922-165">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="cc922-166">Int32</span><span class="sxs-lookup"><span data-stu-id="cc922-166">Int32</span></span>|<span data-ttu-id="cc922-167">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="cc922-167">Number of previous passcodes to block.</span></span> <span data-ttu-id="cc922-168">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="cc922-168">Valid values 1 to 24</span></span>|
|<span data-ttu-id="cc922-169">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="cc922-169">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="cc922-170">Int32</span><span class="sxs-lookup"><span data-stu-id="cc922-170">Int32</span></span>|<span data-ttu-id="cc922-171">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="cc922-171">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="cc922-172">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="cc922-172">passcodeRequiredType</span></span>|[<span data-ttu-id="cc922-173">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="cc922-173">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="cc922-174">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="cc922-174">The required passcode type.</span></span> <span data-ttu-id="cc922-175">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="cc922-175">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="cc922-176">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="cc922-176">passcodeRequired</span></span>|<span data-ttu-id="cc922-177">Логический</span><span class="sxs-lookup"><span data-stu-id="cc922-177">Boolean</span></span>|<span data-ttu-id="cc922-178">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="cc922-178">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="cc922-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="cc922-179">osMinimumVersion</span></span>|<span data-ttu-id="cc922-180">Строка</span><span class="sxs-lookup"><span data-stu-id="cc922-180">String</span></span>|<span data-ttu-id="cc922-181">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="cc922-181">Minimum IOS version.</span></span>|
|<span data-ttu-id="cc922-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="cc922-182">osMaximumVersion</span></span>|<span data-ttu-id="cc922-183">String</span><span class="sxs-lookup"><span data-stu-id="cc922-183">String</span></span>|<span data-ttu-id="cc922-184">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="cc922-184">Maximum IOS version.</span></span>|
|<span data-ttu-id="cc922-185">осминимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="cc922-185">osMinimumBuildVersion</span></span>|<span data-ttu-id="cc922-186">Строка</span><span class="sxs-lookup"><span data-stu-id="cc922-186">String</span></span>|<span data-ttu-id="cc922-187">Минимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="cc922-187">Minimum IOS build version.</span></span>|
|<span data-ttu-id="cc922-188">осмаксимумбуилдверсион</span><span class="sxs-lookup"><span data-stu-id="cc922-188">osMaximumBuildVersion</span></span>|<span data-ttu-id="cc922-189">Строка</span><span class="sxs-lookup"><span data-stu-id="cc922-189">String</span></span>|<span data-ttu-id="cc922-190">Максимальная версия сборки IOS.</span><span class="sxs-lookup"><span data-stu-id="cc922-190">Maximum IOS build version.</span></span>|
|<span data-ttu-id="cc922-191">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="cc922-191">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="cc922-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc922-192">Boolean</span></span>|<span data-ttu-id="cc922-193">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="cc922-193">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="cc922-194">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="cc922-194">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="cc922-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc922-195">Boolean</span></span>|<span data-ttu-id="cc922-196">Указывает на то, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="cc922-196">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="cc922-197">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="cc922-197">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="cc922-198">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="cc922-198">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="cc922-199">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="cc922-199">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="cc922-200">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="cc922-200">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="cc922-201">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="cc922-201">managedEmailProfileRequired</span></span>|<span data-ttu-id="cc922-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc922-202">Boolean</span></span>|<span data-ttu-id="cc922-203">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cc922-203">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="cc922-204">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="cc922-204">restrictedApps</span></span>|<span data-ttu-id="cc922-205">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="cc922-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="cc922-206">Потребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="cc922-206">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="cc922-207">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="cc922-207">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="cc922-208">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc922-208">Response</span></span>
<span data-ttu-id="cc922-209">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cc922-209">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc922-210">Пример</span><span class="sxs-lookup"><span data-stu-id="cc922-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc922-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc922-211">Request</span></span>
<span data-ttu-id="cc922-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc922-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="cc922-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc922-213">Response</span></span>
<span data-ttu-id="cc922-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc922-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





