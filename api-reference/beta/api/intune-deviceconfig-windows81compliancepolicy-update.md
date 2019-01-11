---
title: Update windows81CompliancePolicy
description: Обновление свойств объекта windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5168ea2c806f68d864848169f0f43f3a169e247c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842786"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="a2814-103">Update windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a2814-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="a2814-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a2814-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2814-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2814-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2814-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a2814-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2814-107">Обновление свойств объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a2814-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2814-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a2814-108">Prerequisites</span></span>
<span data-ttu-id="a2814-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2814-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2814-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2814-111">Permission type</span></span>|<span data-ttu-id="a2814-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2814-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2814-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2814-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2814-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2814-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2814-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2814-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2814-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2814-116">Not supported.</span></span>|
|<span data-ttu-id="a2814-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2814-117">Application</span></span>|<span data-ttu-id="a2814-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2814-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2814-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2814-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a2814-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2814-120">Request headers</span></span>
|<span data-ttu-id="a2814-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2814-121">Header</span></span>|<span data-ttu-id="a2814-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2814-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2814-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2814-123">Authorization</span></span>|<span data-ttu-id="a2814-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a2814-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2814-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2814-125">Accept</span></span>|<span data-ttu-id="a2814-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2814-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2814-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2814-127">Request body</span></span>
<span data-ttu-id="a2814-128">В теле запроса добавьте представление объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2814-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="a2814-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a2814-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="a2814-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2814-130">Property</span></span>|<span data-ttu-id="a2814-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2814-131">Type</span></span>|<span data-ttu-id="a2814-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2814-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2814-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a2814-133">roleScopeTagIds</span></span>|<span data-ttu-id="a2814-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a2814-134">String collection</span></span>|<span data-ttu-id="a2814-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a2814-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a2814-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a2814-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2814-137">id</span><span class="sxs-lookup"><span data-stu-id="a2814-137">id</span></span>|<span data-ttu-id="a2814-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a2814-138">String</span></span>|<span data-ttu-id="a2814-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a2814-139">Key of the entity.</span></span> <span data-ttu-id="a2814-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a2814-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2814-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2814-141">createdDateTime</span></span>|<span data-ttu-id="a2814-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2814-142">DateTimeOffset</span></span>|<span data-ttu-id="a2814-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a2814-143">DateTime the object was created.</span></span> <span data-ttu-id="a2814-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a2814-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2814-145">описание</span><span class="sxs-lookup"><span data-stu-id="a2814-145">description</span></span>|<span data-ttu-id="a2814-146">Строка</span><span class="sxs-lookup"><span data-stu-id="a2814-146">String</span></span>|<span data-ttu-id="a2814-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a2814-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a2814-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a2814-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2814-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2814-149">lastModifiedDateTime</span></span>|<span data-ttu-id="a2814-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2814-150">DateTimeOffset</span></span>|<span data-ttu-id="a2814-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a2814-151">DateTime the object was last modified.</span></span> <span data-ttu-id="a2814-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a2814-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2814-153">displayName</span><span class="sxs-lookup"><span data-stu-id="a2814-153">displayName</span></span>|<span data-ttu-id="a2814-154">Строка</span><span class="sxs-lookup"><span data-stu-id="a2814-154">String</span></span>|<span data-ttu-id="a2814-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a2814-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a2814-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a2814-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2814-157">version</span><span class="sxs-lookup"><span data-stu-id="a2814-157">version</span></span>|<span data-ttu-id="a2814-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a2814-158">Int32</span></span>|<span data-ttu-id="a2814-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a2814-159">Version of the device configuration.</span></span> <span data-ttu-id="a2814-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a2814-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2814-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a2814-161">passwordRequired</span></span>|<span data-ttu-id="a2814-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2814-162">Boolean</span></span>|<span data-ttu-id="a2814-163">Указывает, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="a2814-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="a2814-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a2814-164">passwordBlockSimple</span></span>|<span data-ttu-id="a2814-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2814-165">Boolean</span></span>|<span data-ttu-id="a2814-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="a2814-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="a2814-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a2814-167">passwordExpirationDays</span></span>|<span data-ttu-id="a2814-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a2814-168">Int32</span></span>|<span data-ttu-id="a2814-169">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="a2814-169">Password expiration in days.</span></span>|
|<span data-ttu-id="a2814-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a2814-170">passwordMinimumLength</span></span>|<span data-ttu-id="a2814-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a2814-171">Int32</span></span>|<span data-ttu-id="a2814-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="a2814-172">The minimum password length.</span></span>|
|<span data-ttu-id="a2814-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a2814-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a2814-174">Int32</span><span class="sxs-lookup"><span data-stu-id="a2814-174">Int32</span></span>|<span data-ttu-id="a2814-175">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="a2814-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="a2814-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a2814-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="a2814-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a2814-177">Int32</span></span>|<span data-ttu-id="a2814-178">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="a2814-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="a2814-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a2814-179">passwordRequiredType</span></span>|[<span data-ttu-id="a2814-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a2814-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="a2814-181">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="a2814-181">The required password type.</span></span> <span data-ttu-id="a2814-182">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="a2814-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a2814-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a2814-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a2814-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a2814-184">Int32</span></span>|<span data-ttu-id="a2814-185">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="a2814-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="a2814-186">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="a2814-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a2814-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a2814-187">osMinimumVersion</span></span>|<span data-ttu-id="a2814-188">String</span><span class="sxs-lookup"><span data-stu-id="a2814-188">String</span></span>|<span data-ttu-id="a2814-189">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="a2814-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="a2814-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a2814-190">osMaximumVersion</span></span>|<span data-ttu-id="a2814-191">String</span><span class="sxs-lookup"><span data-stu-id="a2814-191">String</span></span>|<span data-ttu-id="a2814-192">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="a2814-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="a2814-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="a2814-193">storageRequireEncryption</span></span>|<span data-ttu-id="a2814-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2814-194">Boolean</span></span>|<span data-ttu-id="a2814-195">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="a2814-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="a2814-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2814-196">Response</span></span>
<span data-ttu-id="a2814-197">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a2814-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2814-198">Пример</span><span class="sxs-lookup"><span data-stu-id="a2814-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2814-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2814-199">Request</span></span>
<span data-ttu-id="a2814-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2814-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a2814-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2814-201">Response</span></span>
<span data-ttu-id="a2814-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a2814-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





