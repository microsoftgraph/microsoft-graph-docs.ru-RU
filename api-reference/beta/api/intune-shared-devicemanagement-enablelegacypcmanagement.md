---
title: Действие enableLegacyPcManagement
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b0aad3505dfc0b4a0b22f6af820e269c4aac7b3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210391"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="f1415-103">Действие enableLegacyPcManagement</span><span class="sxs-lookup"><span data-stu-id="f1415-103">enableLegacyPcManagement action</span></span>

<span data-ttu-id="f1415-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1415-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1415-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f1415-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f1415-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1415-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1415-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1415-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1415-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f1415-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1415-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f1415-109">Prerequisites</span></span>
<span data-ttu-id="f1415-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1415-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1415-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1415-112">Permission type</span></span>|<span data-ttu-id="f1415-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1415-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1415-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1415-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f1415-115">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="f1415-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f1415-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1415-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1415-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1415-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1415-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1415-118">Not supported.</span></span>|
|<span data-ttu-id="f1415-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="f1415-119">Application</span></span>||
| <span data-ttu-id="f1415-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="f1415-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f1415-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1415-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1415-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1415-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="f1415-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f1415-123">Request headers</span></span>
|<span data-ttu-id="f1415-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1415-124">Header</span></span>|<span data-ttu-id="f1415-125">Значение</span><span class="sxs-lookup"><span data-stu-id="f1415-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1415-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1415-126">Authorization</span></span>|<span data-ttu-id="f1415-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1415-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1415-128">Accept</span><span class="sxs-lookup"><span data-stu-id="f1415-128">Accept</span></span>|<span data-ttu-id="f1415-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f1415-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1415-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1415-130">Request body</span></span>
<span data-ttu-id="f1415-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1415-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1415-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1415-132">Response</span></span>
<span data-ttu-id="f1415-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f1415-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f1415-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f1415-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1415-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1415-135">Request</span></span>
<span data-ttu-id="f1415-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1415-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="f1415-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1415-137">Response</span></span>
<span data-ttu-id="f1415-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1415-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












