---
title: Обновление windowsPhone81GeneralConfiguration
description: Обновление свойств объекта windowsPhone81GeneralConfiguration.
author: tfitzmac
ms.openlocfilehash: bbc7208465f625a105bc793681bfd28f8a4f6082
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352145"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="29926-103">Обновление windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="29926-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="29926-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="29926-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29926-105">Обновление свойств объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29926-105">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29926-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="29926-106">Prerequisites</span></span>
<span data-ttu-id="29926-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29926-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29926-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29926-109">Permission type</span></span>|<span data-ttu-id="29926-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="29926-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29926-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29926-111">Delegated (work or school account)</span></span>|<span data-ttu-id="29926-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29926-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29926-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29926-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29926-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29926-114">Not supported.</span></span>|
|<span data-ttu-id="29926-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29926-115">Application</span></span>|<span data-ttu-id="29926-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29926-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29926-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29926-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="29926-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29926-118">Request headers</span></span>
|<span data-ttu-id="29926-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="29926-119">Header</span></span>|<span data-ttu-id="29926-120">Значение</span><span class="sxs-lookup"><span data-stu-id="29926-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29926-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29926-121">Authorization</span></span>|<span data-ttu-id="29926-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="29926-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29926-123">Accept</span><span class="sxs-lookup"><span data-stu-id="29926-123">Accept</span></span>|<span data-ttu-id="29926-124">application/json</span><span class="sxs-lookup"><span data-stu-id="29926-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29926-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="29926-125">Request body</span></span>
<span data-ttu-id="29926-126">В теле запроса добавьте представление объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29926-126">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="29926-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29926-127">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="29926-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="29926-128">Property</span></span>|<span data-ttu-id="29926-129">Тип</span><span class="sxs-lookup"><span data-stu-id="29926-129">Type</span></span>|<span data-ttu-id="29926-130">Описание</span><span class="sxs-lookup"><span data-stu-id="29926-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29926-131">id</span><span class="sxs-lookup"><span data-stu-id="29926-131">id</span></span>|<span data-ttu-id="29926-132">Строка</span><span class="sxs-lookup"><span data-stu-id="29926-132">String</span></span>|<span data-ttu-id="29926-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="29926-133">Key of the entity.</span></span> <span data-ttu-id="29926-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29926-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29926-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29926-135">lastModifiedDateTime</span></span>|<span data-ttu-id="29926-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29926-136">DateTimeOffset</span></span>|<span data-ttu-id="29926-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="29926-137">DateTime the object was last modified.</span></span> <span data-ttu-id="29926-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29926-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29926-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29926-139">createdDateTime</span></span>|<span data-ttu-id="29926-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29926-140">DateTimeOffset</span></span>|<span data-ttu-id="29926-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="29926-141">DateTime the object was created.</span></span> <span data-ttu-id="29926-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29926-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29926-143">описание</span><span class="sxs-lookup"><span data-stu-id="29926-143">description</span></span>|<span data-ttu-id="29926-144">Строка</span><span class="sxs-lookup"><span data-stu-id="29926-144">String</span></span>|<span data-ttu-id="29926-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="29926-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="29926-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29926-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29926-147">displayName</span><span class="sxs-lookup"><span data-stu-id="29926-147">displayName</span></span>|<span data-ttu-id="29926-148">Строка</span><span class="sxs-lookup"><span data-stu-id="29926-148">String</span></span>|<span data-ttu-id="29926-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="29926-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="29926-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29926-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29926-151">version</span><span class="sxs-lookup"><span data-stu-id="29926-151">version</span></span>|<span data-ttu-id="29926-152">Int32</span><span class="sxs-lookup"><span data-stu-id="29926-152">Int32</span></span>|<span data-ttu-id="29926-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="29926-153">Version of the device configuration.</span></span> <span data-ttu-id="29926-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29926-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29926-155">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="29926-155">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="29926-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-156">Boolean</span></span>|<span data-ttu-id="29926-157">Указывает, применяется ли эта политика только к Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="29926-157">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="29926-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29926-158">This property is read-only.</span></span>|
|<span data-ttu-id="29926-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="29926-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="29926-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-160">Boolean</span></span>|<span data-ttu-id="29926-161">Указывает, следует ли заблокировать копирование данных.</span><span class="sxs-lookup"><span data-stu-id="29926-161">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="29926-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="29926-162">bluetoothBlocked</span></span>|<span data-ttu-id="29926-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-163">Boolean</span></span>|<span data-ttu-id="29926-164">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="29926-164">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="29926-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="29926-165">cameraBlocked</span></span>|<span data-ttu-id="29926-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-166">Boolean</span></span>|<span data-ttu-id="29926-167">Указывает, следует ли заблокировать камеру.</span><span class="sxs-lookup"><span data-stu-id="29926-167">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="29926-168">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="29926-168">cellularBlockWifiTethering</span></span>|<span data-ttu-id="29926-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-169">Boolean</span></span>|<span data-ttu-id="29926-170">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="29926-170">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="29926-171">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="29926-171">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="29926-172">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="29926-172">compliantAppsList</span></span>|<span data-ttu-id="29926-173">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="29926-173">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="29926-174">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="29926-174">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="29926-175">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="29926-175">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="29926-176">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="29926-176">compliantAppListType</span></span>|[<span data-ttu-id="29926-177">appListType</span><span class="sxs-lookup"><span data-stu-id="29926-177">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="29926-178">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="29926-178">List that is in the AppComplianceList.</span></span> <span data-ttu-id="29926-179">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="29926-179">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="29926-180">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="29926-180">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="29926-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-181">Boolean</span></span>|<span data-ttu-id="29926-182">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="29926-182">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="29926-183">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="29926-183">emailBlockAddingAccounts</span></span>|<span data-ttu-id="29926-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-184">Boolean</span></span>|<span data-ttu-id="29926-185">Указывает, следует ли заблокировать пользовательские учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="29926-185">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="29926-186">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="29926-186">locationServicesBlocked</span></span>|<span data-ttu-id="29926-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-187">Boolean</span></span>|<span data-ttu-id="29926-188">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="29926-188">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="29926-189">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="29926-189">microsoftAccountBlocked</span></span>|<span data-ttu-id="29926-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-190">Boolean</span></span>|<span data-ttu-id="29926-191">Указывает, следует ли запретить использовать учетную запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="29926-191">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="29926-192">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="29926-192">nfcBlocked</span></span>|<span data-ttu-id="29926-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-193">Boolean</span></span>|<span data-ttu-id="29926-194">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="29926-194">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="29926-195">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="29926-195">passwordBlockSimple</span></span>|<span data-ttu-id="29926-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-196">Boolean</span></span>|<span data-ttu-id="29926-197">Указывает, следует ли заблокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="29926-197">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="29926-198">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="29926-198">passwordExpirationDays</span></span>|<span data-ttu-id="29926-199">Int32</span><span class="sxs-lookup"><span data-stu-id="29926-199">Int32</span></span>|<span data-ttu-id="29926-200">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="29926-200">Number of days before the password expires.</span></span>|
|<span data-ttu-id="29926-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="29926-201">passwordMinimumLength</span></span>|<span data-ttu-id="29926-202">Int32</span><span class="sxs-lookup"><span data-stu-id="29926-202">Int32</span></span>|<span data-ttu-id="29926-203">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="29926-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="29926-204">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="29926-204">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="29926-205">Int32</span><span class="sxs-lookup"><span data-stu-id="29926-205">Int32</span></span>|<span data-ttu-id="29926-206">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="29926-206">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="29926-207">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="29926-207">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="29926-208">Int32</span><span class="sxs-lookup"><span data-stu-id="29926-208">Int32</span></span>|<span data-ttu-id="29926-209">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="29926-209">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="29926-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="29926-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="29926-211">Int32</span><span class="sxs-lookup"><span data-stu-id="29926-211">Int32</span></span>|<span data-ttu-id="29926-212">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="29926-212">Number of previous passwords to block.</span></span> <span data-ttu-id="29926-213">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="29926-213">Valid values 0 to 24</span></span>|
|<span data-ttu-id="29926-214">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="29926-214">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="29926-215">Int32</span><span class="sxs-lookup"><span data-stu-id="29926-215">Int32</span></span>|<span data-ttu-id="29926-216">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="29926-216">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="29926-217">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="29926-217">passwordRequiredType</span></span>|[<span data-ttu-id="29926-218">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="29926-218">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="29926-219">Необходимый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="29926-219">Password type that is required.</span></span> <span data-ttu-id="29926-220">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="29926-220">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="29926-221">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="29926-221">passwordRequired</span></span>|<span data-ttu-id="29926-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-222">Boolean</span></span>|<span data-ttu-id="29926-223">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="29926-223">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="29926-224">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="29926-224">screenCaptureBlocked</span></span>|<span data-ttu-id="29926-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-225">Boolean</span></span>|<span data-ttu-id="29926-226">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="29926-226">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="29926-227">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="29926-227">storageBlockRemovableStorage</span></span>|<span data-ttu-id="29926-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-228">Boolean</span></span>|<span data-ttu-id="29926-229">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="29926-229">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="29926-230">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="29926-230">storageRequireEncryption</span></span>|<span data-ttu-id="29926-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-231">Boolean</span></span>|<span data-ttu-id="29926-232">Указывает, обязательно ли шифрование.</span><span class="sxs-lookup"><span data-stu-id="29926-232">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="29926-233">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="29926-233">webBrowserBlocked</span></span>|<span data-ttu-id="29926-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-234">Boolean</span></span>|<span data-ttu-id="29926-235">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="29926-235">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="29926-236">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="29926-236">wifiBlocked</span></span>|<span data-ttu-id="29926-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-237">Boolean</span></span>|<span data-ttu-id="29926-238">Указывает, следует ли заблокировать Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="29926-238">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="29926-239">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="29926-239">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="29926-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-240">Boolean</span></span>|<span data-ttu-id="29926-241">Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="29926-241">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="29926-242">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="29926-242">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="29926-243">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="29926-243">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="29926-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-244">Boolean</span></span>|<span data-ttu-id="29926-245">Указывает, следует ли запретить устройству сообщать об обнаруженных хот-спотах Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="29926-245">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="29926-246">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="29926-246">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="29926-247">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="29926-247">windowsStoreBlocked</span></span>|<span data-ttu-id="29926-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="29926-248">Boolean</span></span>|<span data-ttu-id="29926-249">Указывает, следует ли заблокировать Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="29926-249">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="29926-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="29926-250">Response</span></span>
<span data-ttu-id="29926-251">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="29926-251">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29926-252">Пример</span><span class="sxs-lookup"><span data-stu-id="29926-252">Example</span></span>
### <a name="request"></a><span data-ttu-id="29926-253">Запрос</span><span class="sxs-lookup"><span data-stu-id="29926-253">Request</span></span>
<span data-ttu-id="29926-254">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29926-254">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="29926-255">Ответ</span><span class="sxs-lookup"><span data-stu-id="29926-255">Response</span></span>
<span data-ttu-id="29926-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="29926-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```



