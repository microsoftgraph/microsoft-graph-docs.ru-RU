---
title: Обновление windowsPhone81TrustedRootCertificate
description: Обновление свойства объекта windowsPhone81TrustedRootCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dd1445764cabb9280778c2db5a61021cefc0ce9f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396492"
---
# <a name="update-windowsphone81trustedrootcertificate"></a><span data-ttu-id="97b24-103">Обновление windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="97b24-103">Update windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="97b24-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="97b24-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="97b24-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97b24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97b24-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97b24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97b24-107">Обновление свойства объекта [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="97b24-107">Update the properties of a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97b24-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="97b24-108">Prerequisites</span></span>
<span data-ttu-id="97b24-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="97b24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="97b24-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97b24-111">Permission type</span></span>|<span data-ttu-id="97b24-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97b24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97b24-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97b24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97b24-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97b24-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97b24-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97b24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97b24-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97b24-116">Not supported.</span></span>|
|<span data-ttu-id="97b24-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97b24-117">Application</span></span>|<span data-ttu-id="97b24-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97b24-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97b24-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97b24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="97b24-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97b24-120">Request headers</span></span>
|<span data-ttu-id="97b24-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97b24-121">Header</span></span>|<span data-ttu-id="97b24-122">Значение</span><span class="sxs-lookup"><span data-stu-id="97b24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97b24-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="97b24-123">Authorization</span></span>|<span data-ttu-id="97b24-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="97b24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97b24-125">Accept</span><span class="sxs-lookup"><span data-stu-id="97b24-125">Accept</span></span>|<span data-ttu-id="97b24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97b24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97b24-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97b24-127">Request body</span></span>
<span data-ttu-id="97b24-128">В тексте запроса укажите представление JSON для объекта [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="97b24-128">In the request body, supply a JSON representation for the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="97b24-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="97b24-129">The following table shows the properties that are required when you create the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="97b24-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="97b24-130">Property</span></span>|<span data-ttu-id="97b24-131">Тип</span><span class="sxs-lookup"><span data-stu-id="97b24-131">Type</span></span>|<span data-ttu-id="97b24-132">Описание</span><span class="sxs-lookup"><span data-stu-id="97b24-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97b24-133">id</span><span class="sxs-lookup"><span data-stu-id="97b24-133">id</span></span>|<span data-ttu-id="97b24-134">String</span><span class="sxs-lookup"><span data-stu-id="97b24-134">String</span></span>|<span data-ttu-id="97b24-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="97b24-135">Key of the entity.</span></span> <span data-ttu-id="97b24-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97b24-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97b24-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97b24-137">lastModifiedDateTime</span></span>|<span data-ttu-id="97b24-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97b24-138">DateTimeOffset</span></span>|<span data-ttu-id="97b24-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="97b24-139">DateTime the object was last modified.</span></span> <span data-ttu-id="97b24-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97b24-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97b24-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="97b24-141">roleScopeTagIds</span></span>|<span data-ttu-id="97b24-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="97b24-142">String collection</span></span>|<span data-ttu-id="97b24-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="97b24-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="97b24-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97b24-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97b24-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="97b24-145">supportsScopeTags</span></span>|<span data-ttu-id="97b24-146">Логический</span><span class="sxs-lookup"><span data-stu-id="97b24-146">Boolean</span></span>|<span data-ttu-id="97b24-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="97b24-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="97b24-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="97b24-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="97b24-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="97b24-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="97b24-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97b24-150">This property is read-only.</span></span> <span data-ttu-id="97b24-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97b24-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97b24-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97b24-152">createdDateTime</span></span>|<span data-ttu-id="97b24-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97b24-153">DateTimeOffset</span></span>|<span data-ttu-id="97b24-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="97b24-154">DateTime the object was created.</span></span> <span data-ttu-id="97b24-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97b24-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97b24-156">description</span><span class="sxs-lookup"><span data-stu-id="97b24-156">description</span></span>|<span data-ttu-id="97b24-157">String</span><span class="sxs-lookup"><span data-stu-id="97b24-157">String</span></span>|<span data-ttu-id="97b24-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="97b24-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="97b24-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97b24-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97b24-160">displayName</span><span class="sxs-lookup"><span data-stu-id="97b24-160">displayName</span></span>|<span data-ttu-id="97b24-161">String</span><span class="sxs-lookup"><span data-stu-id="97b24-161">String</span></span>|<span data-ttu-id="97b24-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="97b24-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="97b24-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97b24-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97b24-164">version</span><span class="sxs-lookup"><span data-stu-id="97b24-164">version</span></span>|<span data-ttu-id="97b24-165">Int32</span><span class="sxs-lookup"><span data-stu-id="97b24-165">Int32</span></span>|<span data-ttu-id="97b24-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="97b24-166">Version of the device configuration.</span></span> <span data-ttu-id="97b24-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97b24-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97b24-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="97b24-168">trustedRootCertificate</span></span>|<span data-ttu-id="97b24-169">Binary</span><span class="sxs-lookup"><span data-stu-id="97b24-169">Binary</span></span>|<span data-ttu-id="97b24-170">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="97b24-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="97b24-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="97b24-171">certFileName</span></span>|<span data-ttu-id="97b24-172">String</span><span class="sxs-lookup"><span data-stu-id="97b24-172">String</span></span>|<span data-ttu-id="97b24-173">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="97b24-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="97b24-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="97b24-174">Response</span></span>
<span data-ttu-id="97b24-175">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="97b24-175">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97b24-176">Пример</span><span class="sxs-lookup"><span data-stu-id="97b24-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="97b24-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="97b24-177">Request</span></span>
<span data-ttu-id="97b24-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97b24-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="97b24-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="97b24-179">Response</span></span>
<span data-ttu-id="97b24-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="97b24-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "id": "6316bf01-bf01-6316-01bf-166301bf1663",
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




