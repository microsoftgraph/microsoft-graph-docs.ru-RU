---
title: Обновление windowsPhone81GeneralConfiguration
description: Обновление свойств объекта windowsPhone81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a81ff812b1a40bd9e3b6aeb20f12639d8fc00ac5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447876"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="14294-103">Обновление windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="14294-103">Update windowsPhone81GeneralConfiguration</span></span>

<span data-ttu-id="14294-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14294-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14294-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14294-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14294-106">Обновление свойств объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14294-106">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14294-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="14294-107">Prerequisites</span></span>
<span data-ttu-id="14294-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14294-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14294-110">Permission type</span></span>|<span data-ttu-id="14294-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14294-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14294-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14294-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14294-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14294-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14294-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14294-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14294-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14294-115">Not supported.</span></span>|
|<span data-ttu-id="14294-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14294-116">Application</span></span>|<span data-ttu-id="14294-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14294-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14294-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14294-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="14294-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="14294-119">Request headers</span></span>
|<span data-ttu-id="14294-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14294-120">Header</span></span>|<span data-ttu-id="14294-121">Значение</span><span class="sxs-lookup"><span data-stu-id="14294-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14294-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14294-122">Authorization</span></span>|<span data-ttu-id="14294-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14294-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14294-124">Accept</span><span class="sxs-lookup"><span data-stu-id="14294-124">Accept</span></span>|<span data-ttu-id="14294-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14294-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14294-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14294-126">Request body</span></span>
<span data-ttu-id="14294-127">В теле запроса добавьте представление объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14294-127">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="14294-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14294-128">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="14294-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="14294-129">Property</span></span>|<span data-ttu-id="14294-130">Тип</span><span class="sxs-lookup"><span data-stu-id="14294-130">Type</span></span>|<span data-ttu-id="14294-131">Описание</span><span class="sxs-lookup"><span data-stu-id="14294-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14294-132">id</span><span class="sxs-lookup"><span data-stu-id="14294-132">id</span></span>|<span data-ttu-id="14294-133">String</span><span class="sxs-lookup"><span data-stu-id="14294-133">String</span></span>|<span data-ttu-id="14294-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="14294-134">Key of the entity.</span></span> <span data-ttu-id="14294-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14294-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14294-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14294-136">lastModifiedDateTime</span></span>|<span data-ttu-id="14294-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14294-137">DateTimeOffset</span></span>|<span data-ttu-id="14294-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="14294-138">DateTime the object was last modified.</span></span> <span data-ttu-id="14294-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14294-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14294-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14294-140">createdDateTime</span></span>|<span data-ttu-id="14294-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14294-141">DateTimeOffset</span></span>|<span data-ttu-id="14294-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="14294-142">DateTime the object was created.</span></span> <span data-ttu-id="14294-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14294-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14294-144">description</span><span class="sxs-lookup"><span data-stu-id="14294-144">description</span></span>|<span data-ttu-id="14294-145">String</span><span class="sxs-lookup"><span data-stu-id="14294-145">String</span></span>|<span data-ttu-id="14294-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14294-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="14294-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14294-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14294-148">displayName</span><span class="sxs-lookup"><span data-stu-id="14294-148">displayName</span></span>|<span data-ttu-id="14294-149">Строка</span><span class="sxs-lookup"><span data-stu-id="14294-149">String</span></span>|<span data-ttu-id="14294-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14294-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="14294-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14294-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14294-152">version</span><span class="sxs-lookup"><span data-stu-id="14294-152">version</span></span>|<span data-ttu-id="14294-153">Int32</span><span class="sxs-lookup"><span data-stu-id="14294-153">Int32</span></span>|<span data-ttu-id="14294-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14294-154">Version of the device configuration.</span></span> <span data-ttu-id="14294-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14294-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14294-156">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="14294-156">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="14294-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-157">Boolean</span></span>|<span data-ttu-id="14294-158">Указывает, применяется ли эта политика только к Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="14294-158">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="14294-159">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14294-159">This property is read-only.</span></span>|
|<span data-ttu-id="14294-160">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="14294-160">appsBlockCopyPaste</span></span>|<span data-ttu-id="14294-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-161">Boolean</span></span>|<span data-ttu-id="14294-162">Указывает, следует ли заблокировать копирование данных.</span><span class="sxs-lookup"><span data-stu-id="14294-162">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="14294-163">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="14294-163">bluetoothBlocked</span></span>|<span data-ttu-id="14294-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-164">Boolean</span></span>|<span data-ttu-id="14294-165">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="14294-165">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="14294-166">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="14294-166">cameraBlocked</span></span>|<span data-ttu-id="14294-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-167">Boolean</span></span>|<span data-ttu-id="14294-168">Указывает, следует ли заблокировать камеру.</span><span class="sxs-lookup"><span data-stu-id="14294-168">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="14294-169">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="14294-169">cellularBlockWifiTethering</span></span>|<span data-ttu-id="14294-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-170">Boolean</span></span>|<span data-ttu-id="14294-171">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="14294-171">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="14294-172">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="14294-172">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="14294-173">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="14294-173">compliantAppsList</span></span>|<span data-ttu-id="14294-174">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="14294-174">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="14294-175">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="14294-175">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="14294-176">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="14294-176">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="14294-177">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="14294-177">compliantAppListType</span></span>|[<span data-ttu-id="14294-178">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="14294-178">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="14294-179">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="14294-179">List that is in the AppComplianceList.</span></span> <span data-ttu-id="14294-180">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="14294-180">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="14294-181">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="14294-181">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="14294-182">Логический</span><span class="sxs-lookup"><span data-stu-id="14294-182">Boolean</span></span>|<span data-ttu-id="14294-183">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="14294-183">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="14294-184">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="14294-184">emailBlockAddingAccounts</span></span>|<span data-ttu-id="14294-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-185">Boolean</span></span>|<span data-ttu-id="14294-186">Указывает, следует ли заблокировать пользовательские учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="14294-186">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="14294-187">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="14294-187">locationServicesBlocked</span></span>|<span data-ttu-id="14294-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-188">Boolean</span></span>|<span data-ttu-id="14294-189">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="14294-189">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="14294-190">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="14294-190">microsoftAccountBlocked</span></span>|<span data-ttu-id="14294-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-191">Boolean</span></span>|<span data-ttu-id="14294-192">Указывает, следует ли запретить использовать учетную запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="14294-192">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="14294-193">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="14294-193">nfcBlocked</span></span>|<span data-ttu-id="14294-194">Логический</span><span class="sxs-lookup"><span data-stu-id="14294-194">Boolean</span></span>|<span data-ttu-id="14294-195">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="14294-195">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="14294-196">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="14294-196">passwordBlockSimple</span></span>|<span data-ttu-id="14294-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-197">Boolean</span></span>|<span data-ttu-id="14294-198">Указывает, следует ли заблокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="14294-198">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="14294-199">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="14294-199">passwordExpirationDays</span></span>|<span data-ttu-id="14294-200">Int32</span><span class="sxs-lookup"><span data-stu-id="14294-200">Int32</span></span>|<span data-ttu-id="14294-201">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="14294-201">Number of days before the password expires.</span></span>|
|<span data-ttu-id="14294-202">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="14294-202">passwordMinimumLength</span></span>|<span data-ttu-id="14294-203">Int32</span><span class="sxs-lookup"><span data-stu-id="14294-203">Int32</span></span>|<span data-ttu-id="14294-204">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="14294-204">Minimum length of passwords.</span></span>|
|<span data-ttu-id="14294-205">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="14294-205">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="14294-206">Int32</span><span class="sxs-lookup"><span data-stu-id="14294-206">Int32</span></span>|<span data-ttu-id="14294-207">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="14294-207">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="14294-208">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="14294-208">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="14294-209">Int32</span><span class="sxs-lookup"><span data-stu-id="14294-209">Int32</span></span>|<span data-ttu-id="14294-210">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="14294-210">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="14294-211">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="14294-211">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="14294-212">Int32</span><span class="sxs-lookup"><span data-stu-id="14294-212">Int32</span></span>|<span data-ttu-id="14294-213">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="14294-213">Number of previous passwords to block.</span></span> <span data-ttu-id="14294-214">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="14294-214">Valid values 0 to 24</span></span>|
|<span data-ttu-id="14294-215">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="14294-215">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="14294-216">Int32</span><span class="sxs-lookup"><span data-stu-id="14294-216">Int32</span></span>|<span data-ttu-id="14294-217">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="14294-217">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="14294-218">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="14294-218">passwordRequiredType</span></span>|[<span data-ttu-id="14294-219">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="14294-219">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="14294-220">Необходимый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="14294-220">Password type that is required.</span></span> <span data-ttu-id="14294-221">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="14294-221">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="14294-222">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="14294-222">passwordRequired</span></span>|<span data-ttu-id="14294-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-223">Boolean</span></span>|<span data-ttu-id="14294-224">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="14294-224">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="14294-225">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="14294-225">screenCaptureBlocked</span></span>|<span data-ttu-id="14294-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-226">Boolean</span></span>|<span data-ttu-id="14294-227">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="14294-227">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="14294-228">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="14294-228">storageBlockRemovableStorage</span></span>|<span data-ttu-id="14294-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-229">Boolean</span></span>|<span data-ttu-id="14294-230">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="14294-230">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="14294-231">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="14294-231">storageRequireEncryption</span></span>|<span data-ttu-id="14294-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-232">Boolean</span></span>|<span data-ttu-id="14294-233">Указывает, обязательно ли шифрование.</span><span class="sxs-lookup"><span data-stu-id="14294-233">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="14294-234">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="14294-234">webBrowserBlocked</span></span>|<span data-ttu-id="14294-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-235">Boolean</span></span>|<span data-ttu-id="14294-236">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="14294-236">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="14294-237">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="14294-237">wifiBlocked</span></span>|<span data-ttu-id="14294-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-238">Boolean</span></span>|<span data-ttu-id="14294-239">Указывает, следует ли заблокировать Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="14294-239">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="14294-240">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="14294-240">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="14294-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-241">Boolean</span></span>|<span data-ttu-id="14294-242">Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="14294-242">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="14294-243">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="14294-243">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="14294-244">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="14294-244">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="14294-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-245">Boolean</span></span>|<span data-ttu-id="14294-246">Указывает, следует ли запретить устройству сообщать об обнаруженных хот-спотах Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="14294-246">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="14294-247">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="14294-247">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="14294-248">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="14294-248">windowsStoreBlocked</span></span>|<span data-ttu-id="14294-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="14294-249">Boolean</span></span>|<span data-ttu-id="14294-250">Указывает, следует ли заблокировать Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="14294-250">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="14294-251">Отклик</span><span class="sxs-lookup"><span data-stu-id="14294-251">Response</span></span>
<span data-ttu-id="14294-252">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="14294-252">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14294-253">Пример</span><span class="sxs-lookup"><span data-stu-id="14294-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="14294-254">Запрос</span><span class="sxs-lookup"><span data-stu-id="14294-254">Request</span></span>
<span data-ttu-id="14294-255">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14294-255">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14294-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="14294-256">Response</span></span>
<span data-ttu-id="14294-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14294-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






