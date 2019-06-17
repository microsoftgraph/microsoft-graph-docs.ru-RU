---
title: Обновление Девицеманажементдериведкредентиалсеттингс
description: Обновление свойств объекта Девицеманажементдериведкредентиалсеттингс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0081b43b466439169799d46e0cfcacc341820a3d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967526"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="cc345-103">Обновление Девицеманажементдериведкредентиалсеттингс</span><span class="sxs-lookup"><span data-stu-id="cc345-103">Update deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="cc345-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc345-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc345-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc345-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc345-106">Обновление свойств объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="cc345-106">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc345-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cc345-107">Prerequisites</span></span>
<span data-ttu-id="cc345-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc345-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc345-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc345-110">Permission type</span></span>|<span data-ttu-id="cc345-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc345-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc345-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc345-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc345-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc345-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc345-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc345-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc345-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc345-115">Not supported.</span></span>|
|<span data-ttu-id="cc345-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc345-116">Application</span></span>|<span data-ttu-id="cc345-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc345-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc345-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc345-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a><span data-ttu-id="cc345-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc345-119">Request headers</span></span>
|<span data-ttu-id="cc345-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc345-120">Header</span></span>|<span data-ttu-id="cc345-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cc345-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc345-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc345-122">Authorization</span></span>|<span data-ttu-id="cc345-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc345-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc345-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cc345-124">Accept</span></span>|<span data-ttu-id="cc345-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc345-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc345-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cc345-126">Request body</span></span>
<span data-ttu-id="cc345-127">В тексте запроса добавьте представление объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc345-127">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="cc345-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="cc345-128">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="cc345-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc345-129">Property</span></span>|<span data-ttu-id="cc345-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cc345-130">Type</span></span>|<span data-ttu-id="cc345-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cc345-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc345-132">id</span><span class="sxs-lookup"><span data-stu-id="cc345-132">id</span></span>|<span data-ttu-id="cc345-133">String</span><span class="sxs-lookup"><span data-stu-id="cc345-133">String</span></span>|<span data-ttu-id="cc345-134">Уникальный идентификатор для производных учетных данных</span><span class="sxs-lookup"><span data-stu-id="cc345-134">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="cc345-135">helpUrl</span><span class="sxs-lookup"><span data-stu-id="cc345-135">helpUrl</span></span>|<span data-ttu-id="cc345-136">String</span><span class="sxs-lookup"><span data-stu-id="cc345-136">String</span></span>|<span data-ttu-id="cc345-137">URL-адрес, который будет доступен конечным пользователям для получения производных учетных данных с помощью корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="cc345-137">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="cc345-138">displayName</span><span class="sxs-lookup"><span data-stu-id="cc345-138">displayName</span></span>|<span data-ttu-id="cc345-139">Строка</span><span class="sxs-lookup"><span data-stu-id="cc345-139">String</span></span>|<span data-ttu-id="cc345-140">Отображаемое имя профиля.</span><span class="sxs-lookup"><span data-stu-id="cc345-140">The display name for the profile.</span></span>|
|<span data-ttu-id="cc345-141">имени</span><span class="sxs-lookup"><span data-stu-id="cc345-141">issuer</span></span>|[<span data-ttu-id="cc345-142">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="cc345-142">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="cc345-143">Производный поставщик учетных данных, который будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="cc345-143">The derived credential provider to use.</span></span> <span data-ttu-id="cc345-144">Возможные значения: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="cc345-144">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="cc345-145">notificationType</span><span class="sxs-lookup"><span data-stu-id="cc345-145">notificationType</span></span>|[<span data-ttu-id="cc345-146">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="cc345-146">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="cc345-147">Методы, используемые для информирования конечного пользователя об открытии корпоративного портала для доставки в сеть Wi-Fi, VPN или профилей электронной почты, использующих сертификаты для устройства.</span><span class="sxs-lookup"><span data-stu-id="cc345-147">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="cc345-148">Возможные значения: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="cc345-148">Possible values are: `none`, `companyPortal`, `email`.</span></span>|



## <a name="response"></a><span data-ttu-id="cc345-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc345-149">Response</span></span>
<span data-ttu-id="cc345-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc345-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc345-151">Пример</span><span class="sxs-lookup"><span data-stu-id="cc345-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc345-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc345-152">Request</span></span>
<span data-ttu-id="cc345-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc345-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 241

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "entrustDatacard",
  "notificationType": "companyPortal"
}
```

### <a name="response"></a><span data-ttu-id="cc345-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc345-154">Response</span></span>
<span data-ttu-id="cc345-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc345-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "entrustDatacard",
  "notificationType": "companyPortal"
}
```





