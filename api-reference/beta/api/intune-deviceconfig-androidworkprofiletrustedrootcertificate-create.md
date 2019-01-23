---
title: Создание androidWorkProfileTrustedRootCertificate
description: Создание нового объекта androidWorkProfileTrustedRootCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fc819fb720d6620f03abd9cdb011cde8f71a86f5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424478"
---
# <a name="create-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="eca6b-103">Создание androidWorkProfileTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="eca6b-103">Create androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="eca6b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eca6b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eca6b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eca6b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eca6b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eca6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eca6b-107">Создание нового объекта [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="eca6b-107">Create a new [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eca6b-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="eca6b-108">Prerequisites</span></span>
<span data-ttu-id="eca6b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="eca6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eca6b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eca6b-111">Permission type</span></span>|<span data-ttu-id="eca6b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eca6b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eca6b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eca6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eca6b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eca6b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eca6b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eca6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eca6b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eca6b-116">Not supported.</span></span>|
|<span data-ttu-id="eca6b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eca6b-117">Application</span></span>|<span data-ttu-id="eca6b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eca6b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eca6b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eca6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="eca6b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eca6b-120">Request headers</span></span>
|<span data-ttu-id="eca6b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eca6b-121">Header</span></span>|<span data-ttu-id="eca6b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eca6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eca6b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eca6b-123">Authorization</span></span>|<span data-ttu-id="eca6b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="eca6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eca6b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eca6b-125">Accept</span></span>|<span data-ttu-id="eca6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eca6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eca6b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eca6b-127">Request body</span></span>
<span data-ttu-id="eca6b-128">В тексте запроса укажите представление JSON для объекта androidWorkProfileTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="eca6b-128">In the request body, supply a JSON representation for the androidWorkProfileTrustedRootCertificate object.</span></span>

<span data-ttu-id="eca6b-129">В следующей таблице показаны свойства, которые необходимы для создания androidWorkProfileTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="eca6b-129">The following table shows the properties that are required when you create the androidWorkProfileTrustedRootCertificate.</span></span>

|<span data-ttu-id="eca6b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eca6b-130">Property</span></span>|<span data-ttu-id="eca6b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eca6b-131">Type</span></span>|<span data-ttu-id="eca6b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eca6b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eca6b-133">id</span><span class="sxs-lookup"><span data-stu-id="eca6b-133">id</span></span>|<span data-ttu-id="eca6b-134">String</span><span class="sxs-lookup"><span data-stu-id="eca6b-134">String</span></span>|<span data-ttu-id="eca6b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eca6b-135">Key of the entity.</span></span> <span data-ttu-id="eca6b-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eca6b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca6b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eca6b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="eca6b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eca6b-138">DateTimeOffset</span></span>|<span data-ttu-id="eca6b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="eca6b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="eca6b-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eca6b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca6b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eca6b-141">roleScopeTagIds</span></span>|<span data-ttu-id="eca6b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="eca6b-142">String collection</span></span>|<span data-ttu-id="eca6b-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="eca6b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="eca6b-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eca6b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca6b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="eca6b-145">supportsScopeTags</span></span>|<span data-ttu-id="eca6b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="eca6b-146">Boolean</span></span>|<span data-ttu-id="eca6b-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="eca6b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="eca6b-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="eca6b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="eca6b-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="eca6b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="eca6b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eca6b-150">This property is read-only.</span></span> <span data-ttu-id="eca6b-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eca6b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca6b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eca6b-152">createdDateTime</span></span>|<span data-ttu-id="eca6b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eca6b-153">DateTimeOffset</span></span>|<span data-ttu-id="eca6b-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="eca6b-154">DateTime the object was created.</span></span> <span data-ttu-id="eca6b-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eca6b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca6b-156">description</span><span class="sxs-lookup"><span data-stu-id="eca6b-156">description</span></span>|<span data-ttu-id="eca6b-157">String</span><span class="sxs-lookup"><span data-stu-id="eca6b-157">String</span></span>|<span data-ttu-id="eca6b-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eca6b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eca6b-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eca6b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca6b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="eca6b-160">displayName</span></span>|<span data-ttu-id="eca6b-161">String</span><span class="sxs-lookup"><span data-stu-id="eca6b-161">String</span></span>|<span data-ttu-id="eca6b-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eca6b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eca6b-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eca6b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca6b-164">version</span><span class="sxs-lookup"><span data-stu-id="eca6b-164">version</span></span>|<span data-ttu-id="eca6b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="eca6b-165">Int32</span></span>|<span data-ttu-id="eca6b-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eca6b-166">Version of the device configuration.</span></span> <span data-ttu-id="eca6b-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eca6b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca6b-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="eca6b-168">trustedRootCertificate</span></span>|<span data-ttu-id="eca6b-169">Binary</span><span class="sxs-lookup"><span data-stu-id="eca6b-169">Binary</span></span>|<span data-ttu-id="eca6b-170">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="eca6b-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="eca6b-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="eca6b-171">certFileName</span></span>|<span data-ttu-id="eca6b-172">String</span><span class="sxs-lookup"><span data-stu-id="eca6b-172">String</span></span>|<span data-ttu-id="eca6b-173">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="eca6b-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="eca6b-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="eca6b-174">Response</span></span>
<span data-ttu-id="eca6b-175">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="eca6b-175">If successful, this method returns a `201 Created` response code and a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eca6b-176">Пример</span><span class="sxs-lookup"><span data-stu-id="eca6b-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="eca6b-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="eca6b-177">Request</span></span>
<span data-ttu-id="eca6b-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eca6b-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="eca6b-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="eca6b-179">Response</span></span>
<span data-ttu-id="eca6b-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="eca6b-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 550

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "id": "37cc7454-7454-37cc-5474-cc375474cc37",
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




