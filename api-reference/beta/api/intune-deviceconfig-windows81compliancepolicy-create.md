---
title: Создание объекта windows81CompliancePolicy
description: Создание объекта windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e56271e8854bea82fa7d818722fa1b016f780f97
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935390"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="3a596-103">Создание объекта windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3a596-103">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="3a596-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a596-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a596-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a596-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a596-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3a596-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a596-107">Создание объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a596-107">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a596-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3a596-108">Prerequisites</span></span>
<span data-ttu-id="3a596-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a596-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a596-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a596-111">Permission type</span></span>|<span data-ttu-id="3a596-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a596-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a596-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a596-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a596-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a596-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a596-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a596-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a596-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a596-116">Not supported.</span></span>|
|<span data-ttu-id="3a596-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a596-117">Application</span></span>|<span data-ttu-id="3a596-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a596-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a596-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a596-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3a596-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a596-120">Request headers</span></span>
|<span data-ttu-id="3a596-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a596-121">Header</span></span>|<span data-ttu-id="3a596-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a596-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a596-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a596-123">Authorization</span></span>|<span data-ttu-id="3a596-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3a596-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a596-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a596-125">Accept</span></span>|<span data-ttu-id="3a596-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a596-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a596-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a596-127">Request body</span></span>
<span data-ttu-id="3a596-128">В теле запроса добавьте представление объекта windows81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a596-128">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="3a596-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="3a596-129">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="3a596-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a596-130">Property</span></span>|<span data-ttu-id="3a596-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a596-131">Type</span></span>|<span data-ttu-id="3a596-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a596-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a596-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a596-133">roleScopeTagIds</span></span>|<span data-ttu-id="3a596-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3a596-134">String collection</span></span>|<span data-ttu-id="3a596-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3a596-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3a596-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a596-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a596-137">id</span><span class="sxs-lookup"><span data-stu-id="3a596-137">id</span></span>|<span data-ttu-id="3a596-138">String</span><span class="sxs-lookup"><span data-stu-id="3a596-138">String</span></span>|<span data-ttu-id="3a596-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3a596-139">Key of the entity.</span></span> <span data-ttu-id="3a596-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a596-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a596-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a596-141">createdDateTime</span></span>|<span data-ttu-id="3a596-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a596-142">DateTimeOffset</span></span>|<span data-ttu-id="3a596-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3a596-143">DateTime the object was created.</span></span> <span data-ttu-id="3a596-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a596-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a596-145">описание</span><span class="sxs-lookup"><span data-stu-id="3a596-145">description</span></span>|<span data-ttu-id="3a596-146">String</span><span class="sxs-lookup"><span data-stu-id="3a596-146">String</span></span>|<span data-ttu-id="3a596-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a596-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3a596-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a596-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a596-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a596-149">lastModifiedDateTime</span></span>|<span data-ttu-id="3a596-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a596-150">DateTimeOffset</span></span>|<span data-ttu-id="3a596-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3a596-151">DateTime the object was last modified.</span></span> <span data-ttu-id="3a596-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a596-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a596-153">displayName</span><span class="sxs-lookup"><span data-stu-id="3a596-153">displayName</span></span>|<span data-ttu-id="3a596-154">String</span><span class="sxs-lookup"><span data-stu-id="3a596-154">String</span></span>|<span data-ttu-id="3a596-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a596-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3a596-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a596-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a596-157">version</span><span class="sxs-lookup"><span data-stu-id="3a596-157">version</span></span>|<span data-ttu-id="3a596-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3a596-158">Int32</span></span>|<span data-ttu-id="3a596-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a596-159">Version of the device configuration.</span></span> <span data-ttu-id="3a596-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a596-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a596-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3a596-161">passwordRequired</span></span>|<span data-ttu-id="3a596-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a596-162">Boolean</span></span>|<span data-ttu-id="3a596-163">Указывает, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="3a596-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="3a596-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3a596-164">passwordBlockSimple</span></span>|<span data-ttu-id="3a596-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a596-165">Boolean</span></span>|<span data-ttu-id="3a596-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="3a596-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="3a596-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3a596-167">passwordExpirationDays</span></span>|<span data-ttu-id="3a596-168">Int32</span><span class="sxs-lookup"><span data-stu-id="3a596-168">Int32</span></span>|<span data-ttu-id="3a596-169">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="3a596-169">Password expiration in days.</span></span>|
|<span data-ttu-id="3a596-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3a596-170">passwordMinimumLength</span></span>|<span data-ttu-id="3a596-171">Int32</span><span class="sxs-lookup"><span data-stu-id="3a596-171">Int32</span></span>|<span data-ttu-id="3a596-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="3a596-172">The minimum password length.</span></span>|
|<span data-ttu-id="3a596-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3a596-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3a596-174">Int32</span><span class="sxs-lookup"><span data-stu-id="3a596-174">Int32</span></span>|<span data-ttu-id="3a596-175">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="3a596-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="3a596-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3a596-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3a596-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3a596-177">Int32</span></span>|<span data-ttu-id="3a596-178">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="3a596-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3a596-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3a596-179">passwordRequiredType</span></span>|[<span data-ttu-id="3a596-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3a596-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3a596-181">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="3a596-181">The required password type.</span></span> <span data-ttu-id="3a596-182">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3a596-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3a596-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3a596-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3a596-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3a596-184">Int32</span></span>|<span data-ttu-id="3a596-185">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="3a596-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="3a596-186">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="3a596-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3a596-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3a596-187">osMinimumVersion</span></span>|<span data-ttu-id="3a596-188">String</span><span class="sxs-lookup"><span data-stu-id="3a596-188">String</span></span>|<span data-ttu-id="3a596-189">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="3a596-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="3a596-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3a596-190">osMaximumVersion</span></span>|<span data-ttu-id="3a596-191">String</span><span class="sxs-lookup"><span data-stu-id="3a596-191">String</span></span>|<span data-ttu-id="3a596-192">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="3a596-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="3a596-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3a596-193">storageRequireEncryption</span></span>|<span data-ttu-id="3a596-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a596-194">Boolean</span></span>|<span data-ttu-id="3a596-195">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="3a596-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="3a596-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a596-196">Response</span></span>
<span data-ttu-id="3a596-197">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3a596-197">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a596-198">Пример</span><span class="sxs-lookup"><span data-stu-id="3a596-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a596-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a596-199">Request</span></span>
<span data-ttu-id="3a596-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a596-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3a596-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a596-201">Response</span></span>
<span data-ttu-id="3a596-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3a596-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





