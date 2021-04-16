---
title: Создание microsoftTunnelSite
description: Создайте новый объект microsoftTunnelSite.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b37330f63c9c0f27ae0d701db59b5795d3f15bf4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864811"
---
# <a name="create-microsofttunnelsite"></a><span data-ttu-id="ea5d7-103">Создание microsoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="ea5d7-103">Create microsoftTunnelSite</span></span>

<span data-ttu-id="ea5d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea5d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea5d7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea5d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea5d7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea5d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea5d7-107">Создайте новый [объект microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)</span><span class="sxs-lookup"><span data-stu-id="ea5d7-107">Create a new [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea5d7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea5d7-108">Prerequisites</span></span>
<span data-ttu-id="ea5d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea5d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea5d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea5d7-111">Permission type</span></span>|<span data-ttu-id="ea5d7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea5d7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea5d7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea5d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea5d7-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5d7-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="ea5d7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea5d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea5d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea5d7-116">Not supported.</span></span>|
|<span data-ttu-id="ea5d7-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ea5d7-117">Application</span></span>|<span data-ttu-id="ea5d7-118">MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5d7-118">MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea5d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea5d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites
```

## <a name="request-headers"></a><span data-ttu-id="ea5d7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ea5d7-120">Request headers</span></span>
|<span data-ttu-id="ea5d7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea5d7-121">Header</span></span>|<span data-ttu-id="ea5d7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ea5d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea5d7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea5d7-123">Authorization</span></span>|<span data-ttu-id="ea5d7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea5d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea5d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea5d7-125">Accept</span></span>|<span data-ttu-id="ea5d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea5d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea5d7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea5d7-127">Request body</span></span>
<span data-ttu-id="ea5d7-128">В теле запроса устройте представление JSON для объекта microsoftTunnelSite.</span><span class="sxs-lookup"><span data-stu-id="ea5d7-128">In the request body, supply a JSON representation for the microsoftTunnelSite object.</span></span>

<span data-ttu-id="ea5d7-129">В следующей таблице показаны свойства, необходимые при создании microsoftTunnelSite.</span><span class="sxs-lookup"><span data-stu-id="ea5d7-129">The following table shows the properties that are required when you create the microsoftTunnelSite.</span></span>

|<span data-ttu-id="ea5d7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea5d7-130">Property</span></span>|<span data-ttu-id="ea5d7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ea5d7-131">Type</span></span>|<span data-ttu-id="ea5d7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ea5d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea5d7-133">id</span><span class="sxs-lookup"><span data-stu-id="ea5d7-133">id</span></span>|<span data-ttu-id="ea5d7-134">String</span><span class="sxs-lookup"><span data-stu-id="ea5d7-134">String</span></span>|<span data-ttu-id="ea5d7-135">Id MicrosoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="ea5d7-135">The MicrosoftTunnelSite's Id</span></span>|
|<span data-ttu-id="ea5d7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ea5d7-136">displayName</span></span>|<span data-ttu-id="ea5d7-137">String</span><span class="sxs-lookup"><span data-stu-id="ea5d7-137">String</span></span>|<span data-ttu-id="ea5d7-138">Имя отображения MicrosoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="ea5d7-138">The MicrosoftTunnelSite's display name</span></span>|
|<span data-ttu-id="ea5d7-139">description</span><span class="sxs-lookup"><span data-stu-id="ea5d7-139">description</span></span>|<span data-ttu-id="ea5d7-140">String</span><span class="sxs-lookup"><span data-stu-id="ea5d7-140">String</span></span>|<span data-ttu-id="ea5d7-141">Описание MicrosoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="ea5d7-141">The MicrosoftTunnelSite's description</span></span>|
|<span data-ttu-id="ea5d7-142">publicAddress</span><span class="sxs-lookup"><span data-stu-id="ea5d7-142">publicAddress</span></span>|<span data-ttu-id="ea5d7-143">String</span><span class="sxs-lookup"><span data-stu-id="ea5d7-143">String</span></span>|<span data-ttu-id="ea5d7-144">Имя или IP-адрес общественного домена MicrosoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="ea5d7-144">The MicrosoftTunnelSite's public domain name or IP address</span></span>|
|<span data-ttu-id="ea5d7-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ea5d7-145">roleScopeTagIds</span></span>|<span data-ttu-id="ea5d7-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea5d7-146">String collection</span></span>|<span data-ttu-id="ea5d7-147">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="ea5d7-147">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="ea5d7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea5d7-148">Response</span></span>
<span data-ttu-id="ea5d7-149">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ea5d7-149">If successful, this method returns a `201 Created` response code and a [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea5d7-150">Пример</span><span class="sxs-lookup"><span data-stu-id="ea5d7-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea5d7-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea5d7-151">Request</span></span>
<span data-ttu-id="ea5d7-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea5d7-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites
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

### <a name="response"></a><span data-ttu-id="ea5d7-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea5d7-153">Response</span></span>
<span data-ttu-id="ea5d7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea5d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




