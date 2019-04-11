---
title: Обновление Дефаултдевицекомплианцеполици
description: Обновление свойств объекта Дефаултдевицекомплианцеполици.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d69ebb9b07f5544f88e01980ca5684c2ce3dda8a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781969"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="e1c3b-103">Обновление Дефаултдевицекомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="e1c3b-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="e1c3b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1c3b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1c3b-106">Обновление свойств объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e1c3b-106">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1c3b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e1c3b-107">Prerequisites</span></span>
<span data-ttu-id="e1c3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1c3b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1c3b-110">Permission type</span></span>|<span data-ttu-id="e1c3b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1c3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1c3b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1c3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1c3b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1c3b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1c3b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1c3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1c3b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-115">Not supported.</span></span>|
|<span data-ttu-id="e1c3b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1c3b-116">Application</span></span>|<span data-ttu-id="e1c3b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1c3b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1c3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="e1c3b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1c3b-119">Request headers</span></span>
|<span data-ttu-id="e1c3b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1c3b-120">Header</span></span>|<span data-ttu-id="e1c3b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e1c3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1c3b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1c3b-122">Authorization</span></span>|<span data-ttu-id="e1c3b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1c3b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e1c3b-124">Accept</span></span>|<span data-ttu-id="e1c3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1c3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1c3b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1c3b-126">Request body</span></span>
<span data-ttu-id="e1c3b-127">В тексте запроса добавьте представление объекта [Дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-127">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="e1c3b-128">В следующей таблице приведены свойства, необходимые при создании [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-128">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="e1c3b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1c3b-129">Property</span></span>|<span data-ttu-id="e1c3b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e1c3b-130">Type</span></span>|<span data-ttu-id="e1c3b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e1c3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1c3b-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e1c3b-132">roleScopeTagIds</span></span>|<span data-ttu-id="e1c3b-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e1c3b-133">String collection</span></span>|<span data-ttu-id="e1c3b-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e1c3b-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1c3b-136">id</span><span class="sxs-lookup"><span data-stu-id="e1c3b-136">id</span></span>|<span data-ttu-id="e1c3b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e1c3b-137">String</span></span>|<span data-ttu-id="e1c3b-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-138">Key of the entity.</span></span> <span data-ttu-id="e1c3b-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1c3b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1c3b-140">createdDateTime</span></span>|<span data-ttu-id="e1c3b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1c3b-141">DateTimeOffset</span></span>|<span data-ttu-id="e1c3b-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-142">DateTime the object was created.</span></span> <span data-ttu-id="e1c3b-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1c3b-144">description</span><span class="sxs-lookup"><span data-stu-id="e1c3b-144">description</span></span>|<span data-ttu-id="e1c3b-145">String</span><span class="sxs-lookup"><span data-stu-id="e1c3b-145">String</span></span>|<span data-ttu-id="e1c3b-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e1c3b-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1c3b-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1c3b-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e1c3b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1c3b-149">DateTimeOffset</span></span>|<span data-ttu-id="e1c3b-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-150">DateTime the object was last modified.</span></span> <span data-ttu-id="e1c3b-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1c3b-152">displayName</span><span class="sxs-lookup"><span data-stu-id="e1c3b-152">displayName</span></span>|<span data-ttu-id="e1c3b-153">String</span><span class="sxs-lookup"><span data-stu-id="e1c3b-153">String</span></span>|<span data-ttu-id="e1c3b-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e1c3b-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1c3b-156">version</span><span class="sxs-lookup"><span data-stu-id="e1c3b-156">version</span></span>|<span data-ttu-id="e1c3b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e1c3b-157">Int32</span></span>|<span data-ttu-id="e1c3b-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-158">Version of the device configuration.</span></span> <span data-ttu-id="e1c3b-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e1c3b-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1c3b-160">Response</span></span>
<span data-ttu-id="e1c3b-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-161">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1c3b-162">Пример</span><span class="sxs-lookup"><span data-stu-id="e1c3b-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1c3b-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1c3b-163">Request</span></span>
<span data-ttu-id="e1c3b-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e1c3b-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1c3b-165">Response</span></span>
<span data-ttu-id="e1c3b-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





