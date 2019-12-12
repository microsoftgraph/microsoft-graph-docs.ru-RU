---
title: Удаление Импортедаппледевицеидентитиресулт
description: Удаляет объект Импортедаппледевицеидентитиресулт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4be44d52239788cd811a499cde3a868a02067ee1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955282"
---
# <a name="delete-importedappledeviceidentityresult"></a><span data-ttu-id="42869-103">Удаление Импортедаппледевицеидентитиресулт</span><span class="sxs-lookup"><span data-stu-id="42869-103">Delete importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="42869-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42869-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42869-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42869-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42869-106">Удаляет объект [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="42869-106">Deletes a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42869-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="42869-107">Prerequisites</span></span>
<span data-ttu-id="42869-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42869-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42869-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42869-110">Permission type</span></span>|<span data-ttu-id="42869-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42869-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42869-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42869-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42869-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42869-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="42869-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42869-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42869-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42869-115">Not supported.</span></span>|
|<span data-ttu-id="42869-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42869-116">Application</span></span>|<span data-ttu-id="42869-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42869-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42869-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42869-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="42869-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="42869-119">Request headers</span></span>
|<span data-ttu-id="42869-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42869-120">Header</span></span>|<span data-ttu-id="42869-121">Значение</span><span class="sxs-lookup"><span data-stu-id="42869-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42869-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42869-122">Authorization</span></span>|<span data-ttu-id="42869-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42869-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42869-124">Accept</span><span class="sxs-lookup"><span data-stu-id="42869-124">Accept</span></span>|<span data-ttu-id="42869-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42869-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42869-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42869-126">Request body</span></span>
<span data-ttu-id="42869-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42869-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42869-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="42869-128">Response</span></span>
<span data-ttu-id="42869-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="42869-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="42869-130">Пример</span><span class="sxs-lookup"><span data-stu-id="42869-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="42869-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="42869-131">Request</span></span>
<span data-ttu-id="42869-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42869-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="42869-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="42869-133">Response</span></span>
<span data-ttu-id="42869-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42869-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





