---
title: Действие beginOnboarding
description: Запрос на запуск входящей миграции.  Должен быть связан с соответствующими сведениями учетной записи TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 011705a50c5dbeec1559bbc803f03991cd03292d
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178145"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="1dd97-104">Действие beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="1dd97-104">beginOnboarding action</span></span>

<span data-ttu-id="1dd97-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dd97-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dd97-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dd97-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dd97-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1dd97-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dd97-108">Запрос на запуск входящей миграции.</span><span class="sxs-lookup"><span data-stu-id="1dd97-108">A request to start onboarding.</span></span>  <span data-ttu-id="1dd97-109">Должен быть связан с соответствующими сведениями учетной записи TeamViewer</span><span class="sxs-lookup"><span data-stu-id="1dd97-109">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dd97-110">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1dd97-110">Prerequisites</span></span>
<span data-ttu-id="1dd97-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dd97-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dd97-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dd97-113">Permission type</span></span>|<span data-ttu-id="1dd97-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dd97-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dd97-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dd97-115">Delegated (work or school account)</span></span>|<span data-ttu-id="1dd97-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd97-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1dd97-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dd97-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dd97-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dd97-118">Not supported.</span></span>|
|<span data-ttu-id="1dd97-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dd97-119">Application</span></span>|<span data-ttu-id="1dd97-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd97-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dd97-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dd97-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="1dd97-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1dd97-122">Request headers</span></span>
|<span data-ttu-id="1dd97-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1dd97-123">Header</span></span>|<span data-ttu-id="1dd97-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1dd97-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dd97-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dd97-125">Authorization</span></span>|<span data-ttu-id="1dd97-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dd97-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dd97-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1dd97-127">Accept</span></span>|<span data-ttu-id="1dd97-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1dd97-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dd97-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1dd97-129">Request body</span></span>
<span data-ttu-id="1dd97-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1dd97-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dd97-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1dd97-131">Response</span></span>
<span data-ttu-id="1dd97-132">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1dd97-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1dd97-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1dd97-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dd97-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dd97-134">Request</span></span>
<span data-ttu-id="1dd97-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dd97-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="1dd97-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dd97-136">Response</span></span>
<span data-ttu-id="1dd97-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1dd97-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



