---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f9c49ece9485a38a5b9d08cce193f6d6746e711
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086237"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="7b01f-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7b01f-103">Delete deviceCategory</span></span>

> <span data-ttu-id="7b01f-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b01f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7b01f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b01f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b01f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b01f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b01f-107">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="7b01f-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b01f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7b01f-108">Prerequisites</span></span>
<span data-ttu-id="7b01f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b01f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b01f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b01f-111">Permission type</span></span>|<span data-ttu-id="7b01f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b01f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b01f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b01f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7b01f-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7b01f-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7b01f-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b01f-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7b01f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b01f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b01f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b01f-117">Not supported.</span></span>|
|<span data-ttu-id="7b01f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b01f-118">Application</span></span>||
| <span data-ttu-id="7b01f-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7b01f-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7b01f-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b01f-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b01f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b01f-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="7b01f-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7b01f-122">Request headers</span></span>
|<span data-ttu-id="7b01f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b01f-123">Header</span></span>|<span data-ttu-id="7b01f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7b01f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b01f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b01f-125">Authorization</span></span>|<span data-ttu-id="7b01f-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b01f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b01f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7b01f-127">Accept</span></span>|<span data-ttu-id="7b01f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7b01f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b01f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b01f-129">Request body</span></span>
<span data-ttu-id="7b01f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b01f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b01f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b01f-131">Response</span></span>
<span data-ttu-id="7b01f-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7b01f-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7b01f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7b01f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b01f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b01f-134">Request</span></span>

<span data-ttu-id="7b01f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b01f-135">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="7b01f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b01f-136">Response</span></span>

<span data-ttu-id="7b01f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b01f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```












