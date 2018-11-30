---
title: Создание androidForWorkTrustedRootCertificate
description: Создание нового объекта androidForWorkTrustedRootCertificate.
ms.openlocfilehash: 9fe6ca816e8450d4bc946f62f80d3927c2636221
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080953"
---
# <a name="create-androidforworktrustedrootcertificate"></a><span data-ttu-id="f347a-103">Создание androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f347a-103">Create androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="f347a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f347a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f347a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f347a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f347a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f347a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f347a-107">Создание нового объекта [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="f347a-107">Create a new [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f347a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f347a-108">Prerequisites</span></span>
<span data-ttu-id="f347a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f347a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f347a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f347a-111">Permission type</span></span>|<span data-ttu-id="f347a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f347a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f347a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f347a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f347a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f347a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f347a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f347a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f347a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f347a-116">Not supported.</span></span>|
|<span data-ttu-id="f347a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f347a-117">Application</span></span>|<span data-ttu-id="f347a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f347a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f347a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f347a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f347a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f347a-120">Request headers</span></span>
|<span data-ttu-id="f347a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f347a-121">Header</span></span>|<span data-ttu-id="f347a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f347a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f347a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f347a-123">Authorization</span></span>|<span data-ttu-id="f347a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f347a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f347a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f347a-125">Accept</span></span>|<span data-ttu-id="f347a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f347a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f347a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f347a-127">Request body</span></span>
<span data-ttu-id="f347a-128">В тексте запроса укажите представление JSON для объекта androidForWorkTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="f347a-128">In the request body, supply a JSON representation for the androidForWorkTrustedRootCertificate object.</span></span>

<span data-ttu-id="f347a-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="f347a-129">The following table shows the properties that are required when you create the androidForWorkTrustedRootCertificate.</span></span>

|<span data-ttu-id="f347a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f347a-130">Property</span></span>|<span data-ttu-id="f347a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f347a-131">Type</span></span>|<span data-ttu-id="f347a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f347a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f347a-133">id</span><span class="sxs-lookup"><span data-stu-id="f347a-133">id</span></span>|<span data-ttu-id="f347a-134">String</span><span class="sxs-lookup"><span data-stu-id="f347a-134">String</span></span>|<span data-ttu-id="f347a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f347a-135">Key of the entity.</span></span> <span data-ttu-id="f347a-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f347a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f347a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f347a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f347a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f347a-138">DateTimeOffset</span></span>|<span data-ttu-id="f347a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f347a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f347a-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f347a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f347a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f347a-141">roleScopeTagIds</span></span>|<span data-ttu-id="f347a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f347a-142">String collection</span></span>|<span data-ttu-id="f347a-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f347a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f347a-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f347a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f347a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f347a-145">supportsScopeTags</span></span>|<span data-ttu-id="f347a-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f347a-146">Boolean</span></span>|<span data-ttu-id="f347a-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="f347a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f347a-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="f347a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f347a-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f347a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f347a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f347a-150">This property is read-only.</span></span> <span data-ttu-id="f347a-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f347a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f347a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f347a-152">createdDateTime</span></span>|<span data-ttu-id="f347a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f347a-153">DateTimeOffset</span></span>|<span data-ttu-id="f347a-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f347a-154">DateTime the object was created.</span></span> <span data-ttu-id="f347a-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f347a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f347a-156">описание</span><span class="sxs-lookup"><span data-stu-id="f347a-156">description</span></span>|<span data-ttu-id="f347a-157">String</span><span class="sxs-lookup"><span data-stu-id="f347a-157">String</span></span>|<span data-ttu-id="f347a-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f347a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f347a-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f347a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f347a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f347a-160">displayName</span></span>|<span data-ttu-id="f347a-161">String</span><span class="sxs-lookup"><span data-stu-id="f347a-161">String</span></span>|<span data-ttu-id="f347a-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f347a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f347a-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f347a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f347a-164">version</span><span class="sxs-lookup"><span data-stu-id="f347a-164">version</span></span>|<span data-ttu-id="f347a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f347a-165">Int32</span></span>|<span data-ttu-id="f347a-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f347a-166">Version of the device configuration.</span></span> <span data-ttu-id="f347a-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f347a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f347a-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f347a-168">trustedRootCertificate</span></span>|<span data-ttu-id="f347a-169">Двоичный</span><span class="sxs-lookup"><span data-stu-id="f347a-169">Binary</span></span>|<span data-ttu-id="f347a-170">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="f347a-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="f347a-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="f347a-171">certFileName</span></span>|<span data-ttu-id="f347a-172">String</span><span class="sxs-lookup"><span data-stu-id="f347a-172">String</span></span>|<span data-ttu-id="f347a-173">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="f347a-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="f347a-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="f347a-174">Response</span></span>
<span data-ttu-id="f347a-175">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f347a-175">If successful, this method returns a `201 Created` response code and a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f347a-176">Пример</span><span class="sxs-lookup"><span data-stu-id="f347a-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="f347a-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="f347a-177">Request</span></span>
<span data-ttu-id="f347a-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f347a-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 438

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="f347a-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="f347a-179">Response</span></span>
<span data-ttu-id="f347a-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f347a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
  "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
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





