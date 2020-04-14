---
title: Удаление Девицеманажементинтентсеттингкатегори
description: Удаляет объект Девицеманажементинтентсеттингкатегори.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 114b80ff76e0d647752ffef9fc5286c7fd1be4d2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43428074"
---
# <a name="delete-devicemanagementintentsettingcategory"></a><span data-ttu-id="14acb-103">Удаление Девицеманажементинтентсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="14acb-103">Delete deviceManagementIntentSettingCategory</span></span>

<span data-ttu-id="14acb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14acb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14acb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14acb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14acb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14acb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14acb-107">Удаляет объект [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="14acb-107">Deletes a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14acb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="14acb-108">Prerequisites</span></span>
<span data-ttu-id="14acb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14acb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14acb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14acb-111">Permission type</span></span>|<span data-ttu-id="14acb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14acb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14acb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14acb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14acb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14acb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14acb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14acb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14acb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14acb-116">Not supported.</span></span>|
|<span data-ttu-id="14acb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="14acb-117">Application</span></span>|<span data-ttu-id="14acb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14acb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14acb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14acb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="14acb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="14acb-120">Request headers</span></span>
|<span data-ttu-id="14acb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14acb-121">Header</span></span>|<span data-ttu-id="14acb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="14acb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14acb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14acb-123">Authorization</span></span>|<span data-ttu-id="14acb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14acb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14acb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14acb-125">Accept</span></span>|<span data-ttu-id="14acb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14acb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14acb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14acb-127">Request body</span></span>
<span data-ttu-id="14acb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14acb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14acb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="14acb-129">Response</span></span>
<span data-ttu-id="14acb-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="14acb-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="14acb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="14acb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="14acb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="14acb-132">Request</span></span>
<span data-ttu-id="14acb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14acb-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

### <a name="response"></a><span data-ttu-id="14acb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="14acb-134">Response</span></span>
<span data-ttu-id="14acb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14acb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



