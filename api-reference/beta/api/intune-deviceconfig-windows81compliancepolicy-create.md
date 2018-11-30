---
title: Создание объекта windows81CompliancePolicy
description: Создание объекта windows81CompliancePolicy.
ms.openlocfilehash: c7366204a6b3985892f6da51efb5611901286d2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081124"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="63471-103">Создание объекта windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="63471-103">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="63471-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="63471-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63471-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63471-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63471-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="63471-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63471-107">Создание объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="63471-107">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63471-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="63471-108">Prerequisites</span></span>
<span data-ttu-id="63471-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63471-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63471-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63471-111">Permission type</span></span>|<span data-ttu-id="63471-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63471-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63471-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63471-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63471-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63471-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63471-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63471-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63471-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63471-116">Not supported.</span></span>|
|<span data-ttu-id="63471-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63471-117">Application</span></span>|<span data-ttu-id="63471-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63471-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63471-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63471-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="63471-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63471-120">Request headers</span></span>
|<span data-ttu-id="63471-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63471-121">Header</span></span>|<span data-ttu-id="63471-122">Значение</span><span class="sxs-lookup"><span data-stu-id="63471-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63471-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63471-123">Authorization</span></span>|<span data-ttu-id="63471-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="63471-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63471-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63471-125">Accept</span></span>|<span data-ttu-id="63471-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63471-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63471-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="63471-127">Request body</span></span>
<span data-ttu-id="63471-128">В теле запроса добавьте представление объекта windows81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63471-128">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="63471-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="63471-129">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="63471-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="63471-130">Property</span></span>|<span data-ttu-id="63471-131">Тип</span><span class="sxs-lookup"><span data-stu-id="63471-131">Type</span></span>|<span data-ttu-id="63471-132">Description</span><span class="sxs-lookup"><span data-stu-id="63471-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63471-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="63471-133">roleScopeTagIds</span></span>|<span data-ttu-id="63471-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="63471-134">String collection</span></span>|<span data-ttu-id="63471-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="63471-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="63471-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="63471-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="63471-137">id</span><span class="sxs-lookup"><span data-stu-id="63471-137">id</span></span>|<span data-ttu-id="63471-138">String</span><span class="sxs-lookup"><span data-stu-id="63471-138">String</span></span>|<span data-ttu-id="63471-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="63471-139">Key of the entity.</span></span> <span data-ttu-id="63471-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="63471-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="63471-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63471-141">createdDateTime</span></span>|<span data-ttu-id="63471-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63471-142">DateTimeOffset</span></span>|<span data-ttu-id="63471-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="63471-143">DateTime the object was created.</span></span> <span data-ttu-id="63471-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="63471-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="63471-145">описание</span><span class="sxs-lookup"><span data-stu-id="63471-145">description</span></span>|<span data-ttu-id="63471-146">String</span><span class="sxs-lookup"><span data-stu-id="63471-146">String</span></span>|<span data-ttu-id="63471-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="63471-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="63471-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="63471-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="63471-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63471-149">lastModifiedDateTime</span></span>|<span data-ttu-id="63471-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63471-150">DateTimeOffset</span></span>|<span data-ttu-id="63471-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="63471-151">DateTime the object was last modified.</span></span> <span data-ttu-id="63471-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="63471-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="63471-153">displayName</span><span class="sxs-lookup"><span data-stu-id="63471-153">displayName</span></span>|<span data-ttu-id="63471-154">String</span><span class="sxs-lookup"><span data-stu-id="63471-154">String</span></span>|<span data-ttu-id="63471-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="63471-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="63471-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="63471-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="63471-157">version</span><span class="sxs-lookup"><span data-stu-id="63471-157">version</span></span>|<span data-ttu-id="63471-158">Int32</span><span class="sxs-lookup"><span data-stu-id="63471-158">Int32</span></span>|<span data-ttu-id="63471-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="63471-159">Version of the device configuration.</span></span> <span data-ttu-id="63471-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="63471-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="63471-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="63471-161">passwordRequired</span></span>|<span data-ttu-id="63471-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="63471-162">Boolean</span></span>|<span data-ttu-id="63471-163">Указывает, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="63471-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="63471-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="63471-164">passwordBlockSimple</span></span>|<span data-ttu-id="63471-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="63471-165">Boolean</span></span>|<span data-ttu-id="63471-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="63471-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="63471-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="63471-167">passwordExpirationDays</span></span>|<span data-ttu-id="63471-168">Int32</span><span class="sxs-lookup"><span data-stu-id="63471-168">Int32</span></span>|<span data-ttu-id="63471-169">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="63471-169">Password expiration in days.</span></span>|
|<span data-ttu-id="63471-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="63471-170">passwordMinimumLength</span></span>|<span data-ttu-id="63471-171">Int32</span><span class="sxs-lookup"><span data-stu-id="63471-171">Int32</span></span>|<span data-ttu-id="63471-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="63471-172">The minimum password length.</span></span>|
|<span data-ttu-id="63471-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="63471-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="63471-174">Int32</span><span class="sxs-lookup"><span data-stu-id="63471-174">Int32</span></span>|<span data-ttu-id="63471-175">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="63471-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="63471-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="63471-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="63471-177">Int32</span><span class="sxs-lookup"><span data-stu-id="63471-177">Int32</span></span>|<span data-ttu-id="63471-178">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="63471-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="63471-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="63471-179">passwordRequiredType</span></span>|[<span data-ttu-id="63471-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="63471-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="63471-181">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="63471-181">The required password type.</span></span> <span data-ttu-id="63471-182">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="63471-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="63471-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="63471-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="63471-184">Int32</span><span class="sxs-lookup"><span data-stu-id="63471-184">Int32</span></span>|<span data-ttu-id="63471-185">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="63471-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="63471-186">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="63471-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="63471-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="63471-187">osMinimumVersion</span></span>|<span data-ttu-id="63471-188">String</span><span class="sxs-lookup"><span data-stu-id="63471-188">String</span></span>|<span data-ttu-id="63471-189">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="63471-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="63471-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="63471-190">osMaximumVersion</span></span>|<span data-ttu-id="63471-191">String</span><span class="sxs-lookup"><span data-stu-id="63471-191">String</span></span>|<span data-ttu-id="63471-192">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="63471-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="63471-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="63471-193">storageRequireEncryption</span></span>|<span data-ttu-id="63471-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="63471-194">Boolean</span></span>|<span data-ttu-id="63471-195">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="63471-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="63471-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="63471-196">Response</span></span>
<span data-ttu-id="63471-197">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="63471-197">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63471-198">Пример</span><span class="sxs-lookup"><span data-stu-id="63471-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="63471-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="63471-199">Request</span></span>
<span data-ttu-id="63471-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63471-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 728

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
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
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="63471-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="63471-201">Response</span></span>
<span data-ttu-id="63471-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="63471-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 836

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```





