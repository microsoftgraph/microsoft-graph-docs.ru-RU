---
title: Удаление windowsPhone81AppXBundle
description: Удаляет объект windowsPhone81AppXBundle.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 82aa53bb94266ab8770a4616c64b449d5f611f64
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958510"
---
# <a name="delete-windowsphone81appxbundle"></a><span data-ttu-id="a2cdb-103">Удаление windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="a2cdb-103">Delete windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="a2cdb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2cdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2cdb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2cdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2cdb-106">Удаляет объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="a2cdb-106">Deletes a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2cdb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a2cdb-107">Prerequisites</span></span>
<span data-ttu-id="a2cdb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2cdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2cdb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2cdb-110">Permission type</span></span>|<span data-ttu-id="a2cdb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2cdb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2cdb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2cdb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2cdb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2cdb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2cdb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2cdb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2cdb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2cdb-115">Not supported.</span></span>|
|<span data-ttu-id="a2cdb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2cdb-116">Application</span></span>|<span data-ttu-id="a2cdb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2cdb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2cdb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2cdb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a2cdb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2cdb-119">Request headers</span></span>
|<span data-ttu-id="a2cdb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2cdb-120">Header</span></span>|<span data-ttu-id="a2cdb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a2cdb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2cdb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2cdb-122">Authorization</span></span>|<span data-ttu-id="a2cdb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2cdb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2cdb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a2cdb-124">Accept</span></span>|<span data-ttu-id="a2cdb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2cdb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2cdb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2cdb-126">Request body</span></span>
<span data-ttu-id="a2cdb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2cdb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2cdb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2cdb-128">Response</span></span>
<span data-ttu-id="a2cdb-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a2cdb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a2cdb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a2cdb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2cdb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2cdb-131">Request</span></span>
<span data-ttu-id="a2cdb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2cdb-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="a2cdb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2cdb-133">Response</span></span>
<span data-ttu-id="a2cdb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2cdb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




