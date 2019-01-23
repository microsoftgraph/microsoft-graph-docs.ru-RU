---
title: Создание androidTrustedRootCertificate
description: Создание нового объекта androidTrustedRootCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 901d3d94025a4a40c2d57c5c53e3cdb4ac30f0ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401448"
---
# <a name="create-androidtrustedrootcertificate"></a><span data-ttu-id="83917-103">Создание androidTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="83917-103">Create androidTrustedRootCertificate</span></span>

> <span data-ttu-id="83917-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="83917-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83917-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83917-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83917-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83917-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83917-107">Создание нового объекта [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="83917-107">Create a new [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83917-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="83917-108">Prerequisites</span></span>
<span data-ttu-id="83917-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="83917-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="83917-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83917-111">Permission type</span></span>|<span data-ttu-id="83917-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83917-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83917-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83917-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83917-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83917-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83917-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83917-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83917-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83917-116">Not supported.</span></span>|
|<span data-ttu-id="83917-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83917-117">Application</span></span>|<span data-ttu-id="83917-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83917-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83917-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83917-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="83917-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83917-120">Request headers</span></span>
|<span data-ttu-id="83917-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83917-121">Header</span></span>|<span data-ttu-id="83917-122">Значение</span><span class="sxs-lookup"><span data-stu-id="83917-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83917-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83917-123">Authorization</span></span>|<span data-ttu-id="83917-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="83917-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83917-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83917-125">Accept</span></span>|<span data-ttu-id="83917-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83917-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83917-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83917-127">Request body</span></span>
<span data-ttu-id="83917-128">В тексте запроса укажите представление JSON для объекта androidTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="83917-128">In the request body, supply a JSON representation for the androidTrustedRootCertificate object.</span></span>

<span data-ttu-id="83917-129">В следующей таблице показаны свойства, которые необходимы для создания androidTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="83917-129">The following table shows the properties that are required when you create the androidTrustedRootCertificate.</span></span>

|<span data-ttu-id="83917-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="83917-130">Property</span></span>|<span data-ttu-id="83917-131">Тип</span><span class="sxs-lookup"><span data-stu-id="83917-131">Type</span></span>|<span data-ttu-id="83917-132">Описание</span><span class="sxs-lookup"><span data-stu-id="83917-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83917-133">id</span><span class="sxs-lookup"><span data-stu-id="83917-133">id</span></span>|<span data-ttu-id="83917-134">String</span><span class="sxs-lookup"><span data-stu-id="83917-134">String</span></span>|<span data-ttu-id="83917-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="83917-135">Key of the entity.</span></span> <span data-ttu-id="83917-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83917-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83917-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83917-137">lastModifiedDateTime</span></span>|<span data-ttu-id="83917-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83917-138">DateTimeOffset</span></span>|<span data-ttu-id="83917-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="83917-139">DateTime the object was last modified.</span></span> <span data-ttu-id="83917-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83917-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83917-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83917-141">roleScopeTagIds</span></span>|<span data-ttu-id="83917-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="83917-142">String collection</span></span>|<span data-ttu-id="83917-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="83917-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83917-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83917-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83917-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="83917-145">supportsScopeTags</span></span>|<span data-ttu-id="83917-146">Логический</span><span class="sxs-lookup"><span data-stu-id="83917-146">Boolean</span></span>|<span data-ttu-id="83917-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="83917-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="83917-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="83917-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="83917-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="83917-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="83917-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83917-150">This property is read-only.</span></span> <span data-ttu-id="83917-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83917-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83917-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83917-152">createdDateTime</span></span>|<span data-ttu-id="83917-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83917-153">DateTimeOffset</span></span>|<span data-ttu-id="83917-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="83917-154">DateTime the object was created.</span></span> <span data-ttu-id="83917-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83917-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83917-156">description</span><span class="sxs-lookup"><span data-stu-id="83917-156">description</span></span>|<span data-ttu-id="83917-157">String</span><span class="sxs-lookup"><span data-stu-id="83917-157">String</span></span>|<span data-ttu-id="83917-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="83917-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83917-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83917-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83917-160">displayName</span><span class="sxs-lookup"><span data-stu-id="83917-160">displayName</span></span>|<span data-ttu-id="83917-161">String</span><span class="sxs-lookup"><span data-stu-id="83917-161">String</span></span>|<span data-ttu-id="83917-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="83917-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83917-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83917-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83917-164">version</span><span class="sxs-lookup"><span data-stu-id="83917-164">version</span></span>|<span data-ttu-id="83917-165">Int32</span><span class="sxs-lookup"><span data-stu-id="83917-165">Int32</span></span>|<span data-ttu-id="83917-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="83917-166">Version of the device configuration.</span></span> <span data-ttu-id="83917-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83917-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83917-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="83917-168">trustedRootCertificate</span></span>|<span data-ttu-id="83917-169">Binary</span><span class="sxs-lookup"><span data-stu-id="83917-169">Binary</span></span>|<span data-ttu-id="83917-170">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="83917-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="83917-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="83917-171">certFileName</span></span>|<span data-ttu-id="83917-172">String</span><span class="sxs-lookup"><span data-stu-id="83917-172">String</span></span>|<span data-ttu-id="83917-173">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="83917-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="83917-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="83917-174">Response</span></span>
<span data-ttu-id="83917-175">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="83917-175">If successful, this method returns a `201 Created` response code and a [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83917-176">Пример</span><span class="sxs-lookup"><span data-stu-id="83917-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="83917-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="83917-177">Request</span></span>
<span data-ttu-id="83917-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83917-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 367

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="83917-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="83917-179">Response</span></span>
<span data-ttu-id="83917-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="83917-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
  "id": "7f8d751e-751e-7f8d-1e75-8d7f1e758d7f",
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




