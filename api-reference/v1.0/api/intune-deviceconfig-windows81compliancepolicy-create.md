---
title: Создание объекта windows81CompliancePolicy
description: Создание объекта windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6a141025a592a322dec6cd5ba5aeb802c04878f5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020068"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="0b162-103">Создание объекта windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0b162-103">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="0b162-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b162-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b162-105">Создание объекта [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0b162-105">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b162-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0b162-106">Prerequisites</span></span>
<span data-ttu-id="0b162-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b162-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b162-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b162-109">Permission type</span></span>|<span data-ttu-id="0b162-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b162-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b162-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b162-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b162-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b162-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b162-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b162-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b162-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b162-114">Not supported.</span></span>|
|<span data-ttu-id="0b162-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b162-115">Application</span></span>|<span data-ttu-id="0b162-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b162-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b162-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b162-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0b162-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b162-118">Request headers</span></span>
|<span data-ttu-id="0b162-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b162-119">Header</span></span>|<span data-ttu-id="0b162-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0b162-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b162-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b162-121">Authorization</span></span>|<span data-ttu-id="0b162-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b162-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b162-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0b162-123">Accept</span></span>|<span data-ttu-id="0b162-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0b162-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b162-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b162-125">Request body</span></span>
<span data-ttu-id="0b162-126">В теле запроса добавьте представление объекта windows81CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b162-126">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="0b162-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="0b162-127">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="0b162-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b162-128">Property</span></span>|<span data-ttu-id="0b162-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0b162-129">Type</span></span>|<span data-ttu-id="0b162-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0b162-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b162-131">id</span><span class="sxs-lookup"><span data-stu-id="0b162-131">id</span></span>|<span data-ttu-id="0b162-132">Строка</span><span class="sxs-lookup"><span data-stu-id="0b162-132">String</span></span>|<span data-ttu-id="0b162-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0b162-133">Key of the entity.</span></span> <span data-ttu-id="0b162-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0b162-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b162-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b162-135">createdDateTime</span></span>|<span data-ttu-id="0b162-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b162-136">DateTimeOffset</span></span>|<span data-ttu-id="0b162-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0b162-137">DateTime the object was created.</span></span> <span data-ttu-id="0b162-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0b162-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b162-139">description</span><span class="sxs-lookup"><span data-stu-id="0b162-139">description</span></span>|<span data-ttu-id="0b162-140">String</span><span class="sxs-lookup"><span data-stu-id="0b162-140">String</span></span>|<span data-ttu-id="0b162-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0b162-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0b162-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0b162-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b162-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b162-143">lastModifiedDateTime</span></span>|<span data-ttu-id="0b162-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b162-144">DateTimeOffset</span></span>|<span data-ttu-id="0b162-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0b162-145">DateTime the object was last modified.</span></span> <span data-ttu-id="0b162-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0b162-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b162-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0b162-147">displayName</span></span>|<span data-ttu-id="0b162-148">Строка</span><span class="sxs-lookup"><span data-stu-id="0b162-148">String</span></span>|<span data-ttu-id="0b162-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0b162-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0b162-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0b162-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b162-151">version</span><span class="sxs-lookup"><span data-stu-id="0b162-151">version</span></span>|<span data-ttu-id="0b162-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0b162-152">Int32</span></span>|<span data-ttu-id="0b162-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0b162-153">Version of the device configuration.</span></span> <span data-ttu-id="0b162-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0b162-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b162-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0b162-155">passwordRequired</span></span>|<span data-ttu-id="0b162-156">Логический</span><span class="sxs-lookup"><span data-stu-id="0b162-156">Boolean</span></span>|<span data-ttu-id="0b162-157">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="0b162-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="0b162-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0b162-158">passwordBlockSimple</span></span>|<span data-ttu-id="0b162-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b162-159">Boolean</span></span>|<span data-ttu-id="0b162-160">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="0b162-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="0b162-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0b162-161">passwordExpirationDays</span></span>|<span data-ttu-id="0b162-162">Int32</span><span class="sxs-lookup"><span data-stu-id="0b162-162">Int32</span></span>|<span data-ttu-id="0b162-163">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="0b162-163">Password expiration in days.</span></span>|
|<span data-ttu-id="0b162-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0b162-164">passwordMinimumLength</span></span>|<span data-ttu-id="0b162-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0b162-165">Int32</span></span>|<span data-ttu-id="0b162-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="0b162-166">The minimum password length.</span></span>|
|<span data-ttu-id="0b162-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0b162-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0b162-168">Int32</span><span class="sxs-lookup"><span data-stu-id="0b162-168">Int32</span></span>|<span data-ttu-id="0b162-169">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="0b162-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0b162-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0b162-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0b162-171">Int32</span><span class="sxs-lookup"><span data-stu-id="0b162-171">Int32</span></span>|<span data-ttu-id="0b162-172">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="0b162-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0b162-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0b162-173">passwordRequiredType</span></span>|[<span data-ttu-id="0b162-174">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="0b162-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0b162-175">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="0b162-175">The required password type.</span></span> <span data-ttu-id="0b162-176">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0b162-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0b162-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0b162-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0b162-178">Int32</span><span class="sxs-lookup"><span data-stu-id="0b162-178">Int32</span></span>|<span data-ttu-id="0b162-179">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="0b162-179">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="0b162-180">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="0b162-180">Valid values 0 to 24</span></span>|
|<span data-ttu-id="0b162-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0b162-181">osMinimumVersion</span></span>|<span data-ttu-id="0b162-182">String</span><span class="sxs-lookup"><span data-stu-id="0b162-182">String</span></span>|<span data-ttu-id="0b162-183">Минимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="0b162-183">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="0b162-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0b162-184">osMaximumVersion</span></span>|<span data-ttu-id="0b162-185">String</span><span class="sxs-lookup"><span data-stu-id="0b162-185">String</span></span>|<span data-ttu-id="0b162-186">Максимальная версия Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="0b162-186">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="0b162-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0b162-187">storageRequireEncryption</span></span>|<span data-ttu-id="0b162-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b162-188">Boolean</span></span>|<span data-ttu-id="0b162-189">Указывает, обязательно ли шифрование данных на устройстве с Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="0b162-189">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="0b162-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b162-190">Response</span></span>
<span data-ttu-id="0b162-191">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b162-191">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b162-192">Пример</span><span class="sxs-lookup"><span data-stu-id="0b162-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b162-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b162-193">Request</span></span>
<span data-ttu-id="0b162-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b162-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="0b162-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b162-195">Response</span></span>
<span data-ttu-id="0b162-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b162-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
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



