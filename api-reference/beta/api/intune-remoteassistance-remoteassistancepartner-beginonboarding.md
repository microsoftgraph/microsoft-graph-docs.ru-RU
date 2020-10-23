---
title: Действие beginOnboarding
description: Запрос на запуск входящей миграции.  Должен быть связан с соответствующими сведениями учетной записи TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f30689740062995f7867b11c2baf5623d068a504
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698395"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="1292b-104">Действие beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="1292b-104">beginOnboarding action</span></span>

<span data-ttu-id="1292b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1292b-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1292b-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1292b-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1292b-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1292b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1292b-108">Запрос на запуск входящей миграции.</span><span class="sxs-lookup"><span data-stu-id="1292b-108">A request to start onboarding.</span></span>  <span data-ttu-id="1292b-109">Должен быть связан с соответствующими сведениями учетной записи TeamViewer</span><span class="sxs-lookup"><span data-stu-id="1292b-109">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1292b-110">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1292b-110">Prerequisites</span></span>
<span data-ttu-id="1292b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1292b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1292b-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1292b-113">Permission type</span></span>|<span data-ttu-id="1292b-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1292b-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1292b-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1292b-115">Delegated (work or school account)</span></span>|<span data-ttu-id="1292b-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1292b-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1292b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1292b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1292b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1292b-118">Not supported.</span></span>|
|<span data-ttu-id="1292b-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1292b-119">Application</span></span>|<span data-ttu-id="1292b-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1292b-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1292b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1292b-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="1292b-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1292b-122">Request headers</span></span>
|<span data-ttu-id="1292b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1292b-123">Header</span></span>|<span data-ttu-id="1292b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1292b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1292b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1292b-125">Authorization</span></span>|<span data-ttu-id="1292b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1292b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1292b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1292b-127">Accept</span></span>|<span data-ttu-id="1292b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1292b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1292b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1292b-129">Request body</span></span>
<span data-ttu-id="1292b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1292b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1292b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1292b-131">Response</span></span>
<span data-ttu-id="1292b-132">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1292b-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1292b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1292b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1292b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1292b-134">Request</span></span>
<span data-ttu-id="1292b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1292b-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="1292b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1292b-136">Response</span></span>
<span data-ttu-id="1292b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1292b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





