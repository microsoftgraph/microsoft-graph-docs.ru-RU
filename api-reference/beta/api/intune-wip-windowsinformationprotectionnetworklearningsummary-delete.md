---
title: Удаление windowsInformationProtectionNetworkLearningSummary
description: Удаление объекта windowsInformationProtectionNetworkLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 769f2e50ec0fa37025f5de5e7d92551717503386
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993265"
---
# <a name="delete-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="dfca3-103">Удаление windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="dfca3-103">Delete windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="dfca3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfca3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfca3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfca3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfca3-106">Удаление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="dfca3-106">Deletes a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfca3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dfca3-107">Prerequisites</span></span>
<span data-ttu-id="dfca3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfca3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfca3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfca3-110">Permission type</span></span>|<span data-ttu-id="dfca3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfca3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfca3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfca3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfca3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfca3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dfca3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfca3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfca3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfca3-115">Not supported.</span></span>|
|<span data-ttu-id="dfca3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfca3-116">Application</span></span>|<span data-ttu-id="dfca3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfca3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfca3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfca3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="dfca3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfca3-119">Request headers</span></span>
|<span data-ttu-id="dfca3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dfca3-120">Header</span></span>|<span data-ttu-id="dfca3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dfca3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfca3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfca3-122">Authorization</span></span>|<span data-ttu-id="dfca3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfca3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfca3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dfca3-124">Accept</span></span>|<span data-ttu-id="dfca3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfca3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfca3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dfca3-126">Request body</span></span>
<span data-ttu-id="dfca3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfca3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfca3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfca3-128">Response</span></span>
<span data-ttu-id="dfca3-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dfca3-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dfca3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dfca3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfca3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfca3-131">Request</span></span>
<span data-ttu-id="dfca3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfca3-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="dfca3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfca3-133">Response</span></span>
<span data-ttu-id="dfca3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfca3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





