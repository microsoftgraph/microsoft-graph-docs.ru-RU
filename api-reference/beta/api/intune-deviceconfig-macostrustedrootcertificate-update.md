---
title: Обновление macOSTrustedRootCertificate
description: Обновление свойства объекта macOSTrustedRootCertificate.
ms.openlocfilehash: b3a859cbc5218a24b1d1ebd13dfd9f6c5260fec7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074706"
---
# <a name="update-macostrustedrootcertificate"></a><span data-ttu-id="c2c73-103">Обновление macOSTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c2c73-103">Update macOSTrustedRootCertificate</span></span>

> <span data-ttu-id="c2c73-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2c73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2c73-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2c73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2c73-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2c73-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2c73-107">Обновление свойства объекта [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="c2c73-107">Update the properties of a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2c73-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2c73-108">Prerequisites</span></span>
<span data-ttu-id="c2c73-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2c73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2c73-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2c73-111">Permission type</span></span>|<span data-ttu-id="c2c73-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2c73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2c73-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2c73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2c73-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2c73-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2c73-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2c73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2c73-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2c73-116">Not supported.</span></span>|
|<span data-ttu-id="c2c73-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2c73-117">Application</span></span>|<span data-ttu-id="c2c73-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2c73-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2c73-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2c73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="c2c73-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2c73-120">Request headers</span></span>
|<span data-ttu-id="c2c73-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2c73-121">Header</span></span>|<span data-ttu-id="c2c73-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2c73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2c73-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2c73-123">Authorization</span></span>|<span data-ttu-id="c2c73-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c2c73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2c73-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2c73-125">Accept</span></span>|<span data-ttu-id="c2c73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2c73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2c73-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2c73-127">Request body</span></span>
<span data-ttu-id="c2c73-128">В тексте запроса укажите представление JSON для объекта [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="c2c73-128">In the request body, supply a JSON representation for the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="c2c73-129">В следующей таблице показаны свойства, которые необходимы для создания [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="c2c73-129">The following table shows the properties that are required when you create the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="c2c73-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2c73-130">Property</span></span>|<span data-ttu-id="c2c73-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c2c73-131">Type</span></span>|<span data-ttu-id="c2c73-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c2c73-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2c73-133">id</span><span class="sxs-lookup"><span data-stu-id="c2c73-133">id</span></span>|<span data-ttu-id="c2c73-134">String</span><span class="sxs-lookup"><span data-stu-id="c2c73-134">String</span></span>|<span data-ttu-id="c2c73-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c2c73-135">Key of the entity.</span></span> <span data-ttu-id="c2c73-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2c73-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2c73-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2c73-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c2c73-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2c73-138">DateTimeOffset</span></span>|<span data-ttu-id="c2c73-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c2c73-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c2c73-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2c73-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2c73-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c2c73-141">roleScopeTagIds</span></span>|<span data-ttu-id="c2c73-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c2c73-142">String collection</span></span>|<span data-ttu-id="c2c73-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c2c73-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c2c73-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2c73-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2c73-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c2c73-145">supportsScopeTags</span></span>|<span data-ttu-id="c2c73-146">Логический</span><span class="sxs-lookup"><span data-stu-id="c2c73-146">Boolean</span></span>|<span data-ttu-id="c2c73-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="c2c73-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c2c73-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="c2c73-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c2c73-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c2c73-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c2c73-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2c73-150">This property is read-only.</span></span> <span data-ttu-id="c2c73-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2c73-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2c73-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2c73-152">createdDateTime</span></span>|<span data-ttu-id="c2c73-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2c73-153">DateTimeOffset</span></span>|<span data-ttu-id="c2c73-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c2c73-154">DateTime the object was created.</span></span> <span data-ttu-id="c2c73-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2c73-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2c73-156">описание</span><span class="sxs-lookup"><span data-stu-id="c2c73-156">description</span></span>|<span data-ttu-id="c2c73-157">String</span><span class="sxs-lookup"><span data-stu-id="c2c73-157">String</span></span>|<span data-ttu-id="c2c73-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c2c73-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c2c73-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2c73-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2c73-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c2c73-160">displayName</span></span>|<span data-ttu-id="c2c73-161">String</span><span class="sxs-lookup"><span data-stu-id="c2c73-161">String</span></span>|<span data-ttu-id="c2c73-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c2c73-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c2c73-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2c73-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2c73-164">version</span><span class="sxs-lookup"><span data-stu-id="c2c73-164">version</span></span>|<span data-ttu-id="c2c73-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c2c73-165">Int32</span></span>|<span data-ttu-id="c2c73-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c2c73-166">Version of the device configuration.</span></span> <span data-ttu-id="c2c73-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2c73-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2c73-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c2c73-168">trustedRootCertificate</span></span>|<span data-ttu-id="c2c73-169">Двоичный</span><span class="sxs-lookup"><span data-stu-id="c2c73-169">Binary</span></span>|<span data-ttu-id="c2c73-170">Доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="c2c73-170">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="c2c73-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="c2c73-171">certFileName</span></span>|<span data-ttu-id="c2c73-172">String</span><span class="sxs-lookup"><span data-stu-id="c2c73-172">String</span></span>|<span data-ttu-id="c2c73-173">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="c2c73-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="c2c73-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2c73-174">Response</span></span>
<span data-ttu-id="c2c73-175">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c2c73-175">If successful, this method returns a `200 OK` response code and an updated [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2c73-176">Пример</span><span class="sxs-lookup"><span data-stu-id="c2c73-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2c73-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2c73-177">Request</span></span>
<span data-ttu-id="c2c73-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2c73-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 363

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="c2c73-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2c73-179">Response</span></span>
<span data-ttu-id="c2c73-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c2c73-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 537

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "id": "c5fac954-c954-c5fa-54c9-fac554c9fac5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```





