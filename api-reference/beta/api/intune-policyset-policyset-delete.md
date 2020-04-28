---
title: Удаление политики
description: Удаляет набор политик.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f3d62876f163911c8bcd3ff22f944faebd096f8b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43391720"
---
# <a name="delete-policyset"></a><span data-ttu-id="615bd-103">Удаление политики</span><span class="sxs-lookup"><span data-stu-id="615bd-103">Delete policySet</span></span>

<span data-ttu-id="615bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="615bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="615bd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="615bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="615bd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="615bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="615bd-107">Удаляет набор [политик](../resources/intune-policyset-policyset.md).</span><span class="sxs-lookup"><span data-stu-id="615bd-107">Deletes a [policySet](../resources/intune-policyset-policyset.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="615bd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="615bd-108">Prerequisites</span></span>
<span data-ttu-id="615bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="615bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="615bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="615bd-111">Permission type</span></span>|<span data-ttu-id="615bd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="615bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="615bd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="615bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="615bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="615bd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="615bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="615bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="615bd-116">Not supported.</span></span>|
|<span data-ttu-id="615bd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="615bd-117">Application</span></span>|<span data-ttu-id="615bd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615bd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="615bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="615bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/policySets/{policySetId}
```

## <a name="request-headers"></a><span data-ttu-id="615bd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="615bd-120">Request headers</span></span>
|<span data-ttu-id="615bd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="615bd-121">Header</span></span>|<span data-ttu-id="615bd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="615bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="615bd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="615bd-123">Authorization</span></span>|<span data-ttu-id="615bd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="615bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="615bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="615bd-125">Accept</span></span>|<span data-ttu-id="615bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="615bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="615bd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="615bd-127">Request body</span></span>
<span data-ttu-id="615bd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="615bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="615bd-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="615bd-129">Response</span></span>
<span data-ttu-id="615bd-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="615bd-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="615bd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="615bd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="615bd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="615bd-132">Request</span></span>
<span data-ttu-id="615bd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="615bd-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}
```

### <a name="response"></a><span data-ttu-id="615bd-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="615bd-134">Response</span></span>
<span data-ttu-id="615bd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="615bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



