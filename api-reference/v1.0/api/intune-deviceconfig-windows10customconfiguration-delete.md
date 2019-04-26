---
title: Delete windows10CustomConfiguration
description: Удаляет объект windows10CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e4bd49582ee3f7e3e2eaa3885013a3953d9fd775
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558162"
---
# <a name="delete-windows10customconfiguration"></a><span data-ttu-id="2ccce-103">Delete windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ccce-103">Delete windows10CustomConfiguration</span></span>

> <span data-ttu-id="2ccce-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ccce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ccce-105">Удаляет объект [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ccce-105">Deletes a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ccce-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2ccce-106">Prerequisites</span></span>
<span data-ttu-id="2ccce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ccce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ccce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ccce-109">Permission type</span></span>|<span data-ttu-id="2ccce-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ccce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ccce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ccce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2ccce-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ccce-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ccce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ccce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ccce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ccce-114">Not supported.</span></span>|
|<span data-ttu-id="2ccce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ccce-115">Application</span></span>|<span data-ttu-id="2ccce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ccce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ccce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ccce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2ccce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ccce-118">Request headers</span></span>
|<span data-ttu-id="2ccce-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ccce-119">Header</span></span>|<span data-ttu-id="2ccce-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2ccce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ccce-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ccce-121">Authorization</span></span>|<span data-ttu-id="2ccce-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ccce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ccce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2ccce-123">Accept</span></span>|<span data-ttu-id="2ccce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2ccce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ccce-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ccce-125">Request body</span></span>
<span data-ttu-id="2ccce-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ccce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ccce-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ccce-127">Response</span></span>
<span data-ttu-id="2ccce-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2ccce-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2ccce-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2ccce-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ccce-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ccce-130">Request</span></span>
<span data-ttu-id="2ccce-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ccce-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2ccce-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ccce-132">Response</span></span>
<span data-ttu-id="2ccce-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ccce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



