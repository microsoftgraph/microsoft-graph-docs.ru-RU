---
title: Удаление windowsOfficeClientConfiguration
description: Удаление определенной политики, не влияемой на безопасность.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f0d9ebcdbccd11576fd418a4962001da19063f4d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753459"
---
# <a name="delete-windowsofficeclientconfiguration"></a><span data-ttu-id="654d1-103">Удаление windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="654d1-103">Delete windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="654d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="654d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="654d1-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="654d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="654d1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="654d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="654d1-107">Удаление определенной политики, не влияемой на безопасность.</span><span class="sxs-lookup"><span data-stu-id="654d1-107">Delete a specific non-security policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="654d1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="654d1-108">Prerequisites</span></span>
<span data-ttu-id="654d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="654d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="654d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="654d1-111">Permission type</span></span>|<span data-ttu-id="654d1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="654d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="654d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="654d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="654d1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="654d1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="654d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="654d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="654d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="654d1-116">Not supported.</span></span>|
|<span data-ttu-id="654d1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="654d1-117">Application</span></span>|<span data-ttu-id="654d1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="654d1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="654d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="654d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="654d1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="654d1-120">Request headers</span></span>
|<span data-ttu-id="654d1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="654d1-121">Header</span></span>|<span data-ttu-id="654d1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="654d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="654d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="654d1-123">Authorization</span></span>|<span data-ttu-id="654d1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="654d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="654d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="654d1-125">Accept</span></span>|<span data-ttu-id="654d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="654d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="654d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="654d1-127">Request body</span></span>
<span data-ttu-id="654d1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="654d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="654d1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="654d1-129">Response</span></span>
<span data-ttu-id="654d1-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="654d1-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="654d1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="654d1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="654d1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="654d1-132">Request</span></span>
<span data-ttu-id="654d1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="654d1-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="654d1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="654d1-134">Response</span></span>
<span data-ttu-id="654d1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="654d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```




