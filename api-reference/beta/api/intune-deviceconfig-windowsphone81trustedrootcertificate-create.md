---
title: Создание windowsPhone81TrustedRootCertificate
description: Создание нового объекта windowsPhone81TrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 230bac046c5df3a5dd476c0324e4b25293d5d418
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931470"
---
# <a name="create-windowsphone81trustedrootcertificate"></a><span data-ttu-id="d52fb-103">Создание windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d52fb-103">Create windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="d52fb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d52fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d52fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d52fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d52fb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d52fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d52fb-107">Создание нового объекта [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="d52fb-107">Create a new [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d52fb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d52fb-108">Prerequisites</span></span>
<span data-ttu-id="d52fb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d52fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d52fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d52fb-111">Permission type</span></span>|<span data-ttu-id="d52fb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d52fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d52fb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d52fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d52fb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d52fb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d52fb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d52fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d52fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d52fb-116">Not supported.</span></span>|
|<span data-ttu-id="d52fb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d52fb-117">Application</span></span>|<span data-ttu-id="d52fb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d52fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d52fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d52fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d52fb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d52fb-120">Request headers</span></span>
|<span data-ttu-id="d52fb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d52fb-121">Header</span></span>|<span data-ttu-id="d52fb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d52fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d52fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d52fb-123">Authorization</span></span>|<span data-ttu-id="d52fb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d52fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d52fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d52fb-125">Accept</span></span>|<span data-ttu-id="d52fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d52fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d52fb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d52fb-127">Request body</span></span>
<span data-ttu-id="d52fb-128">В тексте запроса укажите представление JSON для объекта windowsPhone81TrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="d52fb-128">In the request body, supply a JSON representation for the windowsPhone81TrustedRootCertificate object.</span></span>

<span data-ttu-id="d52fb-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPhone81TrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="d52fb-129">The following table shows the properties that are required when you create the windowsPhone81TrustedRootCertificate.</span></span>

|<span data-ttu-id="d52fb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d52fb-130">Property</span></span>|<span data-ttu-id="d52fb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d52fb-131">Type</span></span>|<span data-ttu-id="d52fb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d52fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d52fb-133">id</span><span class="sxs-lookup"><span data-stu-id="d52fb-133">id</span></span>|<span data-ttu-id="d52fb-134">String</span><span class="sxs-lookup"><span data-stu-id="d52fb-134">String</span></span>|<span data-ttu-id="d52fb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d52fb-135">Key of the entity.</span></span> <span data-ttu-id="d52fb-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d52fb-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d52fb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d52fb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d52fb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d52fb-138">DateTimeOffset</span></span>|<span data-ttu-id="d52fb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d52fb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d52fb-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d52fb-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d52fb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d52fb-141">roleScopeTagIds</span></span>|<span data-ttu-id="d52fb-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d52fb-142">String collection</span></span>|<span data-ttu-id="d52fb-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d52fb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d52fb-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d52fb-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d52fb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d52fb-145">supportsScopeTags</span></span>|<span data-ttu-id="d52fb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d52fb-146">Boolean</span></span>|<span data-ttu-id="d52fb-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="d52fb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d52fb-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="d52fb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d52fb-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d52fb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d52fb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d52fb-150">This property is read-only.</span></span> <span data-ttu-id="d52fb-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d52fb-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d52fb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d52fb-152">createdDateTime</span></span>|<span data-ttu-id="d52fb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d52fb-153">DateTimeOffset</span></span>|<span data-ttu-id="d52fb-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d52fb-154">DateTime the object was created.</span></span> <span data-ttu-id="d52fb-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d52fb-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d52fb-156">описание</span><span class="sxs-lookup"><span data-stu-id="d52fb-156">description</span></span>|<span data-ttu-id="d52fb-157">String</span><span class="sxs-lookup"><span data-stu-id="d52fb-157">String</span></span>|<span data-ttu-id="d52fb-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d52fb-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d52fb-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d52fb-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d52fb-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d52fb-160">displayName</span></span>|<span data-ttu-id="d52fb-161">String</span><span class="sxs-lookup"><span data-stu-id="d52fb-161">String</span></span>|<span data-ttu-id="d52fb-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d52fb-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d52fb-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d52fb-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d52fb-164">version</span><span class="sxs-lookup"><span data-stu-id="d52fb-164">version</span></span>|<span data-ttu-id="d52fb-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d52fb-165">Int32</span></span>|<span data-ttu-id="d52fb-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d52fb-166">Version of the device configuration.</span></span> <span data-ttu-id="d52fb-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d52fb-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d52fb-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d52fb-168">trustedRootCertificate</span></span>|<span data-ttu-id="d52fb-169">Binary</span><span class="sxs-lookup"><span data-stu-id="d52fb-169">Binary</span></span>|<span data-ttu-id="d52fb-170">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="d52fb-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="d52fb-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="d52fb-171">certFileName</span></span>|<span data-ttu-id="d52fb-172">String</span><span class="sxs-lookup"><span data-stu-id="d52fb-172">String</span></span>|<span data-ttu-id="d52fb-173">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="d52fb-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="d52fb-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="d52fb-174">Response</span></span>
<span data-ttu-id="d52fb-175">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d52fb-175">If successful, this method returns a `201 Created` response code and a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d52fb-176">Пример</span><span class="sxs-lookup"><span data-stu-id="d52fb-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="d52fb-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="d52fb-177">Request</span></span>
<span data-ttu-id="d52fb-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d52fb-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 438

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="d52fb-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="d52fb-179">Response</span></span>
<span data-ttu-id="d52fb-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d52fb-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





