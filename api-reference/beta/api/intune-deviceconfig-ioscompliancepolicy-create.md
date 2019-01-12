---
title: Create iosCompliancePolicy
description: Создание объекта iosCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8cce9c837f6333401025a7775387de2cc15204d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948991"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="a3396-103">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a3396-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="a3396-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a3396-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3396-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3396-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3396-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a3396-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3396-107">Создание объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a3396-107">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3396-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a3396-108">Prerequisites</span></span>
<span data-ttu-id="a3396-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3396-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3396-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3396-111">Permission type</span></span>|<span data-ttu-id="a3396-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3396-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3396-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3396-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3396-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3396-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3396-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3396-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3396-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3396-116">Not supported.</span></span>|
|<span data-ttu-id="a3396-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3396-117">Application</span></span>|<span data-ttu-id="a3396-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3396-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3396-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3396-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a3396-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3396-120">Request headers</span></span>
|<span data-ttu-id="a3396-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3396-121">Header</span></span>|<span data-ttu-id="a3396-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a3396-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3396-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3396-123">Authorization</span></span>|<span data-ttu-id="a3396-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a3396-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3396-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a3396-125">Accept</span></span>|<span data-ttu-id="a3396-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3396-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3396-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3396-127">Request body</span></span>
<span data-ttu-id="a3396-128">В тексте запроса добавьте представление объекта iosCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3396-128">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="a3396-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="a3396-129">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="a3396-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3396-130">Property</span></span>|<span data-ttu-id="a3396-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a3396-131">Type</span></span>|<span data-ttu-id="a3396-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a3396-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3396-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a3396-133">roleScopeTagIds</span></span>|<span data-ttu-id="a3396-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a3396-134">String collection</span></span>|<span data-ttu-id="a3396-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a3396-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a3396-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a3396-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a3396-137">id</span><span class="sxs-lookup"><span data-stu-id="a3396-137">id</span></span>|<span data-ttu-id="a3396-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a3396-138">String</span></span>|<span data-ttu-id="a3396-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3396-139">Key of the entity.</span></span> <span data-ttu-id="a3396-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a3396-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a3396-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3396-141">createdDateTime</span></span>|<span data-ttu-id="a3396-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3396-142">DateTimeOffset</span></span>|<span data-ttu-id="a3396-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a3396-143">DateTime the object was created.</span></span> <span data-ttu-id="a3396-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a3396-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a3396-145">описание</span><span class="sxs-lookup"><span data-stu-id="a3396-145">description</span></span>|<span data-ttu-id="a3396-146">Строка</span><span class="sxs-lookup"><span data-stu-id="a3396-146">String</span></span>|<span data-ttu-id="a3396-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3396-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a3396-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a3396-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a3396-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3396-149">lastModifiedDateTime</span></span>|<span data-ttu-id="a3396-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3396-150">DateTimeOffset</span></span>|<span data-ttu-id="a3396-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a3396-151">DateTime the object was last modified.</span></span> <span data-ttu-id="a3396-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a3396-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a3396-153">displayName</span><span class="sxs-lookup"><span data-stu-id="a3396-153">displayName</span></span>|<span data-ttu-id="a3396-154">Строка</span><span class="sxs-lookup"><span data-stu-id="a3396-154">String</span></span>|<span data-ttu-id="a3396-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3396-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a3396-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a3396-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a3396-157">version</span><span class="sxs-lookup"><span data-stu-id="a3396-157">version</span></span>|<span data-ttu-id="a3396-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a3396-158">Int32</span></span>|<span data-ttu-id="a3396-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3396-159">Version of the device configuration.</span></span> <span data-ttu-id="a3396-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a3396-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a3396-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a3396-161">passcodeBlockSimple</span></span>|<span data-ttu-id="a3396-162">Логический</span><span class="sxs-lookup"><span data-stu-id="a3396-162">Boolean</span></span>|<span data-ttu-id="a3396-163">Указывает, следует ли блокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="a3396-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="a3396-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a3396-164">passcodeExpirationDays</span></span>|<span data-ttu-id="a3396-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a3396-165">Int32</span></span>|<span data-ttu-id="a3396-166">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="a3396-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="a3396-167">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="a3396-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="a3396-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a3396-168">passcodeMinimumLength</span></span>|<span data-ttu-id="a3396-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a3396-169">Int32</span></span>|<span data-ttu-id="a3396-170">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="a3396-170">Minimum length of passcode.</span></span> <span data-ttu-id="a3396-171">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="a3396-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="a3396-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a3396-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a3396-173">Int32</span><span class="sxs-lookup"><span data-stu-id="a3396-173">Int32</span></span>|<span data-ttu-id="a3396-174">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="a3396-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="a3396-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a3396-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a3396-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a3396-176">Int32</span></span>|<span data-ttu-id="a3396-177">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a3396-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a3396-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="a3396-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="a3396-179">Int32</span><span class="sxs-lookup"><span data-stu-id="a3396-179">Int32</span></span>|<span data-ttu-id="a3396-180">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="a3396-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="a3396-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="a3396-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a3396-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a3396-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="a3396-183">Int32</span><span class="sxs-lookup"><span data-stu-id="a3396-183">Int32</span></span>|<span data-ttu-id="a3396-184">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="a3396-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="a3396-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="a3396-185">passcodeRequiredType</span></span>|[<span data-ttu-id="a3396-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a3396-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="a3396-187">Требуемый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="a3396-187">The required passcode type.</span></span> <span data-ttu-id="a3396-188">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="a3396-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a3396-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="a3396-189">passcodeRequired</span></span>|<span data-ttu-id="a3396-190">Логический</span><span class="sxs-lookup"><span data-stu-id="a3396-190">Boolean</span></span>|<span data-ttu-id="a3396-191">Указывает, требуется ли запрашивать секретный код.</span><span class="sxs-lookup"><span data-stu-id="a3396-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="a3396-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a3396-192">osMinimumVersion</span></span>|<span data-ttu-id="a3396-193">String</span><span class="sxs-lookup"><span data-stu-id="a3396-193">String</span></span>|<span data-ttu-id="a3396-194">Минимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="a3396-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="a3396-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a3396-195">osMaximumVersion</span></span>|<span data-ttu-id="a3396-196">String</span><span class="sxs-lookup"><span data-stu-id="a3396-196">String</span></span>|<span data-ttu-id="a3396-197">Максимальная версия iOS.</span><span class="sxs-lookup"><span data-stu-id="a3396-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="a3396-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="a3396-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="a3396-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3396-199">Boolean</span></span>|<span data-ttu-id="a3396-200">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="a3396-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="a3396-201">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a3396-201">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="a3396-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3396-202">Boolean</span></span>|<span data-ttu-id="a3396-203">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="a3396-203">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="a3396-204">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a3396-204">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="a3396-205">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="a3396-205">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="a3396-206">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="a3396-206">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="a3396-207">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="a3396-207">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="a3396-208">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="a3396-208">managedEmailProfileRequired</span></span>|<span data-ttu-id="a3396-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3396-209">Boolean</span></span>|<span data-ttu-id="a3396-210">Указывает, обязательно ли использовать управляемый профиль электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a3396-210">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="a3396-211">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="a3396-211">restrictedApps</span></span>|<span data-ttu-id="a3396-212">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a3396-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a3396-213">Требуется устройство, чтобы отказаться от указанного приложения, установленные.</span><span class="sxs-lookup"><span data-stu-id="a3396-213">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="a3396-214">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="a3396-214">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a3396-215">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3396-215">Response</span></span>
<span data-ttu-id="a3396-216">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a3396-216">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3396-217">Пример</span><span class="sxs-lookup"><span data-stu-id="a3396-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3396-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3396-218">Request</span></span>
<span data-ttu-id="a3396-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3396-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1181

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="a3396-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3396-220">Response</span></span>
<span data-ttu-id="a3396-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a3396-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





