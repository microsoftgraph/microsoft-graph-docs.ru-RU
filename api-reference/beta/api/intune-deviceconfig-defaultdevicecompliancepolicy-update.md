---
title: Обновление Дефаултдевицекомплианцеполици
description: Обновление свойств объекта Дефаултдевицекомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fdfb957022d66a4e4e18209d6ba9b8a3c0e776f0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949807"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="24856-103">Обновление Дефаултдевицекомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="24856-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="24856-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24856-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24856-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24856-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24856-106">Обновление свойств объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="24856-106">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24856-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24856-107">Prerequisites</span></span>
<span data-ttu-id="24856-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24856-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24856-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24856-110">Permission type</span></span>|<span data-ttu-id="24856-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24856-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24856-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24856-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24856-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24856-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24856-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24856-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24856-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24856-115">Not supported.</span></span>|
|<span data-ttu-id="24856-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24856-116">Application</span></span>|<span data-ttu-id="24856-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24856-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24856-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24856-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="24856-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24856-119">Request headers</span></span>
|<span data-ttu-id="24856-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24856-120">Header</span></span>|<span data-ttu-id="24856-121">Значение</span><span class="sxs-lookup"><span data-stu-id="24856-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24856-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24856-122">Authorization</span></span>|<span data-ttu-id="24856-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24856-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24856-124">Accept</span><span class="sxs-lookup"><span data-stu-id="24856-124">Accept</span></span>|<span data-ttu-id="24856-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24856-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24856-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24856-126">Request body</span></span>
<span data-ttu-id="24856-127">В тексте запроса добавьте представление объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24856-127">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="24856-128">В следующей таблице приведены свойства, необходимые при создании [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24856-128">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="24856-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="24856-129">Property</span></span>|<span data-ttu-id="24856-130">Тип</span><span class="sxs-lookup"><span data-stu-id="24856-130">Type</span></span>|<span data-ttu-id="24856-131">Описание</span><span class="sxs-lookup"><span data-stu-id="24856-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24856-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="24856-132">roleScopeTagIds</span></span>|<span data-ttu-id="24856-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="24856-133">String collection</span></span>|<span data-ttu-id="24856-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="24856-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="24856-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24856-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24856-136">id</span><span class="sxs-lookup"><span data-stu-id="24856-136">id</span></span>|<span data-ttu-id="24856-137">String</span><span class="sxs-lookup"><span data-stu-id="24856-137">String</span></span>|<span data-ttu-id="24856-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="24856-138">Key of the entity.</span></span> <span data-ttu-id="24856-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24856-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24856-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24856-140">createdDateTime</span></span>|<span data-ttu-id="24856-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24856-141">DateTimeOffset</span></span>|<span data-ttu-id="24856-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="24856-142">DateTime the object was created.</span></span> <span data-ttu-id="24856-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24856-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24856-144">description</span><span class="sxs-lookup"><span data-stu-id="24856-144">description</span></span>|<span data-ttu-id="24856-145">String</span><span class="sxs-lookup"><span data-stu-id="24856-145">String</span></span>|<span data-ttu-id="24856-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="24856-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="24856-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24856-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24856-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24856-148">lastModifiedDateTime</span></span>|<span data-ttu-id="24856-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24856-149">DateTimeOffset</span></span>|<span data-ttu-id="24856-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="24856-150">DateTime the object was last modified.</span></span> <span data-ttu-id="24856-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24856-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24856-152">displayName</span><span class="sxs-lookup"><span data-stu-id="24856-152">displayName</span></span>|<span data-ttu-id="24856-153">Строка</span><span class="sxs-lookup"><span data-stu-id="24856-153">String</span></span>|<span data-ttu-id="24856-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="24856-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="24856-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24856-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24856-156">version</span><span class="sxs-lookup"><span data-stu-id="24856-156">version</span></span>|<span data-ttu-id="24856-157">Int32</span><span class="sxs-lookup"><span data-stu-id="24856-157">Int32</span></span>|<span data-ttu-id="24856-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="24856-158">Version of the device configuration.</span></span> <span data-ttu-id="24856-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24856-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="24856-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="24856-160">Response</span></span>
<span data-ttu-id="24856-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24856-161">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24856-162">Пример</span><span class="sxs-lookup"><span data-stu-id="24856-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="24856-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="24856-163">Request</span></span>
<span data-ttu-id="24856-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24856-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="24856-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="24856-165">Response</span></span>
<span data-ttu-id="24856-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24856-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





