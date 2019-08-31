---
title: Создание Девицеманажементдериведкредентиалсеттингс
description: Создание нового объекта Девицеманажементдериведкредентиалсеттингс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2b948df68c5bf1e9467c66e7a4c326e14dd036f8
ms.sourcegitcommit: 0f3e0bd7b57870a0f7b34cf52eaf4776ac82671e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2019
ms.locfileid: "36699525"
---
# <a name="create-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="05474-103">Создание Девицеманажементдериведкредентиалсеттингс</span><span class="sxs-lookup"><span data-stu-id="05474-103">Create deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="05474-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05474-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05474-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05474-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05474-106">Создание нового объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="05474-106">Create a new [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05474-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="05474-107">Prerequisites</span></span>
<span data-ttu-id="05474-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05474-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05474-110">Permission type</span></span>|<span data-ttu-id="05474-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05474-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05474-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05474-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="05474-113">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="05474-113">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="05474-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05474-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="05474-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05474-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05474-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05474-116">Not supported.</span></span>|
|<span data-ttu-id="05474-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05474-117">Application</span></span>||
|<span data-ttu-id="05474-118">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="05474-118">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="05474-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05474-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05474-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05474-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="05474-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05474-121">Request headers</span></span>
|<span data-ttu-id="05474-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05474-122">Header</span></span>|<span data-ttu-id="05474-123">Значение</span><span class="sxs-lookup"><span data-stu-id="05474-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05474-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05474-124">Authorization</span></span>|<span data-ttu-id="05474-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05474-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05474-126">Accept</span><span class="sxs-lookup"><span data-stu-id="05474-126">Accept</span></span>|<span data-ttu-id="05474-127">application/json</span><span class="sxs-lookup"><span data-stu-id="05474-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05474-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05474-128">Request body</span></span>
<span data-ttu-id="05474-129">В тексте запроса добавьте представление объекта Девицеманажементдериведкредентиалсеттингс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05474-129">In the request body, supply a JSON representation for the deviceManagementDerivedCredentialSettings object.</span></span>

<span data-ttu-id="05474-130">В следующей таблице приведены свойства, необходимые при создании Девицеманажементдериведкредентиалсеттингс.</span><span class="sxs-lookup"><span data-stu-id="05474-130">The following table shows the properties that are required when you create the deviceManagementDerivedCredentialSettings.</span></span>

|<span data-ttu-id="05474-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="05474-131">Property</span></span>|<span data-ttu-id="05474-132">Тип</span><span class="sxs-lookup"><span data-stu-id="05474-132">Type</span></span>|<span data-ttu-id="05474-133">Описание</span><span class="sxs-lookup"><span data-stu-id="05474-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05474-134">id</span><span class="sxs-lookup"><span data-stu-id="05474-134">id</span></span>|<span data-ttu-id="05474-135">String</span><span class="sxs-lookup"><span data-stu-id="05474-135">String</span></span>|<span data-ttu-id="05474-136">Уникальный идентификатор для производных учетных данных</span><span class="sxs-lookup"><span data-stu-id="05474-136">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="05474-137">helpUrl</span><span class="sxs-lookup"><span data-stu-id="05474-137">helpUrl</span></span>|<span data-ttu-id="05474-138">String.</span><span class="sxs-lookup"><span data-stu-id="05474-138">String</span></span>|<span data-ttu-id="05474-139">URL-адрес, который будет доступен конечным пользователям для получения производных учетных данных с помощью корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="05474-139">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="05474-140">displayName</span><span class="sxs-lookup"><span data-stu-id="05474-140">displayName</span></span>|<span data-ttu-id="05474-141">Строка</span><span class="sxs-lookup"><span data-stu-id="05474-141">String</span></span>|<span data-ttu-id="05474-142">Отображаемое имя профиля.</span><span class="sxs-lookup"><span data-stu-id="05474-142">The display name for the profile.</span></span>|
|<span data-ttu-id="05474-143">имени</span><span class="sxs-lookup"><span data-stu-id="05474-143">issuer</span></span>|[<span data-ttu-id="05474-144">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="05474-144">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-shared-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="05474-145">Производный поставщик учетных данных, который будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="05474-145">The derived credential provider to use.</span></span> <span data-ttu-id="05474-146">Возможные значения: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="05474-146">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="05474-147">notificationType</span><span class="sxs-lookup"><span data-stu-id="05474-147">notificationType</span></span>|[<span data-ttu-id="05474-148">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="05474-148">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-shared-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="05474-149">Методы, используемые для информирования конечного пользователя об открытии корпоративного портала для доставки в сеть Wi-Fi, VPN или профилей электронной почты, использующих сертификаты для устройства.</span><span class="sxs-lookup"><span data-stu-id="05474-149">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="05474-150">Возможные значения: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="05474-150">Possible values are: `none`, `companyPortal`, `email`.</span></span>|



## <a name="response"></a><span data-ttu-id="05474-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="05474-151">Response</span></span>
<span data-ttu-id="05474-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05474-152">If successful, this method returns a `201 Created` response code and a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05474-153">Пример</span><span class="sxs-lookup"><span data-stu-id="05474-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="05474-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="05474-154">Request</span></span>
<span data-ttu-id="05474-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05474-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
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

### <a name="response"></a><span data-ttu-id="05474-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="05474-156">Response</span></span>
<span data-ttu-id="05474-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05474-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




