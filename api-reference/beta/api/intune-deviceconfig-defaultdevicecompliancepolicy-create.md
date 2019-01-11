---
title: Создание defaultDeviceCompliancePolicy
description: Создание нового объекта defaultDeviceCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a69c83e9de07f2e809e53f449d3f9686e238a138
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886781"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="8340c-103">Создание defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8340c-103">Create defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="8340c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8340c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8340c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8340c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8340c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8340c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8340c-107">Создание нового объекта [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8340c-107">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8340c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8340c-108">Prerequisites</span></span>
<span data-ttu-id="8340c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8340c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8340c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8340c-111">Permission type</span></span>|<span data-ttu-id="8340c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8340c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8340c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8340c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8340c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8340c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8340c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8340c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8340c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8340c-116">Not supported.</span></span>|
|<span data-ttu-id="8340c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8340c-117">Application</span></span>|<span data-ttu-id="8340c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8340c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8340c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8340c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8340c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8340c-120">Request headers</span></span>
|<span data-ttu-id="8340c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8340c-121">Header</span></span>|<span data-ttu-id="8340c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8340c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8340c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8340c-123">Authorization</span></span>|<span data-ttu-id="8340c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8340c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8340c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8340c-125">Accept</span></span>|<span data-ttu-id="8340c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8340c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8340c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8340c-127">Request body</span></span>
<span data-ttu-id="8340c-128">В тексте запроса укажите представление JSON для объекта defaultDeviceCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="8340c-128">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="8340c-129">В следующей таблице показаны свойства, которые необходимы для создания defaultDeviceCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="8340c-129">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="8340c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8340c-130">Property</span></span>|<span data-ttu-id="8340c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8340c-131">Type</span></span>|<span data-ttu-id="8340c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8340c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8340c-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8340c-133">roleScopeTagIds</span></span>|<span data-ttu-id="8340c-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8340c-134">String collection</span></span>|<span data-ttu-id="8340c-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8340c-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8340c-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8340c-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8340c-137">id</span><span class="sxs-lookup"><span data-stu-id="8340c-137">id</span></span>|<span data-ttu-id="8340c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="8340c-138">String</span></span>|<span data-ttu-id="8340c-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8340c-139">Key of the entity.</span></span> <span data-ttu-id="8340c-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8340c-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8340c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8340c-141">createdDateTime</span></span>|<span data-ttu-id="8340c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8340c-142">DateTimeOffset</span></span>|<span data-ttu-id="8340c-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8340c-143">DateTime the object was created.</span></span> <span data-ttu-id="8340c-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8340c-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8340c-145">описание</span><span class="sxs-lookup"><span data-stu-id="8340c-145">description</span></span>|<span data-ttu-id="8340c-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8340c-146">String</span></span>|<span data-ttu-id="8340c-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8340c-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8340c-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8340c-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8340c-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8340c-149">lastModifiedDateTime</span></span>|<span data-ttu-id="8340c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8340c-150">DateTimeOffset</span></span>|<span data-ttu-id="8340c-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8340c-151">DateTime the object was last modified.</span></span> <span data-ttu-id="8340c-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8340c-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8340c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="8340c-153">displayName</span></span>|<span data-ttu-id="8340c-154">Строка</span><span class="sxs-lookup"><span data-stu-id="8340c-154">String</span></span>|<span data-ttu-id="8340c-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8340c-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8340c-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8340c-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8340c-157">version</span><span class="sxs-lookup"><span data-stu-id="8340c-157">version</span></span>|<span data-ttu-id="8340c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8340c-158">Int32</span></span>|<span data-ttu-id="8340c-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8340c-159">Version of the device configuration.</span></span> <span data-ttu-id="8340c-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8340c-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8340c-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="8340c-161">Response</span></span>
<span data-ttu-id="8340c-162">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8340c-162">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8340c-163">Пример</span><span class="sxs-lookup"><span data-stu-id="8340c-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="8340c-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="8340c-164">Request</span></span>
<span data-ttu-id="8340c-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8340c-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 293

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="8340c-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="8340c-166">Response</span></span>
<span data-ttu-id="8340c-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8340c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





