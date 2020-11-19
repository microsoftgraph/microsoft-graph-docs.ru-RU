---
title: Удалить vppToken
description: Удаляет vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 193c65364adbcea5166264d5177895d1a0210c67
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276870"
---
# <a name="delete-vpptoken"></a><span data-ttu-id="915cf-103">Удалить vppToken</span><span class="sxs-lookup"><span data-stu-id="915cf-103">Delete vppToken</span></span>

<span data-ttu-id="915cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="915cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="915cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="915cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="915cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="915cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="915cf-107">Удаляет [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="915cf-107">Deletes a [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="915cf-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="915cf-108">Prerequisites</span></span>
<span data-ttu-id="915cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="915cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="915cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="915cf-111">Permission type</span></span>|<span data-ttu-id="915cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="915cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="915cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="915cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="915cf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="915cf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="915cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="915cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="915cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="915cf-116">Not supported.</span></span>|
|<span data-ttu-id="915cf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="915cf-117">Application</span></span>|<span data-ttu-id="915cf-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="915cf-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="915cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="915cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="915cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="915cf-120">Request headers</span></span>
|<span data-ttu-id="915cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="915cf-121">Header</span></span>|<span data-ttu-id="915cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="915cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="915cf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="915cf-123">Authorization</span></span>|<span data-ttu-id="915cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="915cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="915cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="915cf-125">Accept</span></span>|<span data-ttu-id="915cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="915cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="915cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="915cf-127">Request body</span></span>
<span data-ttu-id="915cf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="915cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="915cf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="915cf-129">Response</span></span>
<span data-ttu-id="915cf-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="915cf-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="915cf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="915cf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="915cf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="915cf-132">Request</span></span>
<span data-ttu-id="915cf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="915cf-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="915cf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="915cf-134">Response</span></span>
<span data-ttu-id="915cf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="915cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




