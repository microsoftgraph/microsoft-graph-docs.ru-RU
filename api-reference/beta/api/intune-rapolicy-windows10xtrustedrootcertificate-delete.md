---
title: Удаление windows10XTrustedRootCertificate
description: Удаляет windows10XTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 87d9baa18891f43c3d86f5ec8f5a07966c71debd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145119"
---
# <a name="delete-windows10xtrustedrootcertificate"></a><span data-ttu-id="50bfc-103">Удаление windows10XTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="50bfc-103">Delete windows10XTrustedRootCertificate</span></span>

<span data-ttu-id="50bfc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50bfc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50bfc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50bfc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50bfc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50bfc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50bfc-107">Удаляет [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="50bfc-107">Deletes a [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50bfc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="50bfc-108">Prerequisites</span></span>
<span data-ttu-id="50bfc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50bfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50bfc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50bfc-111">Permission type</span></span>|<span data-ttu-id="50bfc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50bfc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50bfc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50bfc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50bfc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50bfc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="50bfc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50bfc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50bfc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50bfc-116">Not supported.</span></span>|
|<span data-ttu-id="50bfc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="50bfc-117">Application</span></span>|<span data-ttu-id="50bfc-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50bfc-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50bfc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50bfc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="request-headers"></a><span data-ttu-id="50bfc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50bfc-120">Request headers</span></span>
|<span data-ttu-id="50bfc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50bfc-121">Header</span></span>|<span data-ttu-id="50bfc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50bfc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50bfc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50bfc-123">Authorization</span></span>|<span data-ttu-id="50bfc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50bfc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50bfc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50bfc-125">Accept</span></span>|<span data-ttu-id="50bfc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50bfc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50bfc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50bfc-127">Request body</span></span>
<span data-ttu-id="50bfc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50bfc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50bfc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="50bfc-129">Response</span></span>
<span data-ttu-id="50bfc-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="50bfc-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50bfc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="50bfc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="50bfc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="50bfc-132">Request</span></span>
<span data-ttu-id="50bfc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50bfc-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

### <a name="response"></a><span data-ttu-id="50bfc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="50bfc-134">Response</span></span>
<span data-ttu-id="50bfc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50bfc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




