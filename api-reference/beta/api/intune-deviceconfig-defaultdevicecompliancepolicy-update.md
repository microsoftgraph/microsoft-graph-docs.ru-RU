---
title: Обновление defaultDeviceCompliancePolicy
description: Обновление свойств объекта defaultDeviceCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7eb64c52fc7680c995ac4a3f0d497be8974dc3de
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155710"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="9a01c-103">Обновление defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9a01c-103">Update defaultDeviceCompliancePolicy</span></span>

<span data-ttu-id="9a01c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a01c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a01c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a01c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a01c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a01c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a01c-107">Обновление свойств объекта [defaultDeviceCompliancePolicy.](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a01c-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a01c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9a01c-108">Prerequisites</span></span>
<span data-ttu-id="9a01c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a01c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a01c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a01c-111">Permission type</span></span>|<span data-ttu-id="9a01c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a01c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a01c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a01c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a01c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a01c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a01c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a01c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a01c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a01c-116">Not supported.</span></span>|
|<span data-ttu-id="9a01c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9a01c-117">Application</span></span>|<span data-ttu-id="9a01c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a01c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a01c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a01c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9a01c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9a01c-120">Request headers</span></span>
|<span data-ttu-id="9a01c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a01c-121">Header</span></span>|<span data-ttu-id="9a01c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9a01c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a01c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a01c-123">Authorization</span></span>|<span data-ttu-id="9a01c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a01c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a01c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a01c-125">Accept</span></span>|<span data-ttu-id="9a01c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a01c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a01c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a01c-127">Request body</span></span>
<span data-ttu-id="9a01c-128">В теле запроса поставляем представление JSON для объекта [defaultDeviceCompliancePolicy.](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a01c-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="9a01c-129">В следующей таблице показаны свойства, необходимые при создании [defaultDeviceCompliancePolicy.](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a01c-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="9a01c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a01c-130">Property</span></span>|<span data-ttu-id="9a01c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9a01c-131">Type</span></span>|<span data-ttu-id="9a01c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9a01c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a01c-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9a01c-133">roleScopeTagIds</span></span>|<span data-ttu-id="9a01c-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9a01c-134">String collection</span></span>|<span data-ttu-id="9a01c-135">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="9a01c-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9a01c-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9a01c-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a01c-137">id</span><span class="sxs-lookup"><span data-stu-id="9a01c-137">id</span></span>|<span data-ttu-id="9a01c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="9a01c-138">String</span></span>|<span data-ttu-id="9a01c-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9a01c-139">Key of the entity.</span></span> <span data-ttu-id="9a01c-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9a01c-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a01c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a01c-141">createdDateTime</span></span>|<span data-ttu-id="9a01c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a01c-142">DateTimeOffset</span></span>|<span data-ttu-id="9a01c-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9a01c-143">DateTime the object was created.</span></span> <span data-ttu-id="9a01c-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9a01c-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a01c-145">description</span><span class="sxs-lookup"><span data-stu-id="9a01c-145">description</span></span>|<span data-ttu-id="9a01c-146">Строка</span><span class="sxs-lookup"><span data-stu-id="9a01c-146">String</span></span>|<span data-ttu-id="9a01c-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9a01c-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9a01c-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9a01c-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a01c-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a01c-149">lastModifiedDateTime</span></span>|<span data-ttu-id="9a01c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a01c-150">DateTimeOffset</span></span>|<span data-ttu-id="9a01c-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9a01c-151">DateTime the object was last modified.</span></span> <span data-ttu-id="9a01c-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9a01c-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a01c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="9a01c-153">displayName</span></span>|<span data-ttu-id="9a01c-154">Строка</span><span class="sxs-lookup"><span data-stu-id="9a01c-154">String</span></span>|<span data-ttu-id="9a01c-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9a01c-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9a01c-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9a01c-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a01c-157">version</span><span class="sxs-lookup"><span data-stu-id="9a01c-157">version</span></span>|<span data-ttu-id="9a01c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9a01c-158">Int32</span></span>|<span data-ttu-id="9a01c-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9a01c-159">Version of the device configuration.</span></span> <span data-ttu-id="9a01c-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9a01c-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9a01c-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a01c-161">Response</span></span>
<span data-ttu-id="9a01c-162">В случае успешного использования этот метод возвращает код ответа и обновленный объект `200 OK` [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9a01c-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a01c-163">Пример</span><span class="sxs-lookup"><span data-stu-id="9a01c-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a01c-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a01c-164">Request</span></span>
<span data-ttu-id="9a01c-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a01c-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 229

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="9a01c-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a01c-166">Response</span></span>
<span data-ttu-id="9a01c-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a01c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




