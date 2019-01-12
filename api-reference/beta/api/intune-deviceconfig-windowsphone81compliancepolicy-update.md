---
title: Обновление объекта windowsPhone81CompliancePolicy
description: Обновление свойств объекта windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6357ed5b20689dd5059d63869cf5b35e745bdf4d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938407"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="05f7a-103">Обновление объекта windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="05f7a-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="05f7a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05f7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05f7a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05f7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05f7a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="05f7a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05f7a-107">Обновление свойств объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="05f7a-107">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05f7a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="05f7a-108">Prerequisites</span></span>
<span data-ttu-id="05f7a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05f7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05f7a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05f7a-111">Permission type</span></span>|<span data-ttu-id="05f7a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05f7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05f7a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05f7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05f7a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05f7a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05f7a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05f7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05f7a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05f7a-116">Not supported.</span></span>|
|<span data-ttu-id="05f7a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05f7a-117">Application</span></span>|<span data-ttu-id="05f7a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05f7a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05f7a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05f7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="05f7a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05f7a-120">Request headers</span></span>
|<span data-ttu-id="05f7a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05f7a-121">Header</span></span>|<span data-ttu-id="05f7a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="05f7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05f7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05f7a-123">Authorization</span></span>|<span data-ttu-id="05f7a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="05f7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05f7a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05f7a-125">Accept</span></span>|<span data-ttu-id="05f7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05f7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05f7a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05f7a-127">Request body</span></span>
<span data-ttu-id="05f7a-128">В теле запроса добавьте представление объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05f7a-128">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="05f7a-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="05f7a-129">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="05f7a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="05f7a-130">Property</span></span>|<span data-ttu-id="05f7a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="05f7a-131">Type</span></span>|<span data-ttu-id="05f7a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="05f7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05f7a-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="05f7a-133">roleScopeTagIds</span></span>|<span data-ttu-id="05f7a-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="05f7a-134">String collection</span></span>|<span data-ttu-id="05f7a-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="05f7a-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="05f7a-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="05f7a-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="05f7a-137">id</span><span class="sxs-lookup"><span data-stu-id="05f7a-137">id</span></span>|<span data-ttu-id="05f7a-138">String</span><span class="sxs-lookup"><span data-stu-id="05f7a-138">String</span></span>|<span data-ttu-id="05f7a-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="05f7a-139">Key of the entity.</span></span> <span data-ttu-id="05f7a-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="05f7a-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="05f7a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05f7a-141">createdDateTime</span></span>|<span data-ttu-id="05f7a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05f7a-142">DateTimeOffset</span></span>|<span data-ttu-id="05f7a-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="05f7a-143">DateTime the object was created.</span></span> <span data-ttu-id="05f7a-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="05f7a-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="05f7a-145">описание</span><span class="sxs-lookup"><span data-stu-id="05f7a-145">description</span></span>|<span data-ttu-id="05f7a-146">String</span><span class="sxs-lookup"><span data-stu-id="05f7a-146">String</span></span>|<span data-ttu-id="05f7a-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="05f7a-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="05f7a-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="05f7a-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="05f7a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05f7a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="05f7a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05f7a-150">DateTimeOffset</span></span>|<span data-ttu-id="05f7a-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="05f7a-151">DateTime the object was last modified.</span></span> <span data-ttu-id="05f7a-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="05f7a-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="05f7a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="05f7a-153">displayName</span></span>|<span data-ttu-id="05f7a-154">String</span><span class="sxs-lookup"><span data-stu-id="05f7a-154">String</span></span>|<span data-ttu-id="05f7a-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="05f7a-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="05f7a-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="05f7a-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="05f7a-157">version</span><span class="sxs-lookup"><span data-stu-id="05f7a-157">version</span></span>|<span data-ttu-id="05f7a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="05f7a-158">Int32</span></span>|<span data-ttu-id="05f7a-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="05f7a-159">Version of the device configuration.</span></span> <span data-ttu-id="05f7a-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="05f7a-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="05f7a-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="05f7a-161">passwordBlockSimple</span></span>|<span data-ttu-id="05f7a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="05f7a-162">Boolean</span></span>|<span data-ttu-id="05f7a-163">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="05f7a-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="05f7a-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="05f7a-164">passwordExpirationDays</span></span>|<span data-ttu-id="05f7a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="05f7a-165">Int32</span></span>|<span data-ttu-id="05f7a-166">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="05f7a-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="05f7a-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="05f7a-167">passwordMinimumLength</span></span>|<span data-ttu-id="05f7a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="05f7a-168">Int32</span></span>|<span data-ttu-id="05f7a-169">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="05f7a-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="05f7a-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="05f7a-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="05f7a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="05f7a-171">Int32</span></span>|<span data-ttu-id="05f7a-172">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="05f7a-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="05f7a-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="05f7a-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="05f7a-174">Int32</span><span class="sxs-lookup"><span data-stu-id="05f7a-174">Int32</span></span>|<span data-ttu-id="05f7a-175">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="05f7a-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="05f7a-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="05f7a-176">passwordRequiredType</span></span>|[<span data-ttu-id="05f7a-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="05f7a-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="05f7a-178">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="05f7a-178">The required password type.</span></span> <span data-ttu-id="05f7a-179">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="05f7a-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="05f7a-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="05f7a-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="05f7a-181">Int32</span><span class="sxs-lookup"><span data-stu-id="05f7a-181">Int32</span></span>|<span data-ttu-id="05f7a-182">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="05f7a-182">Number of previous passwords to block.</span></span> <span data-ttu-id="05f7a-183">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="05f7a-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="05f7a-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="05f7a-184">passwordRequired</span></span>|<span data-ttu-id="05f7a-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="05f7a-185">Boolean</span></span>|<span data-ttu-id="05f7a-186">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="05f7a-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="05f7a-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="05f7a-187">osMinimumVersion</span></span>|<span data-ttu-id="05f7a-188">String</span><span class="sxs-lookup"><span data-stu-id="05f7a-188">String</span></span>|<span data-ttu-id="05f7a-189">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="05f7a-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="05f7a-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="05f7a-190">osMaximumVersion</span></span>|<span data-ttu-id="05f7a-191">String</span><span class="sxs-lookup"><span data-stu-id="05f7a-191">String</span></span>|<span data-ttu-id="05f7a-192">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="05f7a-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="05f7a-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="05f7a-193">storageRequireEncryption</span></span>|<span data-ttu-id="05f7a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="05f7a-194">Boolean</span></span>|<span data-ttu-id="05f7a-195">Указывает, обязательно ли шифрование данных на устройствах с Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="05f7a-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="05f7a-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="05f7a-196">Response</span></span>
<span data-ttu-id="05f7a-197">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05f7a-197">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05f7a-198">Пример</span><span class="sxs-lookup"><span data-stu-id="05f7a-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="05f7a-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="05f7a-199">Request</span></span>
<span data-ttu-id="05f7a-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05f7a-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 664

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="05f7a-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="05f7a-201">Response</span></span>
<span data-ttu-id="05f7a-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="05f7a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





