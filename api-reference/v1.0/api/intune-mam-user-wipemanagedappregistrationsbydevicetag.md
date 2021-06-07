---
title: Действие wipeManagedAppRegistrationsByDeviceTag
description: Стирает данные о регистрации приложений с указанным тегом приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b4b1ed19d71e5ccdb593ee7a3f3808945891824d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755544"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="82fe3-103">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="82fe3-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

<span data-ttu-id="82fe3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82fe3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82fe3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82fe3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82fe3-106">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="82fe3-106">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82fe3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="82fe3-107">Prerequisites</span></span>
<span data-ttu-id="82fe3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82fe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82fe3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82fe3-110">Permission type</span></span>|<span data-ttu-id="82fe3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82fe3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82fe3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82fe3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82fe3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82fe3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="82fe3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82fe3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82fe3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82fe3-115">Not supported.</span></span>|
|<span data-ttu-id="82fe3-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="82fe3-116">Application</span></span>|<span data-ttu-id="82fe3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82fe3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82fe3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82fe3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="82fe3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="82fe3-119">Request headers</span></span>
|<span data-ttu-id="82fe3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82fe3-120">Header</span></span>|<span data-ttu-id="82fe3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82fe3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82fe3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82fe3-122">Authorization</span></span>|<span data-ttu-id="82fe3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82fe3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82fe3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82fe3-124">Accept</span></span>|<span data-ttu-id="82fe3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82fe3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82fe3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82fe3-126">Request body</span></span>
<span data-ttu-id="82fe3-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82fe3-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="82fe3-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="82fe3-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="82fe3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="82fe3-129">Property</span></span>|<span data-ttu-id="82fe3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="82fe3-130">Type</span></span>|<span data-ttu-id="82fe3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="82fe3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82fe3-132">deviceTag</span><span class="sxs-lookup"><span data-stu-id="82fe3-132">deviceTag</span></span>|<span data-ttu-id="82fe3-133">String</span><span class="sxs-lookup"><span data-stu-id="82fe3-133">String</span></span>|<span data-ttu-id="82fe3-134">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="82fe3-134">device tag</span></span>|



## <a name="response"></a><span data-ttu-id="82fe3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="82fe3-135">Response</span></span>
<span data-ttu-id="82fe3-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="82fe3-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82fe3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="82fe3-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="82fe3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="82fe3-138">Request</span></span>
<span data-ttu-id="82fe3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82fe3-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="82fe3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="82fe3-140">Response</span></span>
<span data-ttu-id="82fe3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82fe3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




