---
title: Удаление объекта userInstallStateSummary
description: Удаляет объект userInstallStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e22ee0ce88b1a8a05b58293e0fba050ad22e72a0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759401"
---
# <a name="delete-userinstallstatesummary"></a><span data-ttu-id="04ae7-103">Удаление объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="04ae7-103">Delete userInstallStateSummary</span></span>

<span data-ttu-id="04ae7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04ae7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04ae7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04ae7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04ae7-106">Удаляет объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="04ae7-106">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04ae7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="04ae7-107">Prerequisites</span></span>
<span data-ttu-id="04ae7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04ae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04ae7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04ae7-110">Permission type</span></span>|<span data-ttu-id="04ae7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04ae7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04ae7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04ae7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04ae7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ae7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04ae7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04ae7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04ae7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04ae7-115">Not supported.</span></span>|
|<span data-ttu-id="04ae7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="04ae7-116">Application</span></span>|<span data-ttu-id="04ae7-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ae7-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04ae7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04ae7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="04ae7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="04ae7-119">Request headers</span></span>
|<span data-ttu-id="04ae7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04ae7-120">Header</span></span>|<span data-ttu-id="04ae7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="04ae7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04ae7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04ae7-122">Authorization</span></span>|<span data-ttu-id="04ae7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04ae7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04ae7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="04ae7-124">Accept</span></span>|<span data-ttu-id="04ae7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04ae7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04ae7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04ae7-126">Request body</span></span>
<span data-ttu-id="04ae7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04ae7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04ae7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="04ae7-128">Response</span></span>
<span data-ttu-id="04ae7-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04ae7-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04ae7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="04ae7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="04ae7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="04ae7-131">Request</span></span>
<span data-ttu-id="04ae7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04ae7-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="04ae7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="04ae7-133">Response</span></span>
<span data-ttu-id="04ae7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04ae7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




