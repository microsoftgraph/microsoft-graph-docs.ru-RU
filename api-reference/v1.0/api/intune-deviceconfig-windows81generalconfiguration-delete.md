---
title: Delete windows81GeneralConfiguration
description: Удаляет объект windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da63317ffad50316d88a3a14da0b6c9ac357ecd5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566061"
---
# <a name="delete-windows81generalconfiguration"></a><span data-ttu-id="bf877-103">Delete windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="bf877-103">Delete windows81GeneralConfiguration</span></span>

> <span data-ttu-id="bf877-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf877-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf877-105">Удаляет объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bf877-105">Deletes a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf877-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bf877-106">Prerequisites</span></span>
<span data-ttu-id="bf877-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf877-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf877-109">Permission type</span></span>|<span data-ttu-id="bf877-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf877-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf877-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf877-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bf877-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf877-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf877-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf877-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf877-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf877-114">Not supported.</span></span>|
|<span data-ttu-id="bf877-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf877-115">Application</span></span>|<span data-ttu-id="bf877-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf877-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf877-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf877-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bf877-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf877-118">Request headers</span></span>
|<span data-ttu-id="bf877-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf877-119">Header</span></span>|<span data-ttu-id="bf877-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bf877-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf877-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf877-121">Authorization</span></span>|<span data-ttu-id="bf877-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf877-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf877-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bf877-123">Accept</span></span>|<span data-ttu-id="bf877-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bf877-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf877-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf877-125">Request body</span></span>
<span data-ttu-id="bf877-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf877-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf877-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf877-127">Response</span></span>
<span data-ttu-id="bf877-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bf877-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bf877-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bf877-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf877-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf877-130">Request</span></span>
<span data-ttu-id="bf877-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf877-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bf877-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf877-132">Response</span></span>
<span data-ttu-id="bf877-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf877-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



