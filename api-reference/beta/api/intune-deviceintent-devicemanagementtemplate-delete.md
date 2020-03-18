---
title: Удаление Девицеманажементтемплате
description: Удаляет объект Девицеманажементтемплате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c12ac8e12b176bb1fdbd35772bf8ccf85187fdc9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814997"
---
# <a name="delete-devicemanagementtemplate"></a><span data-ttu-id="1fcfc-103">Удаление Девицеманажементтемплате</span><span class="sxs-lookup"><span data-stu-id="1fcfc-103">Delete deviceManagementTemplate</span></span>

> <span data-ttu-id="1fcfc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fcfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fcfc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1fcfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fcfc-106">Удаляет объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="1fcfc-106">Deletes a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fcfc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1fcfc-107">Prerequisites</span></span>
<span data-ttu-id="1fcfc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fcfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fcfc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fcfc-110">Permission type</span></span>|<span data-ttu-id="1fcfc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fcfc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fcfc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fcfc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1fcfc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fcfc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1fcfc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fcfc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fcfc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fcfc-115">Not supported.</span></span>|
|<span data-ttu-id="1fcfc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1fcfc-116">Application</span></span>|<span data-ttu-id="1fcfc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fcfc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fcfc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fcfc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/templates/{deviceManagementTemplateId}
DELETE /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="1fcfc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1fcfc-119">Request headers</span></span>
|<span data-ttu-id="1fcfc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1fcfc-120">Header</span></span>|<span data-ttu-id="1fcfc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1fcfc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fcfc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fcfc-122">Authorization</span></span>|<span data-ttu-id="1fcfc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fcfc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fcfc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1fcfc-124">Accept</span></span>|<span data-ttu-id="1fcfc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1fcfc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fcfc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1fcfc-126">Request body</span></span>
<span data-ttu-id="1fcfc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fcfc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fcfc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fcfc-128">Response</span></span>
<span data-ttu-id="1fcfc-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1fcfc-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1fcfc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1fcfc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fcfc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fcfc-131">Request</span></span>
<span data-ttu-id="1fcfc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fcfc-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
```

### <a name="response"></a><span data-ttu-id="1fcfc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fcfc-133">Response</span></span>
<span data-ttu-id="1fcfc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fcfc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




