---
title: Удаление windowsInformationProtectionNetworkLearningSummary
description: Удаление объекта windowsInformationProtectionNetworkLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e0580760d5bc258462a32832493ac053a5acb1fa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457320"
---
# <a name="delete-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="32985-103">Удаление windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="32985-103">Delete windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="32985-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="32985-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32985-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32985-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32985-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32985-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32985-107">Удаление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="32985-107">Deletes a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32985-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="32985-108">Prerequisites</span></span>
<span data-ttu-id="32985-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32985-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32985-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32985-111">Permission type</span></span>|<span data-ttu-id="32985-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32985-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32985-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32985-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32985-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32985-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32985-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32985-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32985-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32985-116">Not supported.</span></span>|
|<span data-ttu-id="32985-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32985-117">Application</span></span>|<span data-ttu-id="32985-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32985-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32985-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32985-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="32985-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="32985-120">Request headers</span></span>
|<span data-ttu-id="32985-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32985-121">Header</span></span>|<span data-ttu-id="32985-122">Значение</span><span class="sxs-lookup"><span data-stu-id="32985-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32985-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32985-123">Authorization</span></span>|<span data-ttu-id="32985-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32985-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32985-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32985-125">Accept</span></span>|<span data-ttu-id="32985-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32985-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32985-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32985-127">Request body</span></span>
<span data-ttu-id="32985-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32985-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32985-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="32985-129">Response</span></span>
<span data-ttu-id="32985-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="32985-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32985-131">Пример</span><span class="sxs-lookup"><span data-stu-id="32985-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="32985-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="32985-132">Request</span></span>
<span data-ttu-id="32985-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32985-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="32985-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="32985-134">Response</span></span>
<span data-ttu-id="32985-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32985-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





