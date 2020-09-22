---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd38e1eb6f732db629a6c88a9a4a36e0357431df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019197"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="b7a74-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b7a74-103">Delete deviceCategory</span></span>

<span data-ttu-id="b7a74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7a74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7a74-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7a74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7a74-106">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b7a74-106">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7a74-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b7a74-107">Prerequisites</span></span>
<span data-ttu-id="b7a74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7a74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7a74-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7a74-110">Permission type</span></span>|<span data-ttu-id="b7a74-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7a74-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7a74-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7a74-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b7a74-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="b7a74-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b7a74-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7a74-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b7a74-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7a74-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7a74-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7a74-116">Not supported.</span></span>|
|<span data-ttu-id="b7a74-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7a74-117">Application</span></span>|<span data-ttu-id="b7a74-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7a74-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7a74-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7a74-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="b7a74-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b7a74-120">Request headers</span></span>
|<span data-ttu-id="b7a74-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7a74-121">Header</span></span>|<span data-ttu-id="b7a74-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b7a74-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7a74-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7a74-123">Authorization</span></span>|<span data-ttu-id="b7a74-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7a74-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7a74-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b7a74-125">Accept</span></span>|<span data-ttu-id="b7a74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7a74-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7a74-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7a74-127">Request body</span></span>
<span data-ttu-id="b7a74-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7a74-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7a74-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7a74-129">Response</span></span>
<span data-ttu-id="b7a74-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b7a74-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b7a74-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b7a74-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b7a74-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7a74-132">Request</span></span>
<span data-ttu-id="b7a74-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7a74-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="b7a74-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7a74-134">Response</span></span>
<span data-ttu-id="b7a74-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7a74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









