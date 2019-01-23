---
title: Обновление defaultDeviceCompliancePolicy
description: Обновление свойства объекта defaultDeviceCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67c8e736707b64ef2f6ebbeb89bdf2c54834ad35
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398942"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="62781-103">Обновление defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="62781-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="62781-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62781-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="62781-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62781-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62781-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62781-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62781-107">Обновление свойства объекта [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="62781-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62781-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="62781-108">Prerequisites</span></span>
<span data-ttu-id="62781-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="62781-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="62781-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62781-111">Permission type</span></span>|<span data-ttu-id="62781-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62781-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62781-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62781-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62781-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62781-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62781-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62781-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62781-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62781-116">Not supported.</span></span>|
|<span data-ttu-id="62781-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62781-117">Application</span></span>|<span data-ttu-id="62781-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62781-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62781-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62781-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="62781-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62781-120">Request headers</span></span>
|<span data-ttu-id="62781-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62781-121">Header</span></span>|<span data-ttu-id="62781-122">Значение</span><span class="sxs-lookup"><span data-stu-id="62781-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62781-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62781-123">Authorization</span></span>|<span data-ttu-id="62781-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="62781-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62781-125">Accept</span><span class="sxs-lookup"><span data-stu-id="62781-125">Accept</span></span>|<span data-ttu-id="62781-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62781-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62781-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62781-127">Request body</span></span>
<span data-ttu-id="62781-128">В тексте запроса укажите представление JSON для объекта [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="62781-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="62781-129">В следующей таблице показаны свойства, которые необходимы для создания [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62781-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="62781-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="62781-130">Property</span></span>|<span data-ttu-id="62781-131">Тип</span><span class="sxs-lookup"><span data-stu-id="62781-131">Type</span></span>|<span data-ttu-id="62781-132">Описание</span><span class="sxs-lookup"><span data-stu-id="62781-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62781-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62781-133">roleScopeTagIds</span></span>|<span data-ttu-id="62781-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="62781-134">String collection</span></span>|<span data-ttu-id="62781-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="62781-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="62781-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62781-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="62781-137">id</span><span class="sxs-lookup"><span data-stu-id="62781-137">id</span></span>|<span data-ttu-id="62781-138">String</span><span class="sxs-lookup"><span data-stu-id="62781-138">String</span></span>|<span data-ttu-id="62781-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="62781-139">Key of the entity.</span></span> <span data-ttu-id="62781-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62781-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="62781-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62781-141">createdDateTime</span></span>|<span data-ttu-id="62781-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62781-142">DateTimeOffset</span></span>|<span data-ttu-id="62781-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="62781-143">DateTime the object was created.</span></span> <span data-ttu-id="62781-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62781-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="62781-145">description</span><span class="sxs-lookup"><span data-stu-id="62781-145">description</span></span>|<span data-ttu-id="62781-146">String</span><span class="sxs-lookup"><span data-stu-id="62781-146">String</span></span>|<span data-ttu-id="62781-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="62781-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="62781-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62781-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="62781-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62781-149">lastModifiedDateTime</span></span>|<span data-ttu-id="62781-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62781-150">DateTimeOffset</span></span>|<span data-ttu-id="62781-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="62781-151">DateTime the object was last modified.</span></span> <span data-ttu-id="62781-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62781-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="62781-153">displayName</span><span class="sxs-lookup"><span data-stu-id="62781-153">displayName</span></span>|<span data-ttu-id="62781-154">String</span><span class="sxs-lookup"><span data-stu-id="62781-154">String</span></span>|<span data-ttu-id="62781-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="62781-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="62781-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62781-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="62781-157">version</span><span class="sxs-lookup"><span data-stu-id="62781-157">version</span></span>|<span data-ttu-id="62781-158">Int32</span><span class="sxs-lookup"><span data-stu-id="62781-158">Int32</span></span>|<span data-ttu-id="62781-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="62781-159">Version of the device configuration.</span></span> <span data-ttu-id="62781-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62781-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="62781-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="62781-161">Response</span></span>
<span data-ttu-id="62781-162">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="62781-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62781-163">Пример</span><span class="sxs-lookup"><span data-stu-id="62781-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="62781-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="62781-164">Request</span></span>
<span data-ttu-id="62781-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62781-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62781-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="62781-166">Response</span></span>
<span data-ttu-id="62781-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="62781-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




