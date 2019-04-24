---
title: Обновление Андроиддевицеовнеркомплианцеполици
description: Обновление свойств объекта Андроиддевицеовнеркомплианцеполици.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f75c206698bbc5f47e3e43abf722ed8f648645e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32481033"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="4d085-103">Обновление Андроиддевицеовнеркомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="4d085-103">Update androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="4d085-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d085-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d085-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d085-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d085-106">Обновление свойств объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4d085-106">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d085-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4d085-107">Prerequisites</span></span>
<span data-ttu-id="4d085-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d085-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d085-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d085-110">Permission type</span></span>|<span data-ttu-id="4d085-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d085-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d085-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d085-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d085-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d085-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d085-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d085-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d085-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d085-115">Not supported.</span></span>|
|<span data-ttu-id="4d085-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d085-116">Application</span></span>|<span data-ttu-id="4d085-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d085-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d085-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d085-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4d085-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d085-119">Request headers</span></span>
|<span data-ttu-id="4d085-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d085-120">Header</span></span>|<span data-ttu-id="4d085-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4d085-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d085-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d085-122">Authorization</span></span>|<span data-ttu-id="4d085-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d085-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d085-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4d085-124">Accept</span></span>|<span data-ttu-id="4d085-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d085-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d085-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d085-126">Request body</span></span>
<span data-ttu-id="4d085-127">В тексте запроса добавьте представление объекта [Андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d085-127">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="4d085-128">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4d085-128">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="4d085-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d085-129">Property</span></span>|<span data-ttu-id="4d085-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4d085-130">Type</span></span>|<span data-ttu-id="4d085-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4d085-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d085-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4d085-132">roleScopeTagIds</span></span>|<span data-ttu-id="4d085-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4d085-133">String collection</span></span>|<span data-ttu-id="4d085-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4d085-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4d085-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4d085-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d085-136">id</span><span class="sxs-lookup"><span data-stu-id="4d085-136">id</span></span>|<span data-ttu-id="4d085-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4d085-137">String</span></span>|<span data-ttu-id="4d085-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4d085-138">Key of the entity.</span></span> <span data-ttu-id="4d085-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4d085-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d085-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d085-140">createdDateTime</span></span>|<span data-ttu-id="4d085-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d085-141">DateTimeOffset</span></span>|<span data-ttu-id="4d085-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4d085-142">DateTime the object was created.</span></span> <span data-ttu-id="4d085-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4d085-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d085-144">description</span><span class="sxs-lookup"><span data-stu-id="4d085-144">description</span></span>|<span data-ttu-id="4d085-145">String</span><span class="sxs-lookup"><span data-stu-id="4d085-145">String</span></span>|<span data-ttu-id="4d085-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4d085-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4d085-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4d085-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d085-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d085-148">lastModifiedDateTime</span></span>|<span data-ttu-id="4d085-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d085-149">DateTimeOffset</span></span>|<span data-ttu-id="4d085-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4d085-150">DateTime the object was last modified.</span></span> <span data-ttu-id="4d085-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4d085-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d085-152">displayName</span><span class="sxs-lookup"><span data-stu-id="4d085-152">displayName</span></span>|<span data-ttu-id="4d085-153">Строка</span><span class="sxs-lookup"><span data-stu-id="4d085-153">String</span></span>|<span data-ttu-id="4d085-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4d085-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4d085-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4d085-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d085-156">version</span><span class="sxs-lookup"><span data-stu-id="4d085-156">version</span></span>|<span data-ttu-id="4d085-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4d085-157">Int32</span></span>|<span data-ttu-id="4d085-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4d085-158">Version of the device configuration.</span></span> <span data-ttu-id="4d085-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4d085-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d085-160">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4d085-160">osMinimumVersion</span></span>|<span data-ttu-id="4d085-161">String</span><span class="sxs-lookup"><span data-stu-id="4d085-161">String</span></span>|<span data-ttu-id="4d085-162">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="4d085-162">Minimum Android version.</span></span>|
|<span data-ttu-id="4d085-163">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4d085-163">osMaximumVersion</span></span>|<span data-ttu-id="4d085-164">String</span><span class="sxs-lookup"><span data-stu-id="4d085-164">String</span></span>|<span data-ttu-id="4d085-165">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="4d085-165">Maximum Android version.</span></span>|
|<span data-ttu-id="4d085-166">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="4d085-166">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="4d085-167">String</span><span class="sxs-lookup"><span data-stu-id="4d085-167">String</span></span>|<span data-ttu-id="4d085-168">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="4d085-168">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="4d085-169">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4d085-169">passwordRequired</span></span>|<span data-ttu-id="4d085-170">Логический</span><span class="sxs-lookup"><span data-stu-id="4d085-170">Boolean</span></span>|<span data-ttu-id="4d085-171">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="4d085-171">Require a password to unlock device.</span></span>|
|<span data-ttu-id="4d085-172">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4d085-172">passwordMinimumLength</span></span>|<span data-ttu-id="4d085-173">Int32</span><span class="sxs-lookup"><span data-stu-id="4d085-173">Int32</span></span>|<span data-ttu-id="4d085-174">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="4d085-174">Minimum password length.</span></span> <span data-ttu-id="4d085-175">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="4d085-175">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4d085-176">Пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="4d085-176">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="4d085-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4d085-177">Int32</span></span>|<span data-ttu-id="4d085-178">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4d085-178">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="4d085-179">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4d085-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4d085-180">Пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="4d085-180">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="4d085-181">Int32</span><span class="sxs-lookup"><span data-stu-id="4d085-181">Int32</span></span>|<span data-ttu-id="4d085-182">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4d085-182">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="4d085-183">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4d085-183">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4d085-184">Пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="4d085-184">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="4d085-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4d085-185">Int32</span></span>|<span data-ttu-id="4d085-186">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4d085-186">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="4d085-187">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4d085-187">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4d085-188">Пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="4d085-188">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="4d085-189">Int32</span><span class="sxs-lookup"><span data-stu-id="4d085-189">Int32</span></span>|<span data-ttu-id="4d085-190">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4d085-190">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="4d085-191">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4d085-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4d085-192">Пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="4d085-192">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="4d085-193">Int32</span><span class="sxs-lookup"><span data-stu-id="4d085-193">Int32</span></span>|<span data-ttu-id="4d085-194">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4d085-194">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="4d085-195">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4d085-195">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4d085-196">Пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="4d085-196">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="4d085-197">Int32</span><span class="sxs-lookup"><span data-stu-id="4d085-197">Int32</span></span>|<span data-ttu-id="4d085-198">Указывает минимальное количество символов в верхнем регистре, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4d085-198">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="4d085-199">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4d085-199">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4d085-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4d085-200">passwordRequiredType</span></span>|[<span data-ttu-id="4d085-201">Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="4d085-201">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="4d085-202">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="4d085-202">Type of characters in password.</span></span> <span data-ttu-id="4d085-203">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="4d085-203">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="4d085-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4d085-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4d085-205">Int32</span><span class="sxs-lookup"><span data-stu-id="4d085-205">Int32</span></span>|<span data-ttu-id="4d085-206">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="4d085-206">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4d085-207">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4d085-207">passwordExpirationDays</span></span>|<span data-ttu-id="4d085-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4d085-208">Int32</span></span>|<span data-ttu-id="4d085-209">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="4d085-209">Number of days before the password expires.</span></span> <span data-ttu-id="4d085-210">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="4d085-210">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4d085-211">Пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="4d085-211">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="4d085-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4d085-212">Int32</span></span>|<span data-ttu-id="4d085-213">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="4d085-213">Number of previous passwords to block.</span></span> <span data-ttu-id="4d085-214">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="4d085-214">Valid values 1 to 24</span></span>|
|<span data-ttu-id="4d085-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4d085-215">storageRequireEncryption</span></span>|<span data-ttu-id="4d085-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d085-216">Boolean</span></span>|<span data-ttu-id="4d085-217">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="4d085-217">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="4d085-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d085-218">Response</span></span>
<span data-ttu-id="4d085-219">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d085-219">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d085-220">Пример</span><span class="sxs-lookup"><span data-stu-id="4d085-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d085-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d085-221">Request</span></span>
<span data-ttu-id="4d085-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d085-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 932

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="4d085-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d085-223">Response</span></span>
<span data-ttu-id="4d085-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d085-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1104

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "be2464b4-64b4-be24-b464-24beb46424be",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```





