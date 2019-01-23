---
title: Обновление iosTrustedRootCertificate
description: Обновление свойства объекта iosTrustedRootCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0b187a3dde0e5fab752319d6edb83fe5ea6e801
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405074"
---
# <a name="update-iostrustedrootcertificate"></a><span data-ttu-id="ae716-103">Обновление iosTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ae716-103">Update iosTrustedRootCertificate</span></span>

> <span data-ttu-id="ae716-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ae716-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae716-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae716-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae716-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae716-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae716-107">Обновление свойства объекта [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ae716-107">Update the properties of a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae716-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="ae716-108">Prerequisites</span></span>
<span data-ttu-id="ae716-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae716-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae716-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae716-111">Permission type</span></span>|<span data-ttu-id="ae716-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae716-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae716-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae716-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae716-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae716-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae716-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae716-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae716-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae716-116">Not supported.</span></span>|
|<span data-ttu-id="ae716-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae716-117">Application</span></span>|<span data-ttu-id="ae716-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae716-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae716-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae716-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation/{iosTrustedRootCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="ae716-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae716-120">Request headers</span></span>
|<span data-ttu-id="ae716-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae716-121">Header</span></span>|<span data-ttu-id="ae716-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ae716-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae716-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae716-123">Authorization</span></span>|<span data-ttu-id="ae716-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ae716-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae716-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ae716-125">Accept</span></span>|<span data-ttu-id="ae716-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae716-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae716-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae716-127">Request body</span></span>
<span data-ttu-id="ae716-128">В тексте запроса укажите представление JSON для объекта [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ae716-128">In the request body, supply a JSON representation for the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="ae716-129">В следующей таблице показаны свойства, которые необходимы для создания [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="ae716-129">The following table shows the properties that are required when you create the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="ae716-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae716-130">Property</span></span>|<span data-ttu-id="ae716-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ae716-131">Type</span></span>|<span data-ttu-id="ae716-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ae716-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae716-133">id</span><span class="sxs-lookup"><span data-stu-id="ae716-133">id</span></span>|<span data-ttu-id="ae716-134">String</span><span class="sxs-lookup"><span data-stu-id="ae716-134">String</span></span>|<span data-ttu-id="ae716-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ae716-135">Key of the entity.</span></span> <span data-ttu-id="ae716-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae716-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae716-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae716-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ae716-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae716-138">DateTimeOffset</span></span>|<span data-ttu-id="ae716-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ae716-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ae716-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae716-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae716-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ae716-141">roleScopeTagIds</span></span>|<span data-ttu-id="ae716-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ae716-142">String collection</span></span>|<span data-ttu-id="ae716-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ae716-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ae716-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae716-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae716-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ae716-145">supportsScopeTags</span></span>|<span data-ttu-id="ae716-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ae716-146">Boolean</span></span>|<span data-ttu-id="ae716-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="ae716-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ae716-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="ae716-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ae716-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ae716-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ae716-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae716-150">This property is read-only.</span></span> <span data-ttu-id="ae716-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae716-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae716-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae716-152">createdDateTime</span></span>|<span data-ttu-id="ae716-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae716-153">DateTimeOffset</span></span>|<span data-ttu-id="ae716-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ae716-154">DateTime the object was created.</span></span> <span data-ttu-id="ae716-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae716-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae716-156">description</span><span class="sxs-lookup"><span data-stu-id="ae716-156">description</span></span>|<span data-ttu-id="ae716-157">String</span><span class="sxs-lookup"><span data-stu-id="ae716-157">String</span></span>|<span data-ttu-id="ae716-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ae716-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ae716-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae716-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae716-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ae716-160">displayName</span></span>|<span data-ttu-id="ae716-161">String</span><span class="sxs-lookup"><span data-stu-id="ae716-161">String</span></span>|<span data-ttu-id="ae716-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ae716-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ae716-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae716-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae716-164">version</span><span class="sxs-lookup"><span data-stu-id="ae716-164">version</span></span>|<span data-ttu-id="ae716-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ae716-165">Int32</span></span>|<span data-ttu-id="ae716-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ae716-166">Version of the device configuration.</span></span> <span data-ttu-id="ae716-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae716-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae716-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ae716-168">trustedRootCertificate</span></span>|<span data-ttu-id="ae716-169">Binary</span><span class="sxs-lookup"><span data-stu-id="ae716-169">Binary</span></span>|<span data-ttu-id="ae716-170">Доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="ae716-170">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="ae716-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="ae716-171">certFileName</span></span>|<span data-ttu-id="ae716-172">String</span><span class="sxs-lookup"><span data-stu-id="ae716-172">String</span></span>|<span data-ttu-id="ae716-173">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="ae716-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="ae716-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae716-174">Response</span></span>
<span data-ttu-id="ae716-175">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ae716-175">If successful, this method returns a `200 OK` response code and an updated [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae716-176">Пример</span><span class="sxs-lookup"><span data-stu-id="ae716-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae716-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae716-177">Request</span></span>
<span data-ttu-id="ae716-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae716-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="ae716-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae716-179">Response</span></span>
<span data-ttu-id="ae716-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ae716-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
  "id": "9bc72bb8-2bb8-9bc7-b82b-c79bb82bc79b",
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




