---
title: Удаление объекта androidForWorkAppConfigurationSchema
description: Удаляет объект androidForWorkAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9c111d91fd916886422f499ec7bb6a41d14e2aab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144790"
---
# <a name="delete-androidforworkappconfigurationschema"></a><span data-ttu-id="94668-103">Удаление объекта androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="94668-103">Delete androidForWorkAppConfigurationSchema</span></span>

<span data-ttu-id="94668-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94668-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94668-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94668-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94668-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94668-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94668-107">Удаляет объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="94668-107">Deletes a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94668-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="94668-108">Prerequisites</span></span>
<span data-ttu-id="94668-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94668-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94668-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94668-111">Permission type</span></span>|<span data-ttu-id="94668-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94668-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94668-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94668-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94668-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94668-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="94668-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94668-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94668-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94668-116">Not supported.</span></span>|
|<span data-ttu-id="94668-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="94668-117">Application</span></span>|<span data-ttu-id="94668-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94668-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94668-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94668-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="94668-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="94668-120">Request headers</span></span>
|<span data-ttu-id="94668-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94668-121">Header</span></span>|<span data-ttu-id="94668-122">Значение</span><span class="sxs-lookup"><span data-stu-id="94668-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94668-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94668-123">Authorization</span></span>|<span data-ttu-id="94668-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94668-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94668-125">Accept</span><span class="sxs-lookup"><span data-stu-id="94668-125">Accept</span></span>|<span data-ttu-id="94668-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94668-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94668-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94668-127">Request body</span></span>
<span data-ttu-id="94668-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94668-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94668-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="94668-129">Response</span></span>
<span data-ttu-id="94668-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="94668-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="94668-131">Пример</span><span class="sxs-lookup"><span data-stu-id="94668-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="94668-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="94668-132">Request</span></span>
<span data-ttu-id="94668-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94668-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="94668-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="94668-134">Response</span></span>
<span data-ttu-id="94668-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94668-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




