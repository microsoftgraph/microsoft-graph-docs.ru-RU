---
title: Удаление объекта mobileThreatDefenseConnector
description: Удаляет объект mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f135c758828b6af50317c626e8e974d9d8c032d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528689"
---
# <a name="delete-mobilethreatdefenseconnector"></a><span data-ttu-id="6595f-103">Удаление объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="6595f-103">Delete mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="6595f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6595f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6595f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6595f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6595f-106">Удаляет объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="6595f-106">Deletes a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6595f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6595f-107">Prerequisites</span></span>
<span data-ttu-id="6595f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6595f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6595f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6595f-110">Permission type</span></span>|<span data-ttu-id="6595f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6595f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6595f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6595f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6595f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6595f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6595f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6595f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6595f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6595f-115">Not supported.</span></span>|
|<span data-ttu-id="6595f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6595f-116">Application</span></span>|<span data-ttu-id="6595f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6595f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6595f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6595f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="6595f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6595f-119">Request headers</span></span>
|<span data-ttu-id="6595f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6595f-120">Header</span></span>|<span data-ttu-id="6595f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6595f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6595f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6595f-122">Authorization</span></span>|<span data-ttu-id="6595f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6595f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6595f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6595f-124">Accept</span></span>|<span data-ttu-id="6595f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6595f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6595f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6595f-126">Request body</span></span>
<span data-ttu-id="6595f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6595f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6595f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6595f-128">Response</span></span>
<span data-ttu-id="6595f-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6595f-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6595f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6595f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6595f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6595f-131">Request</span></span>
<span data-ttu-id="6595f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6595f-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="6595f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6595f-133">Response</span></span>
<span data-ttu-id="6595f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6595f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





