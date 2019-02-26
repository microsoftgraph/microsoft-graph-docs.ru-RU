---
title: Действие requestRemoteAssistance
description: Запрос удаленной помощи
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4abb85e26fa8897f42db1948139b1b27f461228
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255579"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="b6619-103">Действие requestRemoteAssistance</span><span class="sxs-lookup"><span data-stu-id="b6619-103">requestRemoteAssistance action</span></span>

> <span data-ttu-id="b6619-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6619-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6619-105">Запрос удаленной помощи</span><span class="sxs-lookup"><span data-stu-id="b6619-105">Request remote assistance</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6619-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b6619-106">Prerequisites</span></span>
<span data-ttu-id="b6619-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b6619-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b6619-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6619-109">Permission type</span></span>|<span data-ttu-id="b6619-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6619-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6619-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6619-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6619-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6619-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b6619-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6619-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6619-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6619-114">Not supported.</span></span>|
|<span data-ttu-id="b6619-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6619-115">Application</span></span>|<span data-ttu-id="b6619-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6619-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6619-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6619-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

## <a name="request-headers"></a><span data-ttu-id="b6619-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6619-118">Request headers</span></span>
|<span data-ttu-id="b6619-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6619-119">Header</span></span>|<span data-ttu-id="b6619-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b6619-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6619-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6619-121">Authorization</span></span>|<span data-ttu-id="b6619-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b6619-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6619-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b6619-123">Accept</span></span>|<span data-ttu-id="b6619-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b6619-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6619-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6619-125">Request body</span></span>
<span data-ttu-id="b6619-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6619-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6619-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6619-127">Response</span></span>
<span data-ttu-id="b6619-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6619-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b6619-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b6619-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6619-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6619-130">Request</span></span>
<span data-ttu-id="b6619-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6619-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="b6619-132">Отклик
</span><span class="sxs-lookup"><span data-stu-id="b6619-132">Response</span></span>
<span data-ttu-id="b6619-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b6619-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



