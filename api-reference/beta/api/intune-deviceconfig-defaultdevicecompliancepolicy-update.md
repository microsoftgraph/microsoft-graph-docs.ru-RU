---
title: Обновление defaultDeviceCompliancePolicy
description: Обновление свойства объекта defaultDeviceCompliancePolicy.
ms.openlocfilehash: 65dcf950a1d8f3bbcbbb19b4132713bfb13b5153
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081825"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="cae35-103">Обновление defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="cae35-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="cae35-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cae35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cae35-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae35-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cae35-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cae35-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cae35-107">Обновление свойства объекта [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="cae35-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cae35-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cae35-108">Prerequisites</span></span>
<span data-ttu-id="cae35-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cae35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae35-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae35-111">Permission type</span></span>|<span data-ttu-id="cae35-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cae35-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cae35-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cae35-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cae35-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cae35-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cae35-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae35-116">Not supported.</span></span>|
|<span data-ttu-id="cae35-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cae35-117">Application</span></span>|<span data-ttu-id="cae35-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae35-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cae35-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cae35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="cae35-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cae35-120">Request headers</span></span>
|<span data-ttu-id="cae35-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cae35-121">Header</span></span>|<span data-ttu-id="cae35-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cae35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cae35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cae35-123">Authorization</span></span>|<span data-ttu-id="cae35-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cae35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cae35-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cae35-125">Accept</span></span>|<span data-ttu-id="cae35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cae35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cae35-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cae35-127">Request body</span></span>
<span data-ttu-id="cae35-128">В тексте запроса укажите представление JSON для объекта [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="cae35-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="cae35-129">В следующей таблице показаны свойства, которые необходимы для создания [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cae35-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="cae35-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cae35-130">Property</span></span>|<span data-ttu-id="cae35-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cae35-131">Type</span></span>|<span data-ttu-id="cae35-132">Description</span><span class="sxs-lookup"><span data-stu-id="cae35-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cae35-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cae35-133">roleScopeTagIds</span></span>|<span data-ttu-id="cae35-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cae35-134">String collection</span></span>|<span data-ttu-id="cae35-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cae35-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cae35-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cae35-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cae35-137">id</span><span class="sxs-lookup"><span data-stu-id="cae35-137">id</span></span>|<span data-ttu-id="cae35-138">String</span><span class="sxs-lookup"><span data-stu-id="cae35-138">String</span></span>|<span data-ttu-id="cae35-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cae35-139">Key of the entity.</span></span> <span data-ttu-id="cae35-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cae35-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cae35-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cae35-141">createdDateTime</span></span>|<span data-ttu-id="cae35-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cae35-142">DateTimeOffset</span></span>|<span data-ttu-id="cae35-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cae35-143">DateTime the object was created.</span></span> <span data-ttu-id="cae35-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cae35-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cae35-145">описание</span><span class="sxs-lookup"><span data-stu-id="cae35-145">description</span></span>|<span data-ttu-id="cae35-146">String</span><span class="sxs-lookup"><span data-stu-id="cae35-146">String</span></span>|<span data-ttu-id="cae35-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cae35-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cae35-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cae35-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cae35-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cae35-149">lastModifiedDateTime</span></span>|<span data-ttu-id="cae35-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cae35-150">DateTimeOffset</span></span>|<span data-ttu-id="cae35-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cae35-151">DateTime the object was last modified.</span></span> <span data-ttu-id="cae35-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cae35-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cae35-153">displayName</span><span class="sxs-lookup"><span data-stu-id="cae35-153">displayName</span></span>|<span data-ttu-id="cae35-154">String</span><span class="sxs-lookup"><span data-stu-id="cae35-154">String</span></span>|<span data-ttu-id="cae35-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cae35-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cae35-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cae35-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cae35-157">version</span><span class="sxs-lookup"><span data-stu-id="cae35-157">version</span></span>|<span data-ttu-id="cae35-158">Int32</span><span class="sxs-lookup"><span data-stu-id="cae35-158">Int32</span></span>|<span data-ttu-id="cae35-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cae35-159">Version of the device configuration.</span></span> <span data-ttu-id="cae35-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cae35-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="cae35-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="cae35-161">Response</span></span>
<span data-ttu-id="cae35-162">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cae35-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cae35-163">Пример</span><span class="sxs-lookup"><span data-stu-id="cae35-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="cae35-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae35-164">Request</span></span>
<span data-ttu-id="cae35-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cae35-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 225

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="cae35-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="cae35-166">Response</span></span>
<span data-ttu-id="cae35-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cae35-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a285f027-f027-a285-27f0-85a227f085a2",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```





