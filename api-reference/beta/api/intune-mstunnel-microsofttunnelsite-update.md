---
title: Обновление Микрософттуннелсите
description: Обновление свойств объекта Микрософттуннелсите.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6fa69846aa08faf3be63382a1ec0429936d77370
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301942"
---
# <a name="update-microsofttunnelsite"></a><span data-ttu-id="6e677-103">Обновление Микрософттуннелсите</span><span class="sxs-lookup"><span data-stu-id="6e677-103">Update microsoftTunnelSite</span></span>

<span data-ttu-id="6e677-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e677-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e677-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e677-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e677-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e677-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e677-107">Обновление свойств объекта [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md) .</span><span class="sxs-lookup"><span data-stu-id="6e677-107">Update the properties of a [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e677-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6e677-108">Prerequisites</span></span>
<span data-ttu-id="6e677-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e677-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e677-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e677-111">Permission type</span></span>|<span data-ttu-id="6e677-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e677-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e677-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e677-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e677-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e677-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e677-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e677-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e677-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e677-116">Not supported.</span></span>|
|<span data-ttu-id="6e677-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6e677-117">Application</span></span>|<span data-ttu-id="6e677-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e677-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e677-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e677-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
```

## <a name="request-headers"></a><span data-ttu-id="6e677-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6e677-120">Request headers</span></span>
|<span data-ttu-id="6e677-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e677-121">Header</span></span>|<span data-ttu-id="6e677-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6e677-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e677-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e677-123">Authorization</span></span>|<span data-ttu-id="6e677-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e677-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e677-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e677-125">Accept</span></span>|<span data-ttu-id="6e677-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e677-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e677-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e677-127">Request body</span></span>
<span data-ttu-id="6e677-128">В тексте запроса добавьте представление объекта [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e677-128">In the request body, supply a JSON representation for the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.</span></span>

<span data-ttu-id="6e677-129">В следующей таблице приведены свойства, необходимые при создании [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md).</span><span class="sxs-lookup"><span data-stu-id="6e677-129">The following table shows the properties that are required when you create the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md).</span></span>

|<span data-ttu-id="6e677-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e677-130">Property</span></span>|<span data-ttu-id="6e677-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6e677-131">Type</span></span>|<span data-ttu-id="6e677-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6e677-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e677-133">id</span><span class="sxs-lookup"><span data-stu-id="6e677-133">id</span></span>|<span data-ttu-id="6e677-134">String</span><span class="sxs-lookup"><span data-stu-id="6e677-134">String</span></span>|<span data-ttu-id="6e677-135">Идентификатор Микрософттуннелсите</span><span class="sxs-lookup"><span data-stu-id="6e677-135">The MicrosoftTunnelSite's Id</span></span>|
|<span data-ttu-id="6e677-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6e677-136">displayName</span></span>|<span data-ttu-id="6e677-137">String</span><span class="sxs-lookup"><span data-stu-id="6e677-137">String</span></span>|<span data-ttu-id="6e677-138">Отображаемое имя Микрософттуннелсите</span><span class="sxs-lookup"><span data-stu-id="6e677-138">The MicrosoftTunnelSite's display name</span></span>|
|<span data-ttu-id="6e677-139">description</span><span class="sxs-lookup"><span data-stu-id="6e677-139">description</span></span>|<span data-ttu-id="6e677-140">String</span><span class="sxs-lookup"><span data-stu-id="6e677-140">String</span></span>|<span data-ttu-id="6e677-141">Описание Микрософттуннелсите</span><span class="sxs-lookup"><span data-stu-id="6e677-141">The MicrosoftTunnelSite's description</span></span>|
|<span data-ttu-id="6e677-142">публикаддресс</span><span class="sxs-lookup"><span data-stu-id="6e677-142">publicAddress</span></span>|<span data-ttu-id="6e677-143">String</span><span class="sxs-lookup"><span data-stu-id="6e677-143">String</span></span>|<span data-ttu-id="6e677-144">Имя или IP-адрес общедоступного домена Микрософттуннелсите</span><span class="sxs-lookup"><span data-stu-id="6e677-144">The MicrosoftTunnelSite's public domain name or IP address</span></span>|
|<span data-ttu-id="6e677-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e677-145">roleScopeTagIds</span></span>|<span data-ttu-id="6e677-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6e677-146">String collection</span></span>|<span data-ttu-id="6e677-147">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6e677-147">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="6e677-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e677-148">Response</span></span>
<span data-ttu-id="6e677-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6e677-149">If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e677-150">Пример</span><span class="sxs-lookup"><span data-stu-id="6e677-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e677-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e677-151">Request</span></span>
<span data-ttu-id="6e677-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e677-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="6e677-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e677-153">Response</span></span>
<span data-ttu-id="6e677-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e677-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "b2f7dc3e-dc3e-b2f7-3edc-f7b23edcf7b2",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




