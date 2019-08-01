---
title: Delete windows10CustomConfiguration
description: Удаляет объект windows10CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6e087bc166d2c006d6b67c1c0c78da02073cade7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997346"
---
# <a name="delete-windows10customconfiguration"></a><span data-ttu-id="c8858-103">Delete windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8858-103">Delete windows10CustomConfiguration</span></span>

> <span data-ttu-id="c8858-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8858-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8858-105">Удаляет объект [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8858-105">Deletes a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8858-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c8858-106">Prerequisites</span></span>
<span data-ttu-id="c8858-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8858-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8858-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8858-109">Permission type</span></span>|<span data-ttu-id="c8858-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8858-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8858-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8858-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8858-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8858-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8858-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8858-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8858-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8858-114">Not supported.</span></span>|
|<span data-ttu-id="c8858-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8858-115">Application</span></span>|<span data-ttu-id="c8858-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8858-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8858-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8858-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c8858-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8858-118">Request headers</span></span>
|<span data-ttu-id="c8858-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8858-119">Header</span></span>|<span data-ttu-id="c8858-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c8858-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8858-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8858-121">Authorization</span></span>|<span data-ttu-id="c8858-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8858-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8858-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c8858-123">Accept</span></span>|<span data-ttu-id="c8858-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c8858-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8858-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c8858-125">Request body</span></span>
<span data-ttu-id="c8858-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8858-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8858-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8858-127">Response</span></span>
<span data-ttu-id="c8858-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c8858-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8858-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c8858-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8858-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8858-130">Request</span></span>
<span data-ttu-id="c8858-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8858-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c8858-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8858-132">Response</span></span>
<span data-ttu-id="c8858-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8858-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



