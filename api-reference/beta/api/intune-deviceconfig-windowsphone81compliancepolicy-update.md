---
title: Обновление объекта windowsPhone81CompliancePolicy
description: Обновление свойств объекта windowsPhone81CompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 190bdcabd7662295c3c02a8fadac48d9ec966ba0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425577"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="1c331-103">Обновление объекта windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="1c331-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="1c331-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1c331-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1c331-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c331-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c331-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c331-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c331-107">Обновление свойств объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c331-107">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c331-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1c331-108">Prerequisites</span></span>
<span data-ttu-id="1c331-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c331-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1c331-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c331-111">Permission type</span></span>|<span data-ttu-id="1c331-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c331-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c331-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c331-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c331-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c331-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c331-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c331-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c331-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c331-116">Not supported.</span></span>|
|<span data-ttu-id="1c331-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c331-117">Application</span></span>|<span data-ttu-id="1c331-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c331-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c331-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c331-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="1c331-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c331-120">Request headers</span></span>
|<span data-ttu-id="1c331-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c331-121">Header</span></span>|<span data-ttu-id="1c331-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1c331-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c331-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c331-123">Authorization</span></span>|<span data-ttu-id="1c331-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1c331-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c331-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c331-125">Accept</span></span>|<span data-ttu-id="1c331-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c331-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c331-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1c331-127">Request body</span></span>
<span data-ttu-id="1c331-128">В теле запроса добавьте представление объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c331-128">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="1c331-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c331-129">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="1c331-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c331-130">Property</span></span>|<span data-ttu-id="1c331-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1c331-131">Type</span></span>|<span data-ttu-id="1c331-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1c331-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c331-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c331-133">roleScopeTagIds</span></span>|<span data-ttu-id="1c331-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1c331-134">String collection</span></span>|<span data-ttu-id="1c331-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1c331-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1c331-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c331-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1c331-137">id</span><span class="sxs-lookup"><span data-stu-id="1c331-137">id</span></span>|<span data-ttu-id="1c331-138">String</span><span class="sxs-lookup"><span data-stu-id="1c331-138">String</span></span>|<span data-ttu-id="1c331-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1c331-139">Key of the entity.</span></span> <span data-ttu-id="1c331-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c331-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1c331-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c331-141">createdDateTime</span></span>|<span data-ttu-id="1c331-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c331-142">DateTimeOffset</span></span>|<span data-ttu-id="1c331-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1c331-143">DateTime the object was created.</span></span> <span data-ttu-id="1c331-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c331-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1c331-145">description</span><span class="sxs-lookup"><span data-stu-id="1c331-145">description</span></span>|<span data-ttu-id="1c331-146">String</span><span class="sxs-lookup"><span data-stu-id="1c331-146">String</span></span>|<span data-ttu-id="1c331-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c331-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1c331-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c331-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1c331-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c331-149">lastModifiedDateTime</span></span>|<span data-ttu-id="1c331-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c331-150">DateTimeOffset</span></span>|<span data-ttu-id="1c331-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1c331-151">DateTime the object was last modified.</span></span> <span data-ttu-id="1c331-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c331-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1c331-153">displayName</span><span class="sxs-lookup"><span data-stu-id="1c331-153">displayName</span></span>|<span data-ttu-id="1c331-154">String</span><span class="sxs-lookup"><span data-stu-id="1c331-154">String</span></span>|<span data-ttu-id="1c331-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c331-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1c331-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c331-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1c331-157">version</span><span class="sxs-lookup"><span data-stu-id="1c331-157">version</span></span>|<span data-ttu-id="1c331-158">Int32</span><span class="sxs-lookup"><span data-stu-id="1c331-158">Int32</span></span>|<span data-ttu-id="1c331-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c331-159">Version of the device configuration.</span></span> <span data-ttu-id="1c331-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c331-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1c331-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1c331-161">passwordBlockSimple</span></span>|<span data-ttu-id="1c331-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c331-162">Boolean</span></span>|<span data-ttu-id="1c331-163">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="1c331-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="1c331-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1c331-164">passwordExpirationDays</span></span>|<span data-ttu-id="1c331-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1c331-165">Int32</span></span>|<span data-ttu-id="1c331-166">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="1c331-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="1c331-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1c331-167">passwordMinimumLength</span></span>|<span data-ttu-id="1c331-168">Int32</span><span class="sxs-lookup"><span data-stu-id="1c331-168">Int32</span></span>|<span data-ttu-id="1c331-169">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="1c331-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="1c331-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1c331-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1c331-171">Int32</span><span class="sxs-lookup"><span data-stu-id="1c331-171">Int32</span></span>|<span data-ttu-id="1c331-172">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="1c331-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="1c331-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1c331-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="1c331-174">Int32</span><span class="sxs-lookup"><span data-stu-id="1c331-174">Int32</span></span>|<span data-ttu-id="1c331-175">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="1c331-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="1c331-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1c331-176">passwordRequiredType</span></span>|[<span data-ttu-id="1c331-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1c331-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="1c331-178">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="1c331-178">The required password type.</span></span> <span data-ttu-id="1c331-179">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="1c331-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="1c331-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1c331-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1c331-181">Int32</span><span class="sxs-lookup"><span data-stu-id="1c331-181">Int32</span></span>|<span data-ttu-id="1c331-182">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="1c331-182">Number of previous passwords to block.</span></span> <span data-ttu-id="1c331-183">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="1c331-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1c331-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1c331-184">passwordRequired</span></span>|<span data-ttu-id="1c331-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c331-185">Boolean</span></span>|<span data-ttu-id="1c331-186">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="1c331-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="1c331-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1c331-187">osMinimumVersion</span></span>|<span data-ttu-id="1c331-188">String</span><span class="sxs-lookup"><span data-stu-id="1c331-188">String</span></span>|<span data-ttu-id="1c331-189">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="1c331-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="1c331-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1c331-190">osMaximumVersion</span></span>|<span data-ttu-id="1c331-191">String</span><span class="sxs-lookup"><span data-stu-id="1c331-191">String</span></span>|<span data-ttu-id="1c331-192">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="1c331-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="1c331-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="1c331-193">storageRequireEncryption</span></span>|<span data-ttu-id="1c331-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c331-194">Boolean</span></span>|<span data-ttu-id="1c331-195">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="1c331-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="1c331-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c331-196">Response</span></span>
<span data-ttu-id="1c331-197">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1c331-197">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c331-198">Пример</span><span class="sxs-lookup"><span data-stu-id="1c331-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c331-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c331-199">Request</span></span>
<span data-ttu-id="1c331-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c331-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 669

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="1c331-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c331-201">Response</span></span>
<span data-ttu-id="1c331-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1c331-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 841

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```




