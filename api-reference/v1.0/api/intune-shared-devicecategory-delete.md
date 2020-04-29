---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 177698ab5034a615a81332b6a734340a6b954c22
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461242"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="90745-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="90745-103">Delete deviceCategory</span></span>

<span data-ttu-id="90745-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90745-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90745-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90745-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90745-106">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="90745-106">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90745-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="90745-107">Prerequisites</span></span>
<span data-ttu-id="90745-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90745-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90745-110">Permission type</span></span>|<span data-ttu-id="90745-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90745-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90745-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90745-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="90745-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="90745-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="90745-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90745-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="90745-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90745-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90745-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90745-116">Not supported.</span></span>|
|<span data-ttu-id="90745-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90745-117">Application</span></span>|<span data-ttu-id="90745-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90745-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90745-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90745-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="90745-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90745-120">Request headers</span></span>
|<span data-ttu-id="90745-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90745-121">Header</span></span>|<span data-ttu-id="90745-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90745-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90745-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90745-123">Authorization</span></span>|<span data-ttu-id="90745-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90745-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90745-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90745-125">Accept</span></span>|<span data-ttu-id="90745-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90745-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90745-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90745-127">Request body</span></span>
<span data-ttu-id="90745-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90745-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90745-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="90745-129">Response</span></span>
<span data-ttu-id="90745-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="90745-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="90745-131">Пример</span><span class="sxs-lookup"><span data-stu-id="90745-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="90745-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90745-132">Request</span></span>
<span data-ttu-id="90745-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90745-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="90745-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="90745-134">Response</span></span>
<span data-ttu-id="90745-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90745-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






