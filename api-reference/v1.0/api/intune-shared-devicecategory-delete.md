---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd38e1eb6f732db629a6c88a9a4a36e0357431df
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732809"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="25fcc-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="25fcc-103">Delete deviceCategory</span></span>

<span data-ttu-id="25fcc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25fcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25fcc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25fcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25fcc-106">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="25fcc-106">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25fcc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="25fcc-107">Prerequisites</span></span>
<span data-ttu-id="25fcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25fcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25fcc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25fcc-110">Permission type</span></span>|<span data-ttu-id="25fcc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25fcc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25fcc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25fcc-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="25fcc-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="25fcc-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="25fcc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25fcc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="25fcc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25fcc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25fcc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25fcc-116">Not supported.</span></span>|
|<span data-ttu-id="25fcc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25fcc-117">Application</span></span>|<span data-ttu-id="25fcc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25fcc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25fcc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25fcc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="25fcc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25fcc-120">Request headers</span></span>
|<span data-ttu-id="25fcc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25fcc-121">Header</span></span>|<span data-ttu-id="25fcc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="25fcc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25fcc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="25fcc-123">Authorization</span></span>|<span data-ttu-id="25fcc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25fcc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25fcc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="25fcc-125">Accept</span></span>|<span data-ttu-id="25fcc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25fcc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25fcc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25fcc-127">Request body</span></span>
<span data-ttu-id="25fcc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25fcc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25fcc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="25fcc-129">Response</span></span>
<span data-ttu-id="25fcc-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="25fcc-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="25fcc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="25fcc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="25fcc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="25fcc-132">Request</span></span>
<span data-ttu-id="25fcc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25fcc-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="25fcc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="25fcc-134">Response</span></span>
<span data-ttu-id="25fcc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25fcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









