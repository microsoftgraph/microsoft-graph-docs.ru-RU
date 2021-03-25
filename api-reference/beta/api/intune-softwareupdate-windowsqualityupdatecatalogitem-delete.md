---
title: Удаление windowsQualityUpdateCatalogItem
description: Удаляет windowsQualityUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 87f05706fe06c5601c39d2ba4c5366146488c0d0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156312"
---
# <a name="delete-windowsqualityupdatecatalogitem"></a><span data-ttu-id="d3265-103">Удаление windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="d3265-103">Delete windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="d3265-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3265-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3265-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3265-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3265-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3265-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3265-107">Удаляет [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).</span><span class="sxs-lookup"><span data-stu-id="d3265-107">Deletes a [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3265-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d3265-108">Prerequisites</span></span>
<span data-ttu-id="d3265-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3265-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3265-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3265-111">Permission type</span></span>|<span data-ttu-id="d3265-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3265-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3265-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3265-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3265-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3265-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3265-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3265-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3265-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3265-116">Not supported.</span></span>|
|<span data-ttu-id="d3265-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d3265-117">Application</span></span>|<span data-ttu-id="d3265-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3265-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3265-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3265-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="request-headers"></a><span data-ttu-id="d3265-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d3265-120">Request headers</span></span>
|<span data-ttu-id="d3265-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3265-121">Header</span></span>|<span data-ttu-id="d3265-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d3265-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3265-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3265-123">Authorization</span></span>|<span data-ttu-id="d3265-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3265-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3265-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3265-125">Accept</span></span>|<span data-ttu-id="d3265-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3265-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3265-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3265-127">Request body</span></span>
<span data-ttu-id="d3265-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3265-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3265-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3265-129">Response</span></span>
<span data-ttu-id="d3265-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d3265-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d3265-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d3265-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3265-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3265-132">Request</span></span>
<span data-ttu-id="d3265-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3265-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

### <a name="response"></a><span data-ttu-id="d3265-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3265-134">Response</span></span>
<span data-ttu-id="d3265-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3265-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




