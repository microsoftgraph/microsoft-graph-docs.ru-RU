---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3fa99ef38b466cff77ba2b374b30b5b1abbba5e2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685025"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="f5ac3-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="f5ac3-103">Delete deviceCategory</span></span>

<span data-ttu-id="f5ac3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5ac3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5ac3-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f5ac3-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f5ac3-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5ac3-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5ac3-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5ac3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5ac3-108">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="f5ac3-108">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5ac3-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f5ac3-109">Prerequisites</span></span>
<span data-ttu-id="f5ac3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5ac3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5ac3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5ac3-112">Permission type</span></span>|<span data-ttu-id="f5ac3-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5ac3-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5ac3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5ac3-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f5ac3-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="f5ac3-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f5ac3-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5ac3-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f5ac3-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5ac3-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5ac3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5ac3-118">Not supported.</span></span>|
|<span data-ttu-id="f5ac3-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5ac3-119">Application</span></span>||
| <span data-ttu-id="f5ac3-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="f5ac3-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f5ac3-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5ac3-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5ac3-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5ac3-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="f5ac3-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f5ac3-123">Request headers</span></span>
|<span data-ttu-id="f5ac3-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5ac3-124">Header</span></span>|<span data-ttu-id="f5ac3-125">Значение</span><span class="sxs-lookup"><span data-stu-id="f5ac3-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5ac3-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5ac3-126">Authorization</span></span>|<span data-ttu-id="f5ac3-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5ac3-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5ac3-128">Accept</span><span class="sxs-lookup"><span data-stu-id="f5ac3-128">Accept</span></span>|<span data-ttu-id="f5ac3-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f5ac3-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5ac3-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f5ac3-130">Request body</span></span>
<span data-ttu-id="f5ac3-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5ac3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5ac3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5ac3-132">Response</span></span>
<span data-ttu-id="f5ac3-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f5ac3-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f5ac3-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f5ac3-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5ac3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5ac3-135">Request</span></span>

<span data-ttu-id="f5ac3-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5ac3-136">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="f5ac3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5ac3-137">Response</span></span>

<span data-ttu-id="f5ac3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5ac3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```











