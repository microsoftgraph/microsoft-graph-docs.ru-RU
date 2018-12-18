---
title: Создание androidTrustedRootCertificate
description: Создание нового объекта androidTrustedRootCertificate.
author: tfitzmac
ms.openlocfilehash: bd2272b71b562584f880b538d4b2fc412374dda8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354945"
---
# <a name="create-androidtrustedrootcertificate"></a><span data-ttu-id="fecc2-103">Создание androidTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="fecc2-103">Create androidTrustedRootCertificate</span></span>

> <span data-ttu-id="fecc2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fecc2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fecc2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fecc2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fecc2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fecc2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fecc2-107">Создание нового объекта [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="fecc2-107">Create a new [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fecc2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fecc2-108">Prerequisites</span></span>
<span data-ttu-id="fecc2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fecc2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fecc2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fecc2-111">Permission type</span></span>|<span data-ttu-id="fecc2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fecc2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fecc2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fecc2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fecc2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fecc2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fecc2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fecc2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fecc2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fecc2-116">Not supported.</span></span>|
|<span data-ttu-id="fecc2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fecc2-117">Application</span></span>|<span data-ttu-id="fecc2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fecc2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fecc2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fecc2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fecc2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fecc2-120">Request headers</span></span>
|<span data-ttu-id="fecc2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fecc2-121">Header</span></span>|<span data-ttu-id="fecc2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fecc2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fecc2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fecc2-123">Authorization</span></span>|<span data-ttu-id="fecc2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fecc2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fecc2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fecc2-125">Accept</span></span>|<span data-ttu-id="fecc2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fecc2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fecc2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fecc2-127">Request body</span></span>
<span data-ttu-id="fecc2-128">В тексте запроса укажите представление JSON для объекта androidTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="fecc2-128">In the request body, supply a JSON representation for the androidTrustedRootCertificate object.</span></span>

<span data-ttu-id="fecc2-129">В следующей таблице показаны свойства, которые необходимы для создания androidTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="fecc2-129">The following table shows the properties that are required when you create the androidTrustedRootCertificate.</span></span>

|<span data-ttu-id="fecc2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fecc2-130">Property</span></span>|<span data-ttu-id="fecc2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fecc2-131">Type</span></span>|<span data-ttu-id="fecc2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fecc2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fecc2-133">id</span><span class="sxs-lookup"><span data-stu-id="fecc2-133">id</span></span>|<span data-ttu-id="fecc2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fecc2-134">String</span></span>|<span data-ttu-id="fecc2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fecc2-135">Key of the entity.</span></span> <span data-ttu-id="fecc2-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fecc2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fecc2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fecc2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fecc2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fecc2-138">DateTimeOffset</span></span>|<span data-ttu-id="fecc2-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fecc2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fecc2-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fecc2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fecc2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fecc2-141">roleScopeTagIds</span></span>|<span data-ttu-id="fecc2-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fecc2-142">String collection</span></span>|<span data-ttu-id="fecc2-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fecc2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fecc2-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fecc2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fecc2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fecc2-145">supportsScopeTags</span></span>|<span data-ttu-id="fecc2-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="fecc2-146">Boolean</span></span>|<span data-ttu-id="fecc2-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="fecc2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fecc2-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="fecc2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fecc2-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fecc2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fecc2-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fecc2-150">This property is read-only.</span></span> <span data-ttu-id="fecc2-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fecc2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fecc2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fecc2-152">createdDateTime</span></span>|<span data-ttu-id="fecc2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fecc2-153">DateTimeOffset</span></span>|<span data-ttu-id="fecc2-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fecc2-154">DateTime the object was created.</span></span> <span data-ttu-id="fecc2-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fecc2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fecc2-156">описание</span><span class="sxs-lookup"><span data-stu-id="fecc2-156">description</span></span>|<span data-ttu-id="fecc2-157">Строка</span><span class="sxs-lookup"><span data-stu-id="fecc2-157">String</span></span>|<span data-ttu-id="fecc2-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fecc2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fecc2-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fecc2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fecc2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fecc2-160">displayName</span></span>|<span data-ttu-id="fecc2-161">Строка</span><span class="sxs-lookup"><span data-stu-id="fecc2-161">String</span></span>|<span data-ttu-id="fecc2-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fecc2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fecc2-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fecc2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fecc2-164">version</span><span class="sxs-lookup"><span data-stu-id="fecc2-164">version</span></span>|<span data-ttu-id="fecc2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fecc2-165">Int32</span></span>|<span data-ttu-id="fecc2-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fecc2-166">Version of the device configuration.</span></span> <span data-ttu-id="fecc2-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fecc2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fecc2-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="fecc2-168">trustedRootCertificate</span></span>|<span data-ttu-id="fecc2-169">Binary</span><span class="sxs-lookup"><span data-stu-id="fecc2-169">Binary</span></span>|<span data-ttu-id="fecc2-170">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="fecc2-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="fecc2-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="fecc2-171">certFileName</span></span>|<span data-ttu-id="fecc2-172">String.</span><span class="sxs-lookup"><span data-stu-id="fecc2-172">String</span></span>|<span data-ttu-id="fecc2-173">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="fecc2-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="fecc2-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="fecc2-174">Response</span></span>
<span data-ttu-id="fecc2-175">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fecc2-175">If successful, this method returns a `201 Created` response code and a [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fecc2-176">Пример</span><span class="sxs-lookup"><span data-stu-id="fecc2-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="fecc2-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="fecc2-177">Request</span></span>
<span data-ttu-id="fecc2-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fecc2-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 431

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="fecc2-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="fecc2-179">Response</span></span>
<span data-ttu-id="fecc2-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fecc2-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





