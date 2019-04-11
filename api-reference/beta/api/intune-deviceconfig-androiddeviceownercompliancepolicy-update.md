---
title: Обновление Андроиддевицеовнеркомплианцеполици
description: Обновление свойств объекта Андроиддевицеовнеркомплианцеполици.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f75c206698bbc5f47e3e43abf722ed8f648645e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809323"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="f1a59-103">Обновление Андроиддевицеовнеркомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="f1a59-103">Update androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="f1a59-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1a59-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1a59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1a59-106">Обновление свойств объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f1a59-106">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1a59-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1a59-107">Prerequisites</span></span>
<span data-ttu-id="f1a59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1a59-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a59-110">Permission type</span></span>|<span data-ttu-id="f1a59-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1a59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1a59-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1a59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1a59-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1a59-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1a59-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1a59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1a59-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a59-115">Not supported.</span></span>|
|<span data-ttu-id="f1a59-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1a59-116">Application</span></span>|<span data-ttu-id="f1a59-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a59-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1a59-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1a59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f1a59-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1a59-119">Request headers</span></span>
|<span data-ttu-id="f1a59-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1a59-120">Header</span></span>|<span data-ttu-id="f1a59-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f1a59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1a59-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1a59-122">Authorization</span></span>|<span data-ttu-id="f1a59-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1a59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1a59-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f1a59-124">Accept</span></span>|<span data-ttu-id="f1a59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1a59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1a59-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1a59-126">Request body</span></span>
<span data-ttu-id="f1a59-127">В тексте запроса добавьте представление объекта [Андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1a59-127">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="f1a59-128">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1a59-128">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="f1a59-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1a59-129">Property</span></span>|<span data-ttu-id="f1a59-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f1a59-130">Type</span></span>|<span data-ttu-id="f1a59-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f1a59-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1a59-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1a59-132">roleScopeTagIds</span></span>|<span data-ttu-id="f1a59-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f1a59-133">String collection</span></span>|<span data-ttu-id="f1a59-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f1a59-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1a59-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1a59-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1a59-136">id</span><span class="sxs-lookup"><span data-stu-id="f1a59-136">id</span></span>|<span data-ttu-id="f1a59-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f1a59-137">String</span></span>|<span data-ttu-id="f1a59-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f1a59-138">Key of the entity.</span></span> <span data-ttu-id="f1a59-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1a59-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1a59-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1a59-140">createdDateTime</span></span>|<span data-ttu-id="f1a59-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1a59-141">DateTimeOffset</span></span>|<span data-ttu-id="f1a59-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f1a59-142">DateTime the object was created.</span></span> <span data-ttu-id="f1a59-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1a59-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1a59-144">description</span><span class="sxs-lookup"><span data-stu-id="f1a59-144">description</span></span>|<span data-ttu-id="f1a59-145">String</span><span class="sxs-lookup"><span data-stu-id="f1a59-145">String</span></span>|<span data-ttu-id="f1a59-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1a59-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1a59-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1a59-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1a59-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1a59-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f1a59-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1a59-149">DateTimeOffset</span></span>|<span data-ttu-id="f1a59-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f1a59-150">DateTime the object was last modified.</span></span> <span data-ttu-id="f1a59-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1a59-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1a59-152">displayName</span><span class="sxs-lookup"><span data-stu-id="f1a59-152">displayName</span></span>|<span data-ttu-id="f1a59-153">Строка</span><span class="sxs-lookup"><span data-stu-id="f1a59-153">String</span></span>|<span data-ttu-id="f1a59-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1a59-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1a59-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1a59-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1a59-156">version</span><span class="sxs-lookup"><span data-stu-id="f1a59-156">version</span></span>|<span data-ttu-id="f1a59-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a59-157">Int32</span></span>|<span data-ttu-id="f1a59-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1a59-158">Version of the device configuration.</span></span> <span data-ttu-id="f1a59-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f1a59-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f1a59-160">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f1a59-160">osMinimumVersion</span></span>|<span data-ttu-id="f1a59-161">String</span><span class="sxs-lookup"><span data-stu-id="f1a59-161">String</span></span>|<span data-ttu-id="f1a59-162">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="f1a59-162">Minimum Android version.</span></span>|
|<span data-ttu-id="f1a59-163">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f1a59-163">osMaximumVersion</span></span>|<span data-ttu-id="f1a59-164">String</span><span class="sxs-lookup"><span data-stu-id="f1a59-164">String</span></span>|<span data-ttu-id="f1a59-165">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="f1a59-165">Maximum Android version.</span></span>|
|<span data-ttu-id="f1a59-166">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f1a59-166">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="f1a59-167">String</span><span class="sxs-lookup"><span data-stu-id="f1a59-167">String</span></span>|<span data-ttu-id="f1a59-168">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="f1a59-168">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="f1a59-169">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f1a59-169">passwordRequired</span></span>|<span data-ttu-id="f1a59-170">Логический</span><span class="sxs-lookup"><span data-stu-id="f1a59-170">Boolean</span></span>|<span data-ttu-id="f1a59-171">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="f1a59-171">Require a password to unlock device.</span></span>|
|<span data-ttu-id="f1a59-172">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f1a59-172">passwordMinimumLength</span></span>|<span data-ttu-id="f1a59-173">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a59-173">Int32</span></span>|<span data-ttu-id="f1a59-174">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="f1a59-174">Minimum password length.</span></span> <span data-ttu-id="f1a59-175">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="f1a59-175">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f1a59-176">Пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="f1a59-176">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="f1a59-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a59-177">Int32</span></span>|<span data-ttu-id="f1a59-178">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="f1a59-178">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="f1a59-179">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="f1a59-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f1a59-180">Пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="f1a59-180">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="f1a59-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a59-181">Int32</span></span>|<span data-ttu-id="f1a59-182">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="f1a59-182">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="f1a59-183">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="f1a59-183">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f1a59-184">Пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="f1a59-184">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="f1a59-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a59-185">Int32</span></span>|<span data-ttu-id="f1a59-186">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="f1a59-186">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="f1a59-187">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="f1a59-187">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f1a59-188">Пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="f1a59-188">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="f1a59-189">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a59-189">Int32</span></span>|<span data-ttu-id="f1a59-190">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="f1a59-190">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="f1a59-191">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="f1a59-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f1a59-192">Пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="f1a59-192">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="f1a59-193">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a59-193">Int32</span></span>|<span data-ttu-id="f1a59-194">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="f1a59-194">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="f1a59-195">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="f1a59-195">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f1a59-196">Пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="f1a59-196">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="f1a59-197">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a59-197">Int32</span></span>|<span data-ttu-id="f1a59-198">Указывает минимальное количество символов в верхнем регистре, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="f1a59-198">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="f1a59-199">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="f1a59-199">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f1a59-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f1a59-200">passwordRequiredType</span></span>|[<span data-ttu-id="f1a59-201">Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="f1a59-201">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="f1a59-202">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="f1a59-202">Type of characters in password.</span></span> <span data-ttu-id="f1a59-203">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="f1a59-203">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="f1a59-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f1a59-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f1a59-205">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a59-205">Int32</span></span>|<span data-ttu-id="f1a59-206">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="f1a59-206">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f1a59-207">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f1a59-207">passwordExpirationDays</span></span>|<span data-ttu-id="f1a59-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a59-208">Int32</span></span>|<span data-ttu-id="f1a59-209">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="f1a59-209">Number of days before the password expires.</span></span> <span data-ttu-id="f1a59-210">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="f1a59-210">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f1a59-211">Пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="f1a59-211">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="f1a59-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a59-212">Int32</span></span>|<span data-ttu-id="f1a59-213">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="f1a59-213">Number of previous passwords to block.</span></span> <span data-ttu-id="f1a59-214">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="f1a59-214">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f1a59-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f1a59-215">storageRequireEncryption</span></span>|<span data-ttu-id="f1a59-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1a59-216">Boolean</span></span>|<span data-ttu-id="f1a59-217">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="f1a59-217">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="f1a59-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a59-218">Response</span></span>
<span data-ttu-id="f1a59-219">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1a59-219">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1a59-220">Пример</span><span class="sxs-lookup"><span data-stu-id="f1a59-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1a59-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1a59-221">Request</span></span>
<span data-ttu-id="f1a59-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1a59-222">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1a59-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a59-223">Response</span></span>
<span data-ttu-id="f1a59-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1a59-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





