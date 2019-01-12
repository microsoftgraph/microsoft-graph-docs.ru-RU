---
title: Update windows81CompliancePolicy
description: Обновление свойств объекта windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecdd69fa115e4352b2470df263df83f889f8c36a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979364"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="dbae5-103">Update windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="dbae5-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="dbae5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dbae5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbae5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbae5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbae5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dbae5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbae5-107">Обновление свойств объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dbae5-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dbae5-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dbae5-108">Prerequisites</span></span>
<span data-ttu-id="dbae5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbae5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbae5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbae5-111">Permission type</span></span>|<span data-ttu-id="dbae5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbae5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbae5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbae5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dbae5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbae5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dbae5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbae5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbae5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbae5-116">Not supported.</span></span>|
|<span data-ttu-id="dbae5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbae5-117">Application</span></span>|<span data-ttu-id="dbae5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbae5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbae5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbae5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="dbae5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbae5-120">Request headers</span></span>
|<span data-ttu-id="dbae5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dbae5-121">Header</span></span>|<span data-ttu-id="dbae5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dbae5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbae5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbae5-123">Authorization</span></span>|<span data-ttu-id="dbae5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dbae5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbae5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dbae5-125">Accept</span></span>|<span data-ttu-id="dbae5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dbae5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbae5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dbae5-127">Request body</span></span>
<span data-ttu-id="dbae5-128">В теле запроса добавьте представление объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbae5-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="dbae5-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dbae5-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="dbae5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbae5-130">Property</span></span>|<span data-ttu-id="dbae5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dbae5-131">Type</span></span>|<span data-ttu-id="dbae5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dbae5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbae5-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dbae5-133">roleScopeTagIds</span></span>|<span data-ttu-id="dbae5-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dbae5-134">String collection</span></span>|<span data-ttu-id="dbae5-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="dbae5-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dbae5-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dbae5-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbae5-137">id</span><span class="sxs-lookup"><span data-stu-id="dbae5-137">id</span></span>|<span data-ttu-id="dbae5-138">String</span><span class="sxs-lookup"><span data-stu-id="dbae5-138">String</span></span>|<span data-ttu-id="dbae5-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dbae5-139">Key of the entity.</span></span> <span data-ttu-id="dbae5-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dbae5-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbae5-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dbae5-141">createdDateTime</span></span>|<span data-ttu-id="dbae5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbae5-142">DateTimeOffset</span></span>|<span data-ttu-id="dbae5-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="dbae5-143">DateTime the object was created.</span></span> <span data-ttu-id="dbae5-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dbae5-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbae5-145">описание</span><span class="sxs-lookup"><span data-stu-id="dbae5-145">description</span></span>|<span data-ttu-id="dbae5-146">String</span><span class="sxs-lookup"><span data-stu-id="dbae5-146">String</span></span>|<span data-ttu-id="dbae5-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dbae5-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dbae5-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dbae5-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbae5-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbae5-149">lastModifiedDateTime</span></span>|<span data-ttu-id="dbae5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbae5-150">DateTimeOffset</span></span>|<span data-ttu-id="dbae5-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dbae5-151">DateTime the object was last modified.</span></span> <span data-ttu-id="dbae5-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dbae5-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbae5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="dbae5-153">displayName</span></span>|<span data-ttu-id="dbae5-154">String</span><span class="sxs-lookup"><span data-stu-id="dbae5-154">String</span></span>|<span data-ttu-id="dbae5-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dbae5-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dbae5-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dbae5-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbae5-157">version</span><span class="sxs-lookup"><span data-stu-id="dbae5-157">version</span></span>|<span data-ttu-id="dbae5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="dbae5-158">Int32</span></span>|<span data-ttu-id="dbae5-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dbae5-159">Version of the device configuration.</span></span> <span data-ttu-id="dbae5-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dbae5-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbae5-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="dbae5-161">passwordRequired</span></span>|<span data-ttu-id="dbae5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbae5-162">Boolean</span></span>|<span data-ttu-id="dbae5-163">Указывает, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="dbae5-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="dbae5-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="dbae5-164">passwordBlockSimple</span></span>|<span data-ttu-id="dbae5-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbae5-165">Boolean</span></span>|<span data-ttu-id="dbae5-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="dbae5-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="dbae5-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dbae5-167">passwordExpirationDays</span></span>|<span data-ttu-id="dbae5-168">Int32</span><span class="sxs-lookup"><span data-stu-id="dbae5-168">Int32</span></span>|<span data-ttu-id="dbae5-169">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="dbae5-169">Password expiration in days.</span></span>|
|<span data-ttu-id="dbae5-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dbae5-170">passwordMinimumLength</span></span>|<span data-ttu-id="dbae5-171">Int32</span><span class="sxs-lookup"><span data-stu-id="dbae5-171">Int32</span></span>|<span data-ttu-id="dbae5-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="dbae5-172">The minimum password length.</span></span>|
|<span data-ttu-id="dbae5-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="dbae5-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="dbae5-174">Int32</span><span class="sxs-lookup"><span data-stu-id="dbae5-174">Int32</span></span>|<span data-ttu-id="dbae5-175">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="dbae5-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="dbae5-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="dbae5-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="dbae5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="dbae5-177">Int32</span></span>|<span data-ttu-id="dbae5-178">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="dbae5-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="dbae5-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="dbae5-179">passwordRequiredType</span></span>|[<span data-ttu-id="dbae5-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dbae5-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="dbae5-181">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="dbae5-181">The required password type.</span></span> <span data-ttu-id="dbae5-182">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="dbae5-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="dbae5-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="dbae5-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="dbae5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="dbae5-184">Int32</span></span>|<span data-ttu-id="dbae5-185">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="dbae5-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="dbae5-186">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="dbae5-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="dbae5-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="dbae5-187">osMinimumVersion</span></span>|<span data-ttu-id="dbae5-188">String</span><span class="sxs-lookup"><span data-stu-id="dbae5-188">String</span></span>|<span data-ttu-id="dbae5-189">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="dbae5-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="dbae5-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="dbae5-190">osMaximumVersion</span></span>|<span data-ttu-id="dbae5-191">String</span><span class="sxs-lookup"><span data-stu-id="dbae5-191">String</span></span>|<span data-ttu-id="dbae5-192">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="dbae5-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="dbae5-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="dbae5-193">storageRequireEncryption</span></span>|<span data-ttu-id="dbae5-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbae5-194">Boolean</span></span>|<span data-ttu-id="dbae5-195">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="dbae5-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="dbae5-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="dbae5-196">Response</span></span>
<span data-ttu-id="dbae5-197">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dbae5-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbae5-198">Пример</span><span class="sxs-lookup"><span data-stu-id="dbae5-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="dbae5-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbae5-199">Request</span></span>
<span data-ttu-id="dbae5-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbae5-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dbae5-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="dbae5-201">Response</span></span>
<span data-ttu-id="dbae5-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dbae5-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





