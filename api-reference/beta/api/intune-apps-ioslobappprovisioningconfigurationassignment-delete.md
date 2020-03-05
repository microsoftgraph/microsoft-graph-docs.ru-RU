---
title: Удаление Иослобапппровисионингконфигуратионассигнмент
description: Удаляет объект Иослобапппровисионингконфигуратионассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 93b7821a6ff40b2372d7e3e3ad1a81be0762c4db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445822"
---
# <a name="delete-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="da3f2-103">Удаление Иослобапппровисионингконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="da3f2-103">Delete iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="da3f2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="da3f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da3f2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da3f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da3f2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da3f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da3f2-107">Удаляет объект [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="da3f2-107">Deletes a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da3f2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="da3f2-108">Prerequisites</span></span>
<span data-ttu-id="da3f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da3f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da3f2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da3f2-111">Permission type</span></span>|<span data-ttu-id="da3f2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="da3f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da3f2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da3f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da3f2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da3f2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="da3f2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da3f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da3f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da3f2-116">Not supported.</span></span>|
|<span data-ttu-id="da3f2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da3f2-117">Application</span></span>|<span data-ttu-id="da3f2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da3f2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da3f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da3f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="da3f2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="da3f2-120">Request headers</span></span>
|<span data-ttu-id="da3f2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da3f2-121">Header</span></span>|<span data-ttu-id="da3f2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="da3f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da3f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da3f2-123">Authorization</span></span>|<span data-ttu-id="da3f2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da3f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da3f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da3f2-125">Accept</span></span>|<span data-ttu-id="da3f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da3f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da3f2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da3f2-127">Request body</span></span>
<span data-ttu-id="da3f2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da3f2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da3f2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="da3f2-129">Response</span></span>
<span data-ttu-id="da3f2-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="da3f2-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="da3f2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="da3f2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="da3f2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="da3f2-132">Request</span></span>
<span data-ttu-id="da3f2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da3f2-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="da3f2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="da3f2-134">Response</span></span>
<span data-ttu-id="da3f2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da3f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





